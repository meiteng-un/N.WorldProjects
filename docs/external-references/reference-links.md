# Curated Reference Links

目的別に、N.Worldsの設計・実装・検証で参照できる公開URLを整理します。

- Last reviewed: 2026-10-12
- Rule: すべてのURLに、何の参照・参考かを一言添える
- Scope: 参考・比較用。導入やコード流用は各参照メモとライセンス確認を経て別途判断する

## UI・デザイン・テーマ

- [UI作成時の参考] [M3E4Unity — Material 3 ExpressiveのUnity uGUI / VRChat UdonSharp実装](https://github.com/NarYuki/M3E4Unity) — Apache-2.0。NOTICE、フォント、第三者依存の条件を確認してから利用する。 [詳細メモ](M3E4Unity.md)

## VRChat公式・Udon・World仕様

- [VRChat World作成の公式基準] [VRChat Creator Docs](https://github.com/vrchat-community/creator-docs) — SDK、Udon、Worldの公式仕様・制約を確認する。
- [Udon GraphのPlayModeとBuild & Testの違い] [Creator Docs: Udon Graph](https://github.com/vrchat-community/creator-docs/blob/main/Docs/docs/worlds/udon/graph/index.md) — Editor内テストとVRChat実行テストを分ける参考。
- [新規VRChat Worldの初期構成] [VRChat Community template-world](https://github.com/vrchat-community/template-world) — UdonSharp付きWorldプロジェクトの最小構成を確認する。ライセンスはVRChat SDK利用条件に従う。

## World作成・Editor支援

- [VRChat WorldのEditor補助と品質向上] [oneVR/VRWorldToolkit](https://github.com/oneVR/VRWorldToolkit) — MIT。Trigger-based occlusion、Custom Editor、Texture処理などの比較参考。
- [UdonSharp挙動・Prefab実装例] [Reava/UwUtils](https://github.com/Reava/UwUtils) — MIT。UdonSharpの小規模なWorld機能とUI補助の実装例を確認する。

## 性能・容量・ビルド品質

- [VRChat Worldのビルドサイズ最適化] [VRCWorldBuildOptimizer](https://github.com/kuzuki-y/VRCWorldBuildOptimizer) — MIT。Texture、Mesh、Audio、Reflection Probe、Fontの最適化とBackup/Restoreの設計を比較する。

## X・投稿・速報情報

X投稿は未確認の参照候補と確認済みの参考を区別して登録します。採用前に引用元・スレッド・公式リポジトリを必要に応じて確認します。

- 追加候補は [X・YouTube参照記録テンプレート](social-video-reference-template.md) で記録してから一覧へ移す。

## YouTube・動画解説

YouTubeは、チャンネル、公開日、該当タイムスタンプ、説明欄の出典を確認できた動画を登録します。

- 動画の主張と公式ドキュメント・リポジトリで確認した事実を分けて記録する。
- 長い字幕や台本は転載せず、必要箇所を要約する。

## 利用時の注意

- 参考URLの内容は取得時点の情報であり、SDK、Unity、VRChat、投稿者の更新で変わる可能性がある。
- 外部コードをそのままN.Worldsへコピーせず、まず設計・依存・入力・同期・性能・ライセンスを比較する。
- M3E4Unityの評価計画は [こちら](../design/m3e4unity-ui-evaluation.md)。
- 検証結果は [Evidence Levels](../validation/evidence-levels.md) に沿って記録する。

## ユーザー指定の参照候補（2026-10-12登録）

用途はユーザー指定。Xの本文・添付画像・動画・投稿日時・引用元・利用条件は未確認です。kuloqui_投稿は直接取得を試みましたが取得エラーでした。他のX投稿は未取得です。未確認でも候補として保存し、採用する作業時に必要な投稿だけ確認します。URLの追跡パラメータと末尾空白を除去しました。

### VRChat内で目指すUI挙動（ユーザー指定）

- [VRChat内の理想に近いUI挙動] [@kuloqui_の投稿](https://x.com/kuloqui_/status/2108482618979389592) — 内容未確認・参照候補。
- [VRChat内の理想に近いUI挙動] [@yui540の投稿](https://x.com/yui540/status/2105533001786658823) — 内容未確認・参照候補。
- [VRChat内の理想に近いUI挙動] [@hancore_linuxの投稿](https://x.com/hancore_linux/status/2103902738845520201) — 内容未確認・参照候補。
- [VRChat内の理想に近いUI挙動] [@k0ii81の投稿](https://x.com/k0ii81/status/2104088269378265096) — 内容未確認・参照候補。
- [VRChat内の理想に近いUI挙動] [@justalexokiの投稿](https://x.com/justalexoki/status/2103841051228418113) — 内容未確認・参照候補。

### VRChatに実装したいギミック（ユーザー指定）

- [VRChatギミック実装の参考] [@lucknknockの投稿](https://x.com/lucknknock/status/2108513110445498686) — 内容未確認・参照候補。
- [VRChatギミック実装の参考] [@teRugWembV78059の投稿](https://x.com/teRugWembV78059/status/2103343389391614154) — 内容未確認・参照候補。
- [VRChatギミック実装の参考] [@xi100の投稿](https://x.com/xi100/status/1985205888379154671) — 内容未確認・参照候補。
- [VRChatギミック実装の参考] [@RR_vrchatの投稿](https://x.com/RR_vrchat/status/2104051031730712617) — 内容未確認・参照候補。
- [VRChatギミック・表現の参考] [@threejsの投稿](https://x.com/threejs/status/2103931735113392379) — 内容未確認・参照候補。

### VRChatコンポーネント設定値

- [VRChat関連コンポーネント設定値の参考] [@lpcwstrの投稿](https://x.com/lpcwstr/status/2106647576590389544) — 内容未確認・参照候補。

### 画像生成

- [画像生成時の参考] [@shimotti_aiの投稿](https://x.com/shimotti_ai/status/2102325574723383436) — 内容未確認・参照候補。

### 汎用Skills・開発支援

- [便利なSkills群の情報収集] [@taiga_aiiの投稿](https://x.com/taiga_aii/status/2083855348767887487) — 内容未確認・参照候補。

### 水・波・光学表現

- [VRChatの水表現・ギミック設計の参考] [SamG-Coder/clearwater](https://github.com/SamG-Coder/clearwater) — 公開README確認済み。CUDA由来のWebGPUデモとWindowsネイティブ版、FFT水面・波紋・光学表現の参考。Unity/VRChat用パッケージではないため、直接導入可能とは判断しない。ソース・ライセンス・VRChat互換性・性能は採用時に別途確認。

### UdonSharp用Skills

- [UdonSharpのVRChat Worldギミック作成Skillsの参考] [niaka3dayo/agent-skills-vrc-udon](https://github.com/niaka3dayo/agent-skills-vrc-udon) — 公開ページ確認済み。UdonSharp生成を支援するSkills・rules・validation hooksの比較候補。個別SKILL.md・スクリプト・ライセンス・既存Naturlin規則との衝突は未確認。未インストール。

### 確認・反映の順序

- UI作成時は既存のM3E4Unity参照と上記UI挙動候補を組み合わせ、外観と操作挙動を分けて評価する。M3E4Unityは既存登録を再利用し重複登録しない。
- 画像解析・画像生成・適した長時間の調査はサイドパネルのChatGPT.comプロジェクト「N.WorldProjects Codex x ChatGPT-Web」を使う。必要なURL・問い・制約だけを渡し、結果を短い参照メモに戻す。アクセス不能なら未確認として報告する。
- 動画は実際に確認できた区間・タイムスタンプを記録し、見ていない挙動を推測で断定しない。参考元のコード・画像・動画は権利確認なしに転載しない。
- 実装は別途依頼の範囲で行い、Unity/UdonSharp・Desktop/VR入力・同期・性能を検証する。この一覧追加だけではコード変更・Skillsインストール・定期監視を行わない。

## 屋上使用アセット（ユーザー指定・2026-10-12）

- [R階の建築・空間構成に使用] [Abstract:Echo — QuickBrown Design Studio](https://lura.booth.pm/items/4490469) — 商品名/説明を確認。Coast Dark Pack/Full Packとの拡張構成の案内あり。所持版・導入状態・個別ギミックは未確認。
- [R階の建築・空間構成に使用] [Abstract:Coast — QuickBrown Design Studio](https://lura.booth.pm/items/3675835) — 商品名確認。Echoとの具体的な部品配置は未指定。
用途と接続案は[階用途表](../design/seamless-world-layout.md)。商品アセット本体は転載しない。ページの規約表記と購入版に付属する規約を実際の改造前に照合する。
