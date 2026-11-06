# N.NavigateHierarchySystem（2026-10-14）

## 方針
- エレベーターのユーザー別共存案は採用せず、完全切替の方針。今回エレベーターのモード処理は変更しない。
- N.FloorGuide_ApproachをSF風の階段案内UIへ拡張。選択・スクロール・暗転はユーザーごとのローカル処理。
- ユーザー確認により、未整備階は無効、既存Borderと行先の権限は維持する。

## 実装
- 既存Text_UIとHighLightを使用。指先接触中に縦スライドし、短いタップの離脱で階を選ぶ。現在階は青、移動可能な選択は緑、拒否時は赤。
- Desktopは視線＋Use/LMBの保持でドラッグ、移動量が小さければ離した時に選択。外部の壁による遮蔽は維持し、案内板自身の取り付け面は無視する。
- N.Border_01/02に専用接触TriggerとnavigationSystem参照を接続。既存の通行権限・通常通行・他のBorderは変更しない。階選択だけでは権限を解除しない。
- 接触時に出発Border権限、行先権限、対応する接触領域、選択状態を確認。暗転開始→完全暗転時にローカルプレイヤーを一度だけ移動→視界復帰→選択消費。移動直前にも権限・行先・床を再検査する。
- 行先権限は現在N.ElevatorSystem.HasLocalFloorAccessを参照。運行そのものには依存しないが、当該Systemの階名・権限設定を共有する。
- 入力は案内板から4m以内で判定。選択中の権限再確認は0.25秒間隔、接触・移動直前は即時確認。
- 日本語/英語、共通ロック、折り畳み、階名付き移動先、PlayModeリセットを備える。

## 初期の配置範囲
- 操作対象は7FのN.FloorGuide_Approach。12階の一覧を保持する。
- 整備済みで安全な到着点を確認できるB2だけを移動先として開放。他階は参照・権限・床を確認して順次開放する。B2の案内板は今回操作UI化しない。
- B2案内板正面の初期候補はCapsule検査で却下。右0.7m・前0.7mの候補(-18.05,-55.96,46.96)は床と半径0.2m/高さ約1.65mの立ち空間を確認。
- Scene適用は既存内容を保持したバックアップ・Undo付き。元Sceneは自動保存しない。二重適用は既存コンポーネントを検出して停止する。

## 検証
- 新規Udon Assembly markerとProgram AssetをUnity APIで生成。GUIDは手作成しない。
- 最終UdonSharp 1,369スクリプトのコンパイル完了（66.050秒）。Scene適用後の参照確認は後述。
- VRのタップ/ドラッグ、Desktop、権限拒否、暗転の視界被覆、階段接触、到着向き、多人数の独立操作は実機確認が必要。

## Scene適用確認
- N.FloorGuide_ApproachにController 1個を配置。12行・12移動先スロット、操作BoxCollider、HighLightのText_UI配下への接続、暗転CanvasGroupを確認。
- B2到着点(-18.05,-55.96,46.96)、有効ルート数1、N.Border_01/02のControllerと専用Trigger参照を確認。
- Backing UdonBehaviourとProgram Sourceあり、Program定義のcontactBorderを確認。対象Nav/Border Program Assetのみ保存。最新Consoleエラー0。
- 操作面のWorld Boundsサイズは(0.05,1.40,0.64)。既存Canvasの向き・スケールを継承する。
- バックアップ: Temp/N_NavigateBeforeInstall_20261014_041610_125.unity。元Sceneは未保存。Udon資産の再インポートとScene保存に時間がかかりHTTPはタイムアウトしたが、その後の読取で適用完了を確認。
- 実機検証は未実施。7Fでの指スライド/タップ、Desktopの押してドラッグ/離して選択、B2選択後の階段Border接触・暗転・到着をまず確認する。
