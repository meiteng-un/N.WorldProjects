# N.ElevatorSystem 仕上げ変更（2026-10-12）

## 方針

PlayMode性能改善はユーザー指示で保留。ワールドのVRChat実機ではFPS問題なしとのユーザー報告。7F↔B2先行運行を維持し、今回他階は開放しない。

## ソース実装

1. 無人待機時の扉再開放: `reopenEmptyIdleCabin` と `idleDoorNearbyRadius`（既定3m）。かご内0人かつ周辺無人、別階要求なし、保守・非常停止中でないとき、閉鎖後の保持時間を過ぎると開放。判定は各台0.25秒間隔。別階要求がある場合は運行を優先する。
2. 到着表示の補強: 状態だけでなく現在階の変更も監視し、かごと到着階の扉へ表示を再適用。停止解除後のAnimator速度も更新。ただしB2扉が開かない症状の根本原因・解消は実機未確認。両かごとB2乗り場のAnimatorは有効・Always Animateだった。
3. FloorCount: パネルにTMP_Text参照を持たせ、現在階変更時だけN.ElevatorSystemの階名を表示。移行メニューはFloorCount_*を接続し、移動するかご内のStaticとRenderer動的オクルージョンを解除する。監査時のFloorCountはactive/enabled、alpha=1、static=0で、無効化や透明色が原因ではない。視認不可の解消は未確認。
4. N.ElevatorButtonに `usePanelMode` を追加。旧個別形式は維持。親1個にボタン親Transform、Collider、種類（呼出/開/閉/行先）、階番号、発光MeshRenderer、任意Material、可動MeshRendererを配列で設定。Permission・Audio・発光色設定はパネル共通。各ボタンの指定材質は任意で、未指定なら現在の材質を維持。

## 入力経路

- Desktopパネル: Head視線Ray → 設定した各Colliderの最寄りヒット → 非Trigger遮蔽物を確認 → InputUseで命令。親の標準Interactは無効化し二重入力を防ぐ。従来の子Udon Interactプロンプトはなくなる。
- VRパネル: 左右人差し指をパネルごとに取得 → 各親のローカル押下軸・半径・深さを判定 → 押し始めだけ命令 → Hapticと可動Mesh・発光を更新。
- パネルのプレイヤーTrigger操作と旧外部PressFromExternalEventは割当先が曖昧なので無効。外部から個別スロットを操作するAPIは未提供。
- グループ判定と所有権取得は従来のCommand経路を利用。Cooldownとエラー表示はパネル共通。
- 他ギミックのInputUse、保持中Pickup、別UIとの入力競合、VR手指の個人差、押下面の距離や遮蔽物は実機で確認が必要。

## Scene移行

メニュー:
- Tools/Naturlin/N.ElevatorSystem/Hotel/Preview Cabin Panels and Displays
- Tools/Naturlin/N.ElevatorSystem/Hotel/Migrate Cabin Panels and Moving Displays

A/B各14個のかご内ボタンを親2個へ集約する。乗り場24個は維持し、合計52→26個のN.ElevatorButtonになる予定。Systemのボタン参照を差し替えてから旧Proxy/BackingをUdonSharpUndoで削除する。ボタンGameObject、Collider、AudioSource、購入アセットの元ファイルは削除しない。

確認ダイアログ、Tempへの未保存状態を含むSceneコピー、Undo、失敗時のUndo復帰付き。元Sceneは自動保存しない。既に集約済み、台数/Scene/個数が異なる、権限・押下軸が不揃い、複数発光/可動メッシュ等の場合は安全のため停止する。配列ごとに手動設定する移行も可能。

このレポート作成時点では確認ダイアログを呼び出し済み、適用完了ログとバックアップ生成は未確認。Scene集約済みとは扱わない。

## 検証

- C# Runtime/Editor DLL更新確認。
- 更新後のUdonSharp 1368スクリプト完了ログ確認（56.369秒）。
- Buttonの `panelFloorTexts` / `usePanelMode`、Systemの `reopenEmptyIdleCabin` がProgram fieldDefinitionsに存在することを確認。
- 対象2個のProgram AssetだけをSaveAssetIfDirtyで保存。元Sceneを保存しない。
- 更新後Consoleエラー0（Synapticフィルター付き）。
- PlayMode性能再測定・新UIのPlayMode操作・VRChat実機・2人同期は行っていない。

## 実機確認項目

7F→B2→7F、両台の扉、到着時のFloorCount表示、降車後の無人常開、近傍滞在中の手動閉鎖、別階要求の優先、保守/非常停止、左右手の指押し、Desktop視線＋Use、拒否時発光、途中参加・所有者交代。他UI・Pickupとの競合も確認する。

## 公式参照

[VRChat Input Events](https://creators.vrchat.com/worlds/udon/input-events/) — InputUseはDesktopの左クリック、キー再割当対応。パネルの共通入力経路に使用。
