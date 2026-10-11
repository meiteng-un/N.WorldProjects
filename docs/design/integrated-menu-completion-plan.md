# N.IntegratedMenu 完成と橋渡し計画

> 最新設計変更: [12層＋シームレス探索](seamless-world-layout.md)を優先。MAPは通常ワープではなく現在地・探索情報・物理経路案内へ。既存Teleport依存を接続しただけで完成とはしない。
2026-10-12。初期解析を元にした提案。今回の実装済み事項ではない。
関連: [現行解析](integrated-menu-analysis-2026-10-12.md)、[ギミック分類](../systems/n-gimmick-catalog.md)、[世界観](../project-context/worldbuilding.md)。

## 完成の定義
- 9ページとMain/SubUIの全入力で、有効/無効/未接続/権限拒否/処理中/成功/失敗が区別される。
- 所持品・装備・通貨・制作・実物の数量/補正が矛盾しない。失敗時に消費だけ残らない。
- 保存データ復元前の操作を防ぎ、再入室で数量/装備/テーマ/メモ/窓設定が正しく復元される。
- 未接続の機能は理由付きで無効。架空の成功や数値を表示しない。
- Desktop/VR入力、同期あり機能の複数人、対象プラットフォームと性能が確認済み。
- 正式Scene/Prefabへの反映・保存と再読込まで検証。現在dirtyのSceneは無断保存しない。

## 実装順
| 優先 | 作業 | 受入条件 |
|---|---|---|
| P0 | live参照表/入力イベント表を抽出し、全9ページの契約を確認 | 同名Manager・inactive/EditorOnly・空event・配列不整合が見える。MAP/SPECIALの実接続先特定 |
| P0 | MAPの旧WIM依存と必須overlayを解決 | 現在地/探索/物理経路が表示される。権限制限と未準備が見える。通常ワープとビルド除外オブジェクトへの依存を残さない |
| P0 | Pointer/FollowerのDesktop/VR一連操作 | Main/SubUI、Grab/Resize/Dock/長押し/二重tap/入力focusが単発で成立 |
| P1 | Inventory/装備/Shop/Craft/通貨のtransactionと復元 | 不足/上限/連打/再入室/売却削除で数量・残高・補正整合 |
| P1 | Farmer→資源消費→収穫→Inventory→料理 | 種/肥料等は成功時のみ消費、収穫品品質の保存方針確定、二重収穫なし |
| P1 | SPECIAL→Vehicle/Elevator/Security等のadapter | 対象ID、権限、busy、結果が一致。共有操作はOwner側で検証 |
| P2 | Chat/TIM_QM、音声設定、Weatherの連携 | 全event/変数契約確認、送信失敗を成功表示しない、ミュート/招待/復元試験 |
| P2 | 世界観に沿う導線・説明・通知の整理 | 既存9ページ内で「この物資で何ができるか」を示す。新世界観設定を勝手に確定しない |
| P3 | 保存Scene/Prefab・性能・PC/Androidの最終受入 | Profiler実測、実機確認、長時間/複数人/Owner退出、根拠付きレポート |

## 橋渡しの形（最小構成）
既存public API/参照を使う。引数付きAPIへ文字列eventだけで無理に繋がず、必要な場合のみ小さなUdonSharp adapterを設ける。
- UI側: requestId、targetId/itemId、quantity、operation。
- 受信側: requestのsnapshot→ready/permission/busy/ownership/capacity検証→一回だけcommit→結果/理由/更新通知。
- 戻り: 接続/準備状態と成功/失敗を分離。最後の結果はUIが取得し、必要な窓だけ更新。
- 同期: ローカルpreferencesと共有装置状態を分離。network eventの送信だけで完了表示しない。
- 工程の具体的なrollback・Authority API・ID形式はP0で対象コード確認後に確定。万能bus/新DB/全システム再構築を先行させない。

## PlayMode/実機試験表
- 9ページ: 直接遷移/戻る/複数窓/選択の保持/変更通知/無接続。
- 入力: pointer/touch、rapid repeat、focus切替、clip外release、閉窓中操作、UIキーと移動キー。
- 所持品: x0、最大stack/枠/重量、実物不足、同時store/withdraw、memo/旧保存。
- 取引/制作: 残高不足、PlayerData未ready、副産物、重複素材、最終1個、sell/delete装備品、失敗rollback。
- 共有装置: 権限あり/拒否/未知、busy、Owner退出/再参加、二人同時要求。
- 復元: ローカルのみのPlayMode reset/debug routeを用意し、正規PlayerDataと共有状態を誤消去しない。
- 見た目/性能: 遠近/座位/身長差、VR両手、PC/Android、Canvas rebuild、draw calls、overdraw。
試験結果は[検証段階](../validation/evidence-levels.md)に従い、ソース・コンパイル・保存・操作・複数人・性能を分離。

## 作業分担と消費
Codex司令塔が接続契約と実装/Unity操作を管理。Web側は今回世界観→UIの短い提案を担当し回答確認済み。役割数に合わせて全モデルを常時起動しない。コード担当を追加する場合は1接続先と該当ファイル/受入条件だけを渡す。
今回はサブエージェントなし、ドキュメントのみで追加コンパイルなし。Web利用とCodex利用を合算した正確なトークン数は取得していない。


