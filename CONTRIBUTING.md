# Contributing

## Issueを作るとき

タイトルの先頭に目的を付けます。

- `[Bug]` 再現する不具合
- `[Design]` 設計案や仕様の相談
- `[Investigation]` 原因調査や比較
- `[Task]` 実装・検証タスク

最低限、次を記録します。

- 対象プロジェクト、Scene、Prefab、Script
- 再現手順
- 期待した動作と実際の動作
- Console/Editor.logなどの関連エラー
- 既に試したこと
- 未確認の範囲
- 完了条件

## 設計メモ

設計案は [docs/design](docs/design/) に置きます。実装方法だけでなく、入力経路、状態遷移、同期、既存機能との競合、Inspector設定、PlayMode/実機での検証方法を記録してください。

複数案がある場合は、採用しなかった案と理由も残します。

## エラー修正

エラー記録は [docs/errors](docs/errors/) に置きます。ログの一行だけで原因を断定せず、再現条件と対象オブジェクトを分けて確認します。

「スクリプト解析成功」「Unity Consoleが綺麗」「Scene保存済み」「PlayMode確認済み」「VRChat実機確認済み」は別の証拠として扱います。

## Pull Request

PR本文には次を含めます。

- 変更目的
- 変更ファイル
- 影響する入力・状態・参照
- 検証した内容
- 未検証の内容
- 既知のリスク
- 関連Issue

ブランチ名の例:

- `fix/<short-name>`
- `design/<short-name>`
- `docs/<short-name>`
- `investigate/<short-name>`

## 情報管理

認証情報、トークン、個人情報、非公開URL、不要なユーザー識別子はコミットしないでください。大きなUnityログやバイナリは、必要性と保存場所を確認してから追加します。
