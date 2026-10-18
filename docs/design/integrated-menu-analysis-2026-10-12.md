# N.IntegratedMenu 現行解析
更新: 2026-10-12。目的: 完成に向けて担当・入力・状態・関連性・未確認を分離する。今回ランタイムコード、Prefab、Sceneの変更は行っていない。

## 検証した範囲
- 対象: D:\VCCUnity\VRChatProjects\N.Worlds Project。
- ライブScene: Assets/N.Assets/N.Scene/N.GimmickTest_002.unity。5,845 GameObjects、497 active。dirty=trueを観測。保存/破棄せず保護。
- N.IntegratedMenu、Inventory、DynamicObject、Status、Movement、Vehicle、Swim、Flying、Farmer、Pet、通貨/権限/Chat/TIM_QMのルートを確認。
- WorldIntegratedMenuルートはinactive、EditorOnly。旧WIMの子コンポーネント参照が実行可能とは保証しない。
- 読取専用のValidate Current Scene実行結果: invalid references=0、VRCUiShape=0、hit targets=751、wired events=669。メニュー配下: Objects=4136、Images=1803、TMP=1030、CanvasRenderers=2892、MeshRenderers=403。
- このvalidatorはnull入力参照等の限定検査。配列長整合、イベント名の実在、全Managerの割当、権限、transactions、保存、実入力までは証明しない。オブジェクト数はdraw callや毎フレーム負荷の実測ではない。
- 前作業のコンパイルエラーなしはユーザー確認。今回は解析/文書化のためコンパイルしていない。PlayMode、VR、Desktop、複数ユーザー、Profilerは未実施。

## 層と担当
| 層 | 主担当 | 責務 |
|---|---|---|
| 窓/入力 | NMainMenuFollower、NIntegratedMenuPointer | 開閉・追従/固定・位置/回転・Resize・Dock・独立窓、ローカル入力解析 |
| 画面統合 | NWIMMenuShell | 9ページ/選択/連携窓のナビ、各機能への委譲、表示更新、チャット・テーマの保存 |
| UIアダプター | NWIMInventoryModule、NWIM*Page | 所持品表示/ソート/メモ/決済仲介、各ページの参照とUI状態 |
| ドメイン | NInventoryManager、NDynamicObject、NStatusSystem、通貨/権限/装置Manager | 所持数、取引、装備、実物、状態、装置制御。UIは別の在庫正本を作らない |
| Editor | NWIMMenuPrefabBuilder、ReferenceBinder、ExperienceBuilder、Optimizer、Validation | 生成・移行・参照接続・検証。ビルド/修復メニューは読取専用解析とは分ける |

N.IntegratedMenuはScene上の統合ルート名。N.MainMenuはFollower/Pointerのスクリプト保存分類。N.WIMExtensionsはUI shellとWIM向けアダプター群。別々の在庫/装備システムではない。

## 9ページ
| page | 担当/到達先 | コードで確認した機能 | 次の検証 |
|---|---|---|---|
| 0 MAIN | Shell | StartでShowPage(0)、ユーザー/インスタンス表示、ページ導線 | 新規/再開/独立窓の初期状態、お知らせの実データ |
| 1 CHAT | Shell→Assets/ChatSystem、TIM_QM | 全体/DM、グループ招待/承諾/辞退、お気に入り/既読/ミュート、名前/アイコン問い合わせ | 全イベント/変数契約、再入室、宛先切替、複数人。同期本文は秘匿DMではない |
| 2 INVENTORY | InventoryModule→InventoryManager | 所持品/カテゴリ/ソート/保管/取り出し/売却/削除/メモ | x0除外、容量/重量、復元、実物の所有権と枯渇 |
| 3 EQUIPMENT | Shell、EquipmentPage→Inventory/Status | 17枠・所持候補・ToggleEquipment、HP/MP/STA/O2/攻防/EXP/重量メーター | 消耗/売却/削除時の装備解除、全補正復元、衣装変更とは区別 |
| 4 SETTINGS | Shell、SettingsPage→AudioSource/Swim/Flying | 音量適用、12テーマ/RGB、PlayerData、移動切替 | 音源の実参照、乗車中の入力競合、保存/初期化範囲 |
| 5 MAP | MapPage→WIM TeleportModule/Target | 目的地列挙・CanUseTarget・TeleportTo | inactive/EditorOnly依存、権限、overlay必須参照。現状は地図地形/探索記録ではなく移動先UI |
| 6 SHOP | ShopPage/Shell→InventoryModule/通貨 | sceneProducts/カテゴリ/購入数、枠拡張、通常通貨/GameChips、交換 | 失敗時の残高と在庫不変、連打、PlayerData未復元 |
| 7 SPECIAL | Shell.specialActionTargets/events | 7サブページ、未接続無効、接続イベントへ委譲 | 装置ID・権限・busy・成功/失敗の戻り。接続済み表示だけでは実行成功にならない |
| 8 CRAFT | CraftPage/Shell→InventoryManager | 組立/合成/調合/分解/修繕/鍛造/料理、素材/数量/副産物、検証後まとめてcommit | 同素材重複、出力が素材にもなる、容量/重量、個体品質、処理内容が名前だけになっていないか |

旧N_MenuIntegration.md/READMEは過去の記録。8装備枠・チャット未接続/クラフト対象外等の記述を現行仕様に採用しない。現行コードであることとSceneの割当/実操作成功も区別する。

## 入力/状態遷移
Desktop/VR入力 → Pointerのhover/press/release → 種別Button/Slider/Scrollbar/Input/Toggle/Scroll/Grab/Resize/Dock/Title → 対応FollowerまたはeventTargets/eventNames → Shell → ドメイン → 通知/表示/保存。
- SDK GraphicRaycasterの通常イベントではなく独自analytic pointer。VRCUiShape=0はこの設計の限定検証結果。
- Desktop: Tab/ShiftTab、相対マウスと固定中の中央照準、Grab/Resize/Dock、U/I/O/J/K/L回転、二重tap等。VR: controller InputUse、stick/trigger、指接触、hand追跡。
- 非表示→召喚→追従/固定→drag/resize→解除→収納、単click/長押し/二重tap、文字入力focus、clip外移動、窓間移動を別ケースにする。
- MainのみControlBar/Dock追加、独立窓から無制限生成しない。複数窓の表示選択は独立、在庫/通貨/権限は共有する正本を参照。
- 再生成やコントロール追加後はpointer配列/イベント表を更新。旧UnityEvent経路と独自dispatchの二重実行、閉じた窓のfocus残留、テキスト入力中の移動キー処理が検証対象。

## 重点課題（原因候補/未完了であり、発生確認済みバグとは限らない）
1. MAPの受信側が旧WIMのinactive/EditorOnly配下ならStart/実行/ビルドで破綻し得る。現Sceneの実参照を追う。
2. FarmerのPlantSeedByIndex/ApplyFertilizer内にはInventory消費がない。種/肥料/水の消費を装置側transactionで接続する設計が必要。
3. Farmer収穫は既存harvestVariantsを移動して再利用。収穫後の保管/再収穫/同時操作/在庫容量、個体形質の保持を確認する。
4. Inventory保存はitemIdと数量/装備IDが主体。Farmerの味/品質等を同一itemIdにまとめると個体差が失われる可能性。ロット単位か品質別IDかを決める。
5. ローカル永続在庫と共有実物のstore/withdrawは別責務。同期の所有権、二人の同時格納/取出、再入室と実物不足を検証する。
6. SPECIALは汎用イベントのみ。車両/昇降機/電源/音声/端末等の結果・権限・クールダウンを受信側が担う橋渡しが不足。
7. PlayerData ready前と装置busy/未接続/権限拒否を別表示にする。UIボタンの無効化だけを安全性の根拠にしない。
8. NWIMChatModule旧経路はSendChat1/2の後に無条件でSentを表示。現行Shellの経路と混在させず、実際の成功判定を接続する。
9. Prefab検証器は旧15品/プレビュー仕様や未接続action前提を含む。現行Sceneの受入試験を代替しない。
10. finite電力/燃料/冷蔵保存/物語ラジオ/狩猟/釣り専用ドメインは今回のN.Script対象解析では実体未確定。新規仕様として先に必要性を決める。

## 根拠となるローカルソース
- Assets/N.Assets/N.Script/N.MainMenu/{NMainMenuFollower,NIntegratedMenuPointer}.cs
- Assets/N.Assets/N.Script/N.WIMExtensions/NWIMMenuShell.cs (Start、HasAction、ExecuteSelectedAction、ApplyAudioSettings、各Chat橋渡し)
- Assets/N.Assets/N.Script/N.WIMExtensions/{NWIMInventoryModule,NWIMEquipmentPage,NWIMCraftPage,NWIMMapPage,NWIMShopPage,NWIMSettingsPage}.cs
- Assets/N.Assets/N.Script/N.Inventory/NInventoryManager.cs (CraftItem/CanCraftItem、StoreWorldItem/WithdrawWorldItem、PlayerData)
- Assets/N.Assets/N.Script/N.FarmerSimulation/Runtime/NFarmerSimulationPlot.cs
- Packages/dev.yukineko.wim.modules-vol2/Runtime/Teleport/TeleportModule.cs
- Assets/ChatSystem/Scripts/ChatSystem.cs、Assets/N.Assets/Editor/N.WIMExtensions/NIntegratedMenuOptimizer.cs
GitHubには第三者コードやScene全体を転載していない。ソース所在/観測結果を文書として記録する。
