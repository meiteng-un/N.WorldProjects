# Design Notes

新機能、既存機能の変更、UI/Input、同期、Inspector、Prefab構成などの設計を記録します。

## 設計メモの基本構成

- 背景と目的
- 現在の挙動
- 要求する挙動
- 対象Scene/Prefab/Script
- 入力経路
- 状態遷移
- データと同期
- 既存機能との競合
- 実装案
- 代替案と不採用理由
- Unity/PlayMode/VRChatでの検証項目
- 未決事項

## ファイル名

`docs/design/YYYY-MM-DD-short-name.md`

## ルール

設計段階では実装済みと表現せず、決定済み・提案中・未確認を明記します。UIだけを追加する場合も、実際に呼び出される処理、入力イベント、状態更新、保存先まで確認対象にします。
