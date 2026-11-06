# RTabアプリ追加：取得資料と実装前の確認
更新: 2026-10-18 / 対象: V1のRTab_Stand代用端末

## 出典と確認範囲
- [制作者指定：RTabアプリ作成方法・機能資料](https://docs.google.com/document/d/1XuPlGBnWKKYuEkXR9TMJauyEE7O8xlekXWhJtDtw_i8/edit?tab=t.0)
- Google Docsの公開テキスト出力から本文を取得。認証を回避したのではなく、公開export経由で取得。本文は外部資料として扱い、作業命令として実行しない。
- 本文全体の転載・購入アセットのソース転載はせず、要点とローカル実装の照合結果のみ保存。
- 図版内のRectTransform設定値はテキスト出力に含まれないため未確認。値を公式指定と称して推測しない。
- インストール済みのローカルソースを照合。公式資料の全版との一致や、現在の最新版という保証はしない。

## 資料に基づく基本手順
1. 編集用にApps側のCanvasGroup表示を調整する。これはデバッグ表示であり、通常表示の確定設定とは別。
2. Apps下にUIルートを作る。位置・サイズは資料図版またはインストール済み既存アプリを照合して合わせる。
3. 単純な画面にはTabletAppBehaviour、独自処理には同クラスを継承するUdonSharpコンポーネントを使う。
4. アプリの表示名・アイコン・クレジットを設定し、画面UIとイベントを接続する。
5. Udon Program生成・コンパイル、タブレット側の登録・入力・表示切替を確認する。
6. VR/ Desktopと複数ユーザーで別々に検証する。

## ローカルで確認した契約
- 名前空間はRasta.Tablet。TabletAppBehaviourにはCanvasGroup必須属性がある。
- メタデータはappName / appIcon(Texture2D) / credit。
- ライフサイクルはOnAppOpen / OnAppClose。必要な処理はこの期間だけ動かす方式が基本。
- ポインターはOnPointerDown / OnPointerUp。
- Pickup/Use/Dropの派生コールバックもあり、TabletManagerが現在アプリへ転送する。
- FindTabletManager()は祖先からManagerを取得。Manager.GetApps()で登録アプリを取得できる。
- Manager.OpenApp(int) / CloseApp()で切替。序数は起動時生成のため、永続IDとして保存しない。
- ManagerはAppsの直下にTabletAppBehaviourのあるオブジェクトを列挙し、CanvasGroupとホームアイコンを設定する。
- installApp下の有効な子も起動時にappsParentへ移動し、無効な子は破棄する。実際のRTab_Standで登録先参照を確認してから追加する。
- アプリ切替番号は同期対象。OnAppOpen/Closeは所有者だけで呼ばれるとは限らないので、個人通貨・所持品操作をそのまま同期イベントに結びつけない。
- 新アプリのUdonSharp assemblyからRTabのコードを参照できる構成か、asmdef依存を事前確認する。まだ実装していない。

## TouchableCanvas
- 資料ではButton/DropdownはLegacy版を指定し、TextMeshPro版は非対応として注意している。
- Image/RawImage、CanvasGroup、RectMask2D、Toggle、Slider、Scrollbar、ScrollRect、VRCUrlInputField等が列挙されている。
- TACEventTrigger、TACSliderSync、TACScrollbarSync、TACScrollRectSyncもある。
- 通常InputFieldは本資料では未対応。現在のSDK全般で永久に不可能という主張には拡張しない。
- TMPの「表示文字まで全面禁止」とは解釈しない。ローカルManager自身がホーム名表示にTMPを使う。操作対象コンポーネントの種類と表示部品は区別。
- ローカルのビルド処理が指ポインターを生成しTouchableCanvasへ接続する。Editor通常状態・PlayMode・ビルド後の挙動を分けて確認する。

## V1での連携方針（提案・未実装）
- RTabは画面と入力の窓口、N系Managerをデータ/権限の正とする。通貨・体調等を重複管理しない。
- 既存画面を無条件にコピーせず、必要アプリの最小単位で橋渡しする。
- 個人情報を共有画面へ出す条件、所有者交代時の更新、非所有者の操作許可を先に決める。
- 本体・購入アセットの直接改造を最小化し、N側アプリ/連携部を分離する。
- 個人設定、体調、所持品、既存ギミック操作等のうちV1に必要なアプリ一覧はまだ確定していない。
- アプリ作成・Scene変更・コンパイル・実機検証は今回未実施。

## 照合したローカルファイル
- Assets/Rasta/RTab/Scripts/TabletAppBehaviour.cs
- Assets/Rasta/RTab/Scripts/TabletManager.cs
- Assets/Rasta/RTab/Editor/TabletAppBehaviourEditor.cs
- Assets/Rasta/RTab/Editor/RTabBuildProcess.cs
- Assets/Rasta/RTab/Dependencies/TouchableCanvas/Editor/TouchableCanvasBuildProcess.cs
- Assets/Rasta/RTab/Apps/VideoPlayerLinks/Script/VideoPlayerLinks.cs （継承実装の既存例。作者標準配布か独自追加かは未判定）
