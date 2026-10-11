# N.WorldProjects

VRChat / Naturlin 系プロジェクトの、エラー修正・設計・検証・議論をまとめるための共同作業リポジトリです。

## 目的

- 再現条件とエラーの記録を残す
- 修正案と設計案をレビュー可能な形で共有する
- Unity上の確認結果と、未確認の範囲を分けて記録する
- 決定事項を後から追跡できるようにする
- 公開されている外部プロジェクトを、ライセンスと出典を保った上で比較・評価する

## 置き場所

- [CONTRIBUTING.md](CONTRIBUTING.md): Issue、設計、PRの進め方
- [docs/errors](docs/errors/): エラー、再現条件、修正状況
- [docs/design](docs/design/): 設計案、代替案、影響範囲
- [docs/decisions](docs/decisions/): 決定事項と理由
- [docs/notes](docs/notes/): 調査メモ、打ち合わせメモ、次回確認事項
- [docs/project-context](docs/project-context/): プロジェクト固有の基準と前提
- [docs/validation](docs/validation/): 検証段階と証拠の分類
- [docs/external-references](docs/external-references/): 公開リポジトリ・資料の出典、ライセンス、評価
- [.github/ISSUE_TEMPLATE](.github/ISSUE_TEMPLATE/): エラー報告・設計議論の入力テンプレート

## 基本ワークフロー

1. Issueで「エラー」「設計」「調査」などの目的を明記する。
2. 再現条件、期待動作、実際の動作、ログ、対象Scene/Prefab/Scriptを記録する。
3. 設計変更がある場合は `docs/design/` に案を置き、影響範囲と未確認事項を列挙する。
4. 外部プロジェクトを参照する場合は、URL、取得日、ライセンス、参照箇所、採用範囲を `docs/external-references/` に残す。
5. 実装はブランチとPull Requestで行い、検証結果をPR本文に追記する。
6. 方針が確定したら `docs/decisions/` に決定事項を残す。

## 状態の扱い

- **未確認**: まだ実環境で再現・検証していない
- **調査中**: 原因や影響範囲を確認中
- **修正案**: 実装前の提案
- **検証待ち**: 修正はあるがUnity/VRChat上の確認が未完了
- **完了**: 必要な検証まで記録済み

## 注意

ログやスクリーンショットを追加するときは、トークン、個人情報、非公開URL、不要なワールド参加者情報を含めないでください。Unity上で成功したことと、Scene保存・PlayMode・実機確認が済んだことは別々に記録します。