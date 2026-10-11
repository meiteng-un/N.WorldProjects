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

X投稿は、投稿だけでなく引用元・スレッド・公式リポジトリまで確認できた場合に登録します。

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