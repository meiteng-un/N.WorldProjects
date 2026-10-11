# 現在展開中のワールドScene: 全ヒエラルキー解析
2026-10-12。現在Sceneは Assets/N.Assets/N.Scene/N.Worlds Project -001.unity。以前解析したN.GimmickTest_002とは別のScene。
最初の軽量概要は46797ノード/active10195、今回全取得したJSONは46850ノード/active10248。差53は観測値の差として記録し、原因未確認。全索引と本レポートの集計基準は後者で統一する。
Sceneは取得開始時からdirty=true。保存/ロード/再配置/削除/コンパイル/PlayModeを実行していない。

## 解析範囲と取得経路
UnityのGetSceneInfoが実Sceneの全rootから子を再帰取得した結果を全走査。通信応答が滞ったため、同じ呼出しのUnity Editor.logにあるSUCCESS JSONを抽出して解析した。未保存Sceneをディスク上のunityファイルで代用していない。重い全取得の再実行はしていない。
取得JSONのstatistics.total_gameobjects=46850と走査件数が一致、components=133312、ルート10、最大深度64。
各ノードの名前/親子/activeInHierarchy/tag/layer/world座標/全コンポーネント型を索引化。
[枝・全型・N系配置索引](scene-structure-index-2026-10-12.md)。全46850行の親キー付きTSVはローカル Documentation/N.WorldProjects/docs/systems/scene-hierarchy-2026-10-12.tsv に保存（GitHubは要約索引のみ）。
975個の名前パスに重複があるため、名前パスだけで操作対象を一意に決めない。TSVのkeyは取得時の兄弟番号で永続IDではない。
Prefab元/serialized reference/Udon public variable/UnityEvent/Component.enabled/Collider境界/通行可能性/同期動作は全数検証していない。Missing Scriptは取得関数がnullを省略するため、この結果からゼロとは判断できない。

## 全ルートの役割と規模
総数/active/EditorOnlyは子孫を含む。EditorOnly列は祖先タグを含み、activeと排他的ではない。

| ルート | 総数 | active | EditorOnly | 構造上の担当 |
|---|---:|---:|---:|---|
| VRChat World Info | 177 | 171 | 5 | Descriptor、初期設定、環境、N.Systems、EventSystem/通貨 |
| Unity-RecorderBindings | 1 | 1 | 1 | Editor専用記録補助 |
| World Layers | 32903 | 9664 | 18980 | ホテルと探索領域 |
| Extra Assets | 2205 | 411 | 686 | 天候、TIM_QM、会話、カード/Wallet、旧WIM |
| Experimental | 62 | 0 | 62 | 防音/マイク/音声チャンネル試験品 |
| -----OldExtra_Assets----- | 6164 | 0 | 6164 | 釣り/船/車/ペン/料理等の旧・待機品 |
| GARAGE | 104 | 0 | 104 | 保管された倉庫/ガレージ素材 |
| nadena.dev.ndmf__Activator | 1 | 1 | 0 | ビルド補助。削除適否は未判断 |
| N.Console | 112 | 0 | 112 | コンソール待機品。9F稼働済みではない |
| Experimentals_Weapons | 5121 | 0 | 5121 | 武器試験品。8F格納/ゲーム武器化済みではない |

## 建物と計画との差
World Layers/N.Luminous Hotelは32901ノード、active9662。
Rooftop、Floor_9、8、6、5、4、3、2、1、Basement_1と全11階間枝は取得時に非activeかつEditorOnly祖先配下。階の名前やモデルが存在しても全12層が通常プレイで有効とは言えない。
Floor_7は12220ノード/active6736、Basement_2は3107/active2467で主要な有効区画。

| 階/枝 | 総数 | active | 具体的構造 |
|---|---:|---:|---|
| Rooftop | 7010 | 0 | StairArea、AbstractEcho（6663）。R用途の完成は未検証 |
| Floor_9 | 484 | 0 | 主にStairArea。管理室として完成とは言えない |
| Floor_8 | 483 | 0 | StairArea中心。倉庫内容・出入庫未確認 |
| Floor_7 | 12220 | 6736 | EntranceArea、RestSpace、SmokingSpace、StairArea、PrivateRooms |
| Floor_6〜2 | 各485 | 0 | StairArea中心。6F住居・商業区画は配置計画と別 |
| Floor_1 | 5255 | 0 | Architecture、Environment、OcclusionCulling、旧Elevator_Root、UdonObject_Dcut |
| Basement_1 | 485 | 0 | StairArea中心。機械/進行イベント未確定 |
| Basement_2 | 3107 | 2467 | StairAreaが2枝、LuminousOasis_Common、EntranceHall、PoolArea、LoungeArea、Sauna |
| N.Exploration Area（末尾空白あり） | 1 | 1 | 子なし。探索フィールドの親だけで、LostMetropolis配置は確認できない |

7F PrivateRoom_701は3683/active2472、702は2477/active1304。701にはSamenoLatteArtSet/EspressoMachineが有効配置、7F入口にはF_Aquarium_Tankが有効配置。
WelcomeBoard_701/702はホテル共通枝に配置。FloorGuidesは7F用枝が存在。
B2には有効なTeleportSystemがあり、701には有効なNDoorTeleportInputが2個。シームレス構想との整合を確認する必要があるが、配置だけで実際のワープ発生を断定しない。

## エレベーター
共通Elevatorsは724ノード/active281。A/Bキャビン、A/Bの階座標枝、NElevatorSystem1個、NElevatorButton全52個（active30、EditorOnly祖先含む22）。
階座標AでR=Y21、9F14、8F7、7F0、6F−7、5F−14、4F−21、3F−28、2F−35、1F−42、B1−49、B2−56。これは座標マーカー値であって床面・歩行路の実測ではない。
A/Bの7F以外の階座標はEditorOnly祖先配下。参照が必要なマーカーをビルド除外してよいか、serialized参照とビルド後データで確認する課題。
現SceneのfloorCount/mode配列/参照を取得確認できていないので、ソースのRealモード設定手順を現Scene実設定と扱わない。
旧Floor_1のElevatorState系は非active/EditorOnly。新旧どちらが正本か、build時の共存を確認する。

## N系の配置状況
VRChat World Info/N.SystemsにBorder、Door、Swim、Flying、Status、Security、Inventory、Movement、Authority、DynamicObject、通貨交換、WeaponsのManagerが配置されている。
VirtualInput/DebugVisualizationは非activeかつEditorOnly。BoothPosterは非activeだがEditorOnly祖先ではない。AvatarNowは7Fでactive。
NDynamicObjectは全84/active10。全84がゲーム内で稼働しているわけではない。
NMainMenuFollower/NWIMMenuShellとN.IntegratedMenu名は全階層索引に見当たらない。旧WorldIntegratedMenuは非activeかつEditorOnlyで、NWIMChatModule/InventoryModuleはその配下。このSceneに統合メニューの完成形が導入済みとは言えない。
Farmer/Petの該当コンポーネントも索引で未検出。前回の全ソース一覧をScene導入済み一覧として扱わない。
FishingRodはOldExtraのFishingRodDarkで非active/EditorOnly。魚を釣ってInventoryへ保存する現導線は未確認。
N.Console、NDynamicYamaPlayerManager、旧GameChipsも保管枝。管理・動画・通貨の同名/旧版参照を後の橋渡しで確認する。

## 規模と検証候補
EditorOnly祖先含む31235ノード（うちactive617）。単純な非表示とビルド除外を分け、他のManagerが除外対象を参照していないか検査する。
MeshRenderer16426（activeオブジェクト上4128）、Light2762（同798）、Canvas632（同169）、AudioSource610（同212）、UdonBehaviour3334（同841）。
LightのComponent.enabled/typeは全数未確認で、軽量概要のLight689と型集計2762は集計条件が異なる。これらはdraw call/更新実行数/実時間を意味しない。
EventSystem全3のうちactiveオブジェクト上1。直ちに多重EventSystem問題とは判断しない。
AudioListener全4のうちTIM_QMとIMEChatのPlayerScaleに2個がactiveオブジェクト上にある。enabled/初期化時制御が未確認なので二重有効と断定せず確認候補にする。
カメラ/ライト/Canvas等はComponent.enabled、EditorOnlyとruntime表示切替を確認した後にProfilerで評価する。

## 次の確認順（提案）
1. このSceneを正式対象として、統合メニューをテストSceneからどう持ち込むかを決める。今は未移植。
2. エレベーターの階座標参照とEditorOnly除外、12層の稼働範囲を読取検証。
3. 7F/B2の扉・テレポート・水泳・Authorityの既存機能を、連続導線に合わせて接続設計。
4. 保存/待機品から釣り等を選定し、Inventory/Status/共有実物へ最小adapterで橋渡し。
5. R/他階/探索フィールドを段階的に実装。EditorOnlyを全解除したり保管品を一括有効化しない。
本レポートは構造把握。コンパイル、Missing Reference、保存、PlayMode、VR/Desktop、複数人、性能合格の証拠ではない。
