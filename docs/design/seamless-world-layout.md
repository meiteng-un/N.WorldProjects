# 最新ワールド構成: 12層＋探索フィールド
2026-10-12。ユーザー確定条件と、未実装の設計提案を分ける。

## 確定条件
地下B2/B1、地上F1〜F9、屋上Rの計12層。探索用フィールドを加える。通常移動は別エリアへのテレポートではなく、連続した空間を歩行等で移動する疑似オープンワールド。
モデル数は少なめ。購入済みBOOTHの釣り・育成・水槽魚挙動・珈琲等を改造/改良して組み込む。階ごとの用途、階高、探索距離、PC/Android対象は未確定。世界観原文の旧階数よりこの条件を優先する。

## 提案する最小構成
一つの連続座標空間に建物と探索フィールドを配置。Floor/Areaは表示・権限・更新頻度の論理ゾーンであってワープ先ではない。
階段/歩行路/実移動エレベーターで接続。フロア表示と権限は同じArea/Floor識別契約を使うが、描画制御とアクセス権判定は分離する。
MAPは現在地・探索済み地点・利用可能な物理ルートを表示。未知エリアを無条件に公開せず、通常テレポートボタンを基本導線にしない。
遠方のローカル演出は距離に応じて更新頻度を下げる候補。共有状態、Owner処理、衝突床を無条件に停止しない。停止/再開時の状態引継ぎを決めてから適用する。
長い配列の毎フレーム走査を避け、分割更新・参照キャッシュを使う方針は[UdonSharp公式性能ガイド](https://creators.vrchat.com/worlds/udon/udonsharp/performance-tips/)に沿う。
室内はOcclusion Cullingの候補だがCPU/メモリのコストもある。描画削減とアセットのメモリ解放は別であり、シーンストリーミング実装済みとは扱わない。[Unity 2022.3公式](https://docs.unity3d.com/ja/2022.3/Manual/OcclusionCulling.html)

## 購入アセットの受入分類
以下はローカルで見つかった候補パス。購入商品名・バージョン・ライセンス・実Scene採用品の照合はまだ行っていない。

| 用途 | 候補 | N系接続先 | 先に決める契約 |
|---|---|---|---|
| 釣り | Assets/FishingRod/Sources | Inventory、DynamicObject、Status、Swim | 釣果ID/個体情報、一回取得、共有竿Owner、取消 |
| 水槽・魚群 | Assets/FUKA/F_Aquarium/Scripts | 釣果/Inventory、Area、WaterRippleは必要時のみ | 展示魚の正本、投入/回収、ローカル演出と共有個体の区別 |
| 珈琲 | Assets/SamenoLab/VRCLatteArt/Scripts | Inventory、通貨、Status、液体bridge | 材料消費、制作完了、飲用効果、容器Owner |
| 育成 | N.FarmerSimulation / N.PetSimulator、他購入品は未特定 | Inventory、DynamicObject、Status | 成長時間、品質/ロット、再入室、共有/個人区分 |
| 液体表示 | Assets/myxyLiquidGlass、N.CocktailLiquidSystem | CocktailInfo、飲料容器 | 液量単位、型、所有権、満杯/空の結果 |

原本を直接大量改造せず、許諾・変更点を記録しN側adapterで可能な部分を接続。必要な改造は商品規約を確認してから実施。購入コードやモデルはGitHub資料へ転載しない。
魚群/釣り/珈琲とN系の併存は、ファイル存在だけでは実動作互換性を保証しない。

## 優先順と受入
- P0: 保存Sceneの12層、床/階段/出入口、エレベーターReal設定と参照を確認。今回はScene未変更。
- P0: MAPのワープ依存を見直す。Doorの物理経路、Border/Security権限を連続通路で検証。
- P1: 釣り→取得→所持→水槽投入/回収の一本を先に完成。
- P1: 育成→収穫→制作/珈琲→飲用/効果→保存を接続。
- P2: 遠方演出/魚群/水面/UIの測定後に調整。モデル増加より導線と既存ギミックの成立を優先。

歩行でB2〜Rとフィールド往復、VR/Desktop、乗車中歩行、二人同時操作、Owner退出、再入室復元、ゾーン境界往復、PlayMode reset/debugを個別に確認する。
安全救出/初期spawnと通常移動は別規則。エレベーター乗客追従の内部TeleportTo許容は体感試験後に判断し、無断で安全機能を消さない。
