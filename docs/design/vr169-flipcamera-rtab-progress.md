# VR169_VL2 / FlipCamera / RTab連携：実装途中
更新: 2026-10-18。完成・Scene適用を意味しない。

## 確定要件
- VR169_VL2を本体とし、外観と撮影機能を残してFlipCameraを追加する。
- 物理ボタン、側面レバー、モニターを掴むチルト/位置調整、縦横切替などを省略しない。
- 撮影からRTabへ自動保存するのでなく、FlipCameraのプリントを写真アプリ表示中のRTabへ近づけて取り込む。
- 写真の再入場後の永続保存は未確定。

## 出典（参照目的）
- [VR169の操作と機構](https://docs.sangoustudio.com/VR169/en/controls/index.html)
- [VR169の制御パラメータ](https://docs.sangoustudio.com/VR169/en/exmenu/index.html)
- [VirtualLens2外部制御](https://vlens2.logilabo.dev/ja/docs/development/)
- 公式資料と導入済みアセットのバージョン差を確認してから各機能を移植する。アバター向けExMenu/ジェスチャー/OSC CompanionをUdonがそのまま利用できると仮定しない。

## 実施済みソース変更
- VirtualLens2.Editor/Generatorsのasmdefにcom.vrchat.avatars有無によるコンパイル条件。Worlds-onlyでSDK3 Avatars名前空間エラーが出るEditor処理を除外。Runtimeは残す。
- 上記修正後、Unity Compilation OKとConsoleエラー0件を確認。その後の写真取り込み変更は再検証待ち。
- FlipCamera Photoにプリント画像/撮影IDの読出しAPIを追加。ダウンロード待ち/失敗中は取り込まない。
- RTab PhotoViewerにプリント参照配列、スキャン位置/距離、上限を追加。
- アプリ表示中のみ0.2秒間隔で参照写真を順次確認。Managerとアルバムのローカル所有者のみ取り込み。
- 撮影ID単位で重複防止。RenderTextureをコピーするので元プリント再利用に追従しない。
- 既存アルバム追加経路へ接続し、縦横比/解像度をソース画像に合わせる（各辺最大2048）。
- 取り込み画像はローカルの実行中Texture。既存のアルバムメタデータ同期は画像バイト転送ではないため、別ユーザー/後入りへの画像共有を保証しない。

## 次の必須作業
- 写真追加コードのC#/UdonコンパイルとScene参照設定。実際のRTab_Stand配置・所有権構成を確認する。
- 撮影ID/写真再利用/ダウンロード待ち/重複/アプリ閉鎖/距離/上限/複数ユーザーを検証。
- 実画像プレビューと原画像の回転/透かし処理を照合。生RTコピーなのでプリント材質にだけ掛かる演出は一致しない場合がある。
- エラー修正以外のVR169本体制御・FlipCamera融合Prefab・レバー/モニター操作はまだ未実装。
- ワールド用の入力と光学制御を一つずつ対応付け、実機確認前に完成扱いにしない。
- 今回Scene/Prefab保存はしていない。購入アセットのソースパッチは更新時に上書きされ得るため差分を保持する。

## 追加進捗：ワールド入力プロトタイプ
- N.VirtualLensWorldを別Runtime/Editorアセンブリに作成。接触ボタン、Grabレバー、モニターチルト/回転、所有者Flip撮影イベント呼出しの土台。
- Program AssetとUdon assembly markerは登録メニュー実行・ファイル生成まで確認。U#コンパイルは手動方針に従い未実行。
- 絞り/フォーカス/ロックは状態値までで光学系へ未接続。縦横は軸回転のみでセンサー連携未実装。元の全機能はまだ未再現。
- Scene・融合Prefabの作成/参照設定・同期・Desktop・VR実機検証は未実施。初期無効。
- 検証メモ: Assets/N.Assets/N.Script/N.VirtualLensWorld/Docs/QuickVerify.md
- 最終Console読取りがタイムアウト。メニュー登録成功を全U#・動作成功とは扱わない。


## 最新のScene適用・検証（2026-10-18、上記の古い未適用記録を更新）
- Scene上に N.VirtualLensWorld_Fused を作成し、Camera/FlipCamera/5ボタン/2レバー/モニター軸を割当て済み。
- 更新版Prefab: Assets/N.Assets/N.Prefab/N.VirtualLensWorld/N.VirtualLensWorld_Fused_001.prefab。初期試作も比較用に保持。
- 原本VR169_VL2/FlipCameraはScene内で非アクティブ・EditorOnlyとして保持。購入元Prefabそのものは変更しない。Sceneは未保存、Undo可能。
- ライブプレビューの撮影先RT追従、中央ColliderレイAF、ロック、AF/MFとMFレバー、絞り/ピント反映用のN側簡易被写界深度を接続。
- VRはカメラを持たない手でボタン・レバー・モニターを操作。モニターを掴む手のUseで画面回転。レバーUseのQuick Actionも追加。
- Desktopは照準+Use、ホイールのズーム、Shift+ホイールの絞り、Ctrl+ホイールのピント。自己Pickup Colliderを無視し外部の壁には遮られる。操作中の誤撮影を抑止。
- 操作者/所有権ガードと変更時最大5Hzの設定同期、PlayMode用の操作リセットを追加。
- 可動部に必要なVRC Constraintは保持。体格/顔/自撮りのアバター依存制御と不要なAvatar Animator参照をコピー側のみ停止。
- RTab写真参照10件/有効10件を再読確認。アプリ表示中に0.2秒間隔でプール全体を走査し、撮影済み・受信完了・shot ID一致の画像のみコピー。1走査最大1枚、重複防止/上限あり。
- 最新差分を含む1,378スクリプトのU#コンパイル完了を確認（55.884秒、player compile要求後53.665秒）。ShaderHasError=False、撮影Camera Depth=Depth/Stereo=None、プレビュー有効も確認。
- autoCompileOnModify=0は維持、アップロード時コンパイルは有効。新規Program更新時のSDK自動検査と最後の明示的compileで検証。
- 実機動作確認はユーザー方針により最後にまとめる。PlayMode、VR/Desktop操作、複数ユーザー、ワールドビルドは未検証。

### 未完成と差異
- N側の被写界深度は9サンプル簡易版。VirtualLens2/LogiBokehの完全移植・同画質ではない。透明物/深度を書かない対象に制約、Quest未検証。
- ボタンはワールド用割当（撮影/ロック/画面回転/画角リセット/AF-MF）。元のFunction階層メニュー、起動/安全ジェスチャー、Face/指/擬似視線AF、Drone/Reposition/Selfie、HUD/グリッド/ピーキングは未移植。
- 画面回転とセンサー縦横/写真RT縦横比は未連動。
- RTab撮影アプリの遠隔操作UI、画像の再入場後永続保存、別ユーザーへのアルバム画像ピクセル転送は未実装。生RTのコピーでありプリント用Shaderの回転/透かしまで焼き込む処理はない。
- 従って「VR169_VL2全機能の融合が完成」とは扱わない。購入アセット更新による上書きにも注意。

検証手順と詳細はプロジェクト内 Assets/N.Assets/N.Script/N.VirtualLensWorld/Docs/QuickVerify.md に記録。
