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
