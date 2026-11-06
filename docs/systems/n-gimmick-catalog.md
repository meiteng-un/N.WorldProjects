# N系ギミック群: 役割・関連性・互換性

> 全種調査追記: [全種解析](n-assets-analysis-2026-10-12.md)、[全217C#索引](n-assets-script-index.md)、[60 asmdef/47 Prefab/11 Shader等](n-assets-asset-index.md)。Editor専用N.Inspectorを含め34分類。以下の初期概要は、この追記と全種解析を優先して読む。
2026-10-12 初期カタログ。対象はAssets/N.Assets/N.Script配下の分類と、メニューから直接使う既知の外部配置品。
「主要コード確認」は参照/API/処理を対象確認したもの。「概要」はファイル/宣言/設定からの初期分類であり全実装解析済みではない。いずれも実機互換性保証ではない。

## 中核（主要コード確認）
| 分類/主担当 | 役割 | 関連・互換性 |
|---|---|---|
| N.MainMenu / Follower・Pointer | ローカル統合窓、開閉、追従、固定、Dock、入力 | Shellと独自イベント表。GraphicRaycasterとの二重入力を避ける |
| N.WIMExtensions / Shell・InventoryModule・各Page | 9画面、取引UI、Chat/Map/設定連携 | N.Inventory等を正本として使う。旧Bool在庫経路と数量経路の自動移行はない |
| N.Inventory / Manager・Inserter・WithdrawButton | itemId数量、所持枠/重量、装備17枠、制作、永続保存 | DynamicObject、PlayerData、changeListeners→UI/Status。共有実物とローカル在庫の整合が要検証 |
| N.DynamicObject / Object・Manager・SnapPoint・PaymentTerminal | item定義、実物Pickup/同期/格納/取り出し、接続/装備/bonus | Inventory、Status、Security、通貨、物理。個体メタデータの在庫への引継ぎは要設計 |
| N.StatusSystem | HP/MP/STA/O2、攻防、EXP、状態異常/補正 | Inventory装備/所持補正、DynamicObject、Movement、Weapons。44補正対象と単純4補正を混同しない |
| N.UdonGameChips / N.UdonChipsExchangeSystem | ゲーム通貨、通常UdonChipsとの交換 | Shop/Inventory/Console。DataReady前の操作、失敗rollbackを検証 |
| N.MovementSystem | 移動速度/走行/ジャンプ/足音・補正 | Status、Swim/Flying、Vehicle外部移動override。速度設定の多重writerを避ける |
| N.VehicleManager / VehicleSystem・各車種 | 車両操縦の排他、車/船/航空等の分類 | 操縦開始でSwim/Flyingを抑制しMovement override取得、終了時復元。召喚UIは別橋渡し |
| N.WeaponsManager / WeaponState | 使用・弾/リロード/安全装置/効果 | Status、変換武器系との担当重複を整理。物語の武器設定と実装完成は別 |
| N.ElevatorSystem / System・Button | 階呼出/目的階/扉/停止/保守 | 権限、入力。有限電力の接続は未確定、privileged引数をUIだけで決めない |
| N.FarmerSimulation / Plot・CropTraits | 成長/水/肥料/収穫/味・品質 | DynamicObject収穫品。Inventory資源消費/ロット保持/料理recipeへの橋渡しが必要 |
| N.PetSimulator / Agent | owner主体の徘徊/待機/休憩、好感度 | Animator・共有状態。家畜生産/戦闘AI/群れの実装とは断定しない |
| N.SecuritySystem / System・Zone・ObjectGuard | ゾーン/実物操作の権限制御 | Authority、DynamicObject。未知権限時fail-closed、表示と受信側検証を分離 |

## 周辺（概要/関連宣言の初期分類）
| 分類 | 役割の初期分類 | 主な橋渡し/確認項目 |
|---|---|---|
| N.AdvancedWorldSettings | プレイヤー/ワールド初期設定 | Movement/Status等の設定上書き順 |
| N.AvatarNow | アバター選択/表示・取得UI | 任意補助。装備ステータスと衣装変更を区別 |
| N.BoothPoster | BOOTHアイテム/URLポスター | URL取得/信頼設定、経済UIとは別 |
| N.Border | 境界とgroup制御 | Authority/接触入力、境界と扉の役割を分離 |
| N.CalibrationSystem | MMD/モデル基準位置・向き・高さ校正 | animatedRoot等。メニュー入力校正とは別 |
| N.DriftCorrection | 入力軸の中立値/deadzone/平滑化・ドリフト補正 | 対象と入力源を確認、実デバイス検証未了 |
| N.CocktailLiquidSystem | CocktailInfoから液体表現へのbridge | 元Cocktail系と混合飲料系の型/効果整合 |
| N.MixedDrinksSystem | 混合飲料系（クラス存在確認） | runtimeはingredientRoot/recipeRoot/recipeDropdown参照とgetter。制作・消費・効果の橋渡しは未完成 |
| N.Console | コマンド、権限ログイン、通貨/ギミック拡張 | 管理者用。ユーザー向けSPECIALと権限分離 |
| N.DebugVisualization | Collider/Contact/Audio/Light等可視化 | PlayMode/debug限定と権限、通常描画負荷 |
| N.DoorSystem | 物理/teleport扉、handle/PhysBone、カード/認証 | Authority、Welcome identity。VR/Desktop別経路 |
| N.DynamicYamaPlayer | 動画player pool・配置/音量/privacy preset | 動画システム。物語ラジオそのものとは別 |
| N.FlyingSystem | ローカル飛行 | Movement/Vehicle、設定UI、world設定 |
| N.SwimSystem | ローカル水泳 | Movement/Vehicle/Status、境界と復元 |
| N.GimmickTransformationSystem | Animator/Contact/PhysBone操作、武器/ダメージbridge | Weapons/Statusとダメージ正本の重複確認 |
| N.TouchPanelUI | 接触UIボタン | 独自Pointerと同時処理しない、VRの二重入力検査 |
| N.VirtualInput | Contact/PhysBone・ジェスチャー/スワイプ推定 | Pointer/Followerとの入力優先とfocus |
| N.WaterRippleSystem | 水面波紋/浮力Pickup | Swim、物理/共有Owner、PC/Android描画 |
| N.WelcomeSystem | WelcomeとIdentity Card bridge | Authority/Doorのidentity発行・登録と接続 |

## Editor共通基盤
N.Inspector（3ファイル）はInspector Base/SceneCache/Validation。Runtimeではなく設定・参照補完・検証担当。

## N.Script外にある関連品
- N.AuthorityLevelManager: QuickBrown/LuminousHotel/Room702_SimpleRoom/.../RoomOwner/SCRIPT下。ShellはconsoleLookupUserName→ResolveConsoleAuthorityLevel→consoleResolvedAuthorityLevelの契約を利用。用途ごとのManager/roomを参照で特定する。
- Assets/ChatSystem: Shellから全体/DM/グループ会話へ。同期文字列本文とrecipientsはUI絞込みであり暗号化ではない。
- TIM_QM: ShellのQueryWIMPlayerPresentationと名前/tag/icon表示契約。
- WorldIntegratedMenu + Modules Vol2: TeleportModule/TeleportTarget/ModuleMetadataの権限・移動。旧ルートinactive/EditorOnlyのまま依存を残せるか確認する。
- WeatherAndSolarSystem: NWIMWeatherModuleがWeatherSystem callbackと現在/予報を表示。独立した9ページ内の接続先/配置は未確認。
- UdonChips: 通常通貨側。GameChipsと同じ残高として扱わない。

## 互換性の共通契約
1. コアは既存UdonSharpとNInspectorの規約を維持。第三者パッケージの更新/移動は行わない。
2. UIはローカル、共有実物はOwner/同期、永続データはプレイヤー単位。いずれか一つの成功を他の成功とみなさない。
3. itemId/recipe ID/装置ID/authority selectorは参照Managerから解決。SceneやPrefabを跨ぐ暗黙の名前検索だけに依存しない。
4. UI→receiverに必要データを渡し、receiverでready/permission/busy/capacity/ownershipを検証。成功/失敗/理由をUIへ戻す。
5. UIはchange通知で更新し、窓ごとに在庫/決済ロジックを複製しない。
6. Legacy Inventory保存からの移行、17枠装備、農作物個体品質などの変更はversion化と旧保存fallbackを先に決める。
7. VR/Desktop、複数ユーザー、PC/Android、再入室/Owner退出、Prefab/Scene保存はそれぞれ別の互換性試験。


