# N.Assets 全種解析
2026-10-12。ソースの静的解析。Unity操作・コード変更・コンパイル・実機試験は行っていない。

## 対象と証拠
対象は実在する Assets/N.Assets。C#217件（Runtime102、Editor96、Dependency19）、34分類。asmdef60、Prefab47、Shader11、Markdown44。
[全C#索引](n-assets-script-index.md)、[関連アセット索引](n-assets-asset-index.md)、[SHA256](n-assets-source-hashes.json)、[全系統の役割](n-gimmick-catalog.md)。
全C#を読取して宣言・参照・同期・保存・コールバックを抽出。意味解析は中核と周辺系統の担当・接続経路を確認した範囲。全217ファイルの全メソッドの動作保証ではない。
Prefab索引はN.Assets内C# GUIDの直接参照のみ。外部スクリプト・Program Asset経由の解決やScene配線の検証ではない。Shaderは構造抽出のみで描画互換性未検証。
再抽出: Documentation/N.WorldProjects/tools/Analyze-NAssets.ps1（読取のみ）。34分類のファイル数は次表。

| 系統 | C#数 |
|---|---|
| N.AdvancedWorldSettings | 2 |
| N.AvatarNow | 31 |
| N.BoothPoster | 18 |
| N.Border | 6 |
| N.CalibrationSystem | 2 |
| N.CocktailLiquidSystem | 2 |
| N.Console | 3 |
| N.DebugVisualization | 5 |
| N.DoorSystem | 9 |
| N.DriftCorrection | 2 |
| N.DynamicObject | 11 |
| N.DynamicYamaPlayer | 3 |
| N.ElevatorSystem | 7 |
| N.FarmerSimulation | 3 |
| N.FlyingSystem | 3 |
| N.GimmickTransformationSystem | 12 |
| N.Inspector | 3 |
| N.Inventory | 10 |
| N.MainMenu | 2 |
| N.MixedDrinksSystem | 4 |
| N.MovementSystem | 3 |
| N.PetSimulator | 2 |
| N.SecuritySystem | 8 |
| N.StatusSystem | 3 |
| N.SwimSystem | 3 |
| N.TouchPanelUI | 3 |
| N.UdonChipsExchangeSystem | 4 |
| N.UdonGameChips | 3 |
| N.VehicleManager | 11 |
| N.VirtualInput | 8 |
| N.WaterRippleSystem | 4 |
| N.WeaponsManager | 4 |
| N.WelcomeSystem | 2 |
| N.WIMExtensions | 21 |

## 接続上の重要事項
- N.MainMenuとWIMExtensionsは表示・要求側。Inventory/Status/通貨/共有装置を正本にし、UI側に処理を複製しない。
- Inventoryのローカル保存とDynamicObjectの共有実物は別。二重格納、所有者交代、再入室、個体品質とitemIdの統合を検証する。
- Farmerの種・肥料とInventory消費は橋渡しが必要。収穫成功時の一回commit、失敗時の非消費、個体品質の保持方式を決める。
- Movement外部overrideをVehicle/Swim/Flyingが使う。優先順位・終了/退出/水域境界での復元を統一する。
- WeaponsManagerはStatus参照だけで攻撃補正統合済みとは言えない。GetDamageの計算と、GimmickTransformation側WorldWeapon/WorldDamageReceiverの独立経路を統合設計する。
- WaterRippleは水面・接触・浮力で、魚AIや釣果管理ではない。波紋はローカル、浮力PickupはOwner主体。DynamicObjectとの物理writer競合を確認する。
- MixedDrinksのruntimeはingredientRoot/recipeRoot/recipeDropdownの参照保持とgetter。飲料制作・消費・Status効果は実装済みと扱わない。
- CocktailLiquidBridgeはCocktailSystem.src.CocktailInfoからMyxy.Glass.Udon.Glassへの液量/色/粘度bridge。別購入珈琲アセットとの互換は未確認。
- Shared InspectorはEditor専用。Runtimeギミックとは分けて索引に含めた。既存参照を保ち、不足参照だけ補完する規約を維持。

## 12層・シームレス設計との齟齬
NElevatorHotelSetupには2基・12階・52ボタンを前提とする検査とRealモード設定が既にある。ただし今回実行しておらず、実Sceneが同設定かは未確認。
NElevatorSystemのReal移動にも乗客追従用TeleportToがある（MoveRealCabin）。別エリアへのワープとは異なるが、乗車中歩行/VR姿勢/複数人/Owner退出を検証する。Runtime既定floorCount=2を実Sceneの12階構成と混同しない。
NWIMMapPage/Shellの通常MAPはTeleportModule/TeleportTarget依存。今回の方針では位置・探索済み情報・物理経路案内を先に設計し、通常ワープを完成条件から外す。
Doorのteleport経路は通常導線と分離。Securityの救出TeleportToは安全機能なので、通常移動禁止を理由に一括削除しない。
[最新配置・接続案](../design/seamless-world-layout.md)。

## 次工程
1. 既存12層のScene参照・座標・歩行/エレベーター経路を読取確認。
2. MainMenu/MAPをシームレス導線に合わせ、Floor/Areaの表示契約を決める。
3. 購入アセットを1種類ずつ、原本保持→接続adapter→保存/共有の受入試験。
4. 資源→制作→実物→所持/装備→効果の一連動作を検証。
5. 描画、Udon更新、同期、メモリを別々に測定。以前のConsole error=0を今回の実動作検証として流用しない。
