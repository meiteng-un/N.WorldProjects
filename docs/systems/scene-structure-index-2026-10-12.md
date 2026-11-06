# 現行Scene構造索引
2026-10-12。N.Worlds Project -001の取得結果46850ノードを全走査。activeはGameObject.activeInHierarchyでありComponent.enabledではない。EditorOnlyは祖先を含むタグからの除外候補で、最終ビルド結果ではない。keyはスナップショット内の兄弟番号による識別子。

## 深さ3までの全枝
| key | パス | 子孫含む総数 | active数 | EditorOnly祖先含む数 |
|---|---|---|---|---|
| /0 | VRChat World Info | 177 | 171 | 5 |
| /0/0 | VRChat World Info/Main Camera | 1 | 1 | 0 |
| /0/1 | VRChat World Info/Environment | 8 | 8 | 0 |
| /0/1/0 | VRChat World Info/Environment/Directional Lights | 4 | 4 | 0 |
| /0/1/0/0 | VRChat World Info/Environment/Directional Lights/Directional Light_ForFog | 1 | 1 | 0 |
| /0/1/0/1 | VRChat World Info/Environment/Directional Lights/Directional Light_Pickup | 1 | 1 | 0 |
| /0/1/0/2 | VRChat World Info/Environment/Directional Lights/Directional Light_Avatar | 1 | 1 | 0 |
| /0/1/1 | VRChat World Info/Environment/Post-process Volumes | 3 | 3 | 0 |
| /0/1/1/0 | VRChat World Info/Environment/Post-process Volumes/Post-process Volume_ColorGrading | 1 | 1 | 0 |
| /0/1/1/1 | VRChat World Info/Environment/Post-process Volumes/Post-process Volume_Bloom | 1 | 1 | 0 |
| /0/2 | VRChat World Info/N.Systems | 33 | 27 | 5 |
| /0/2/0 | VRChat World Info/N.Systems/N.Borders | 6 | 5 | 0 |
| /0/2/0/0 | VRChat World Info/N.Systems/N.Borders/N.Border_01 | 1 | 1 | 0 |
| /0/2/0/1 | VRChat World Info/N.Systems/N.Borders/N.Border_02 | 1 | 1 | 0 |
| /0/2/0/2 | VRChat World Info/N.Systems/N.Borders/N.Border_03 | 1 | 0 | 0 |
| /0/2/0/3 | VRChat World Info/N.Systems/N.Borders/N.Border_04 | 1 | 1 | 0 |
| /0/2/0/4 | VRChat World Info/N.Systems/N.Borders/N.Border_05 | 1 | 1 | 0 |
| /0/2/1 | VRChat World Info/N.Systems/N.VirtualInput | 4 | 0 | 4 |
| /0/2/1/0 | VRChat World Info/N.Systems/N.VirtualInput/MenuAnchor | 3 | 0 | 3 |
| /0/2/2 | VRChat World Info/N.Systems/N.DoorSystem | 1 | 1 | 0 |
| /0/2/3 | VRChat World Info/N.Systems/N.AreaCullinger | 5 | 5 | 0 |
| /0/2/3/0 | VRChat World Info/N.Systems/N.AreaCullinger/AreaCullinger_Pool | 1 | 1 | 0 |
| /0/2/3/1 | VRChat World Info/N.Systems/N.AreaCullinger/AreaCullinger_Hotel_FullPack | 1 | 1 | 0 |
| /0/2/3/2 | VRChat World Info/N.Systems/N.AreaCullinger/AreaCullinger_Hotel_701 | 1 | 1 | 0 |
| /0/2/3/3 | VRChat World Info/N.Systems/N.AreaCullinger/AreaCullinger_Hotel_702 | 1 | 1 | 0 |
| /0/2/4 | VRChat World Info/N.Systems/N.SwimSystem | 1 | 1 | 0 |
| /0/2/5 | VRChat World Info/N.Systems/N.FlyingSystem | 1 | 1 | 0 |
| /0/2/6 | VRChat World Info/N.Systems/N.StatusSystem | 1 | 1 | 0 |
| /0/2/7 | VRChat World Info/N.Systems/N.SecuritySystem | 5 | 5 | 0 |
| /0/2/7/0 | VRChat World Info/N.Systems/N.SecuritySystem/N.SecurityZones | 2 | 2 | 0 |
| /0/2/7/1 | VRChat World Info/N.Systems/N.SecuritySystem/N.SecurityObject Guarders | 2 | 2 | 0 |
| /0/2/8 | VRChat World Info/N.Systems/N.InventorySystem | 1 | 1 | 0 |
| /0/2/9 | VRChat World Info/N.Systems/N.MovementSystem | 1 | 1 | 0 |
| /0/2/10 | VRChat World Info/N.Systems/N.DebugVisualization | 1 | 0 | 1 |
| /0/2/11 | VRChat World Info/N.Systems/N.Authority Level_Manager | 1 | 1 | 0 |
| /0/2/12 | VRChat World Info/N.Systems/N.Dynamic Object_Manager | 1 | 1 | 0 |
| /0/2/13 | VRChat World Info/N.Systems/N.UdonChipsExchangeSystem | 2 | 2 | 0 |
| /0/2/13/0 | VRChat World Info/N.Systems/N.UdonChipsExchangeSystem/N.ChipsExchangeButtonManager | 1 | 1 | 0 |
| /0/2/14 | VRChat World Info/N.Systems/N.Weapons_Manager | 1 | 1 | 0 |
| /0/3 | VRChat World Info/EventSystem | 134 | 134 | 0 |
| /0/3/0 | VRChat World Info/EventSystem/SwitchSyncers | 4 | 4 | 0 |
| /0/3/0/0 | VRChat World Info/EventSystem/SwitchSyncers/SwitchSyncer_Collider | 1 | 1 | 0 |
| /0/3/0/1 | VRChat World Info/EventSystem/SwitchSyncers/SwitchSyncer_LowMode | 1 | 1 | 0 |
| /0/3/0/2 | VRChat World Info/EventSystem/SwitchSyncers/SwitchSyncer_MirrorMode | 1 | 1 | 0 |
| /0/3/1 | VRChat World Info/EventSystem/Light Volumes | 84 | 84 | 0 |
| /0/3/1/0 | VRChat World Info/EventSystem/Light Volumes/Light Volume Manager | 2 | 2 | 0 |
| /0/3/1/1 | VRChat World Info/EventSystem/Light Volumes/LuminousOasis | 77 | 77 | 0 |
| /0/3/1/2 | VRChat World Info/EventSystem/Light Volumes/LuminousHotel | 4 | 4 | 0 |
| /0/3/2 | VRChat World Info/EventSystem/SpawnPoint | 3 | 3 | 0 |
| /0/3/2/0 | VRChat World Info/EventSystem/SpawnPoint/SpawnPoint_01 | 1 | 1 | 0 |
| /0/3/2/1 | VRChat World Info/EventSystem/SpawnPoint/SpawnPoint_02 | 1 | 1 | 0 |
| /0/3/3 | VRChat World Info/EventSystem/Occluder | 34 | 34 | 0 |
| /0/3/3/0 | VRChat World Info/EventSystem/Occluder/Rooftop | 2 | 2 | 0 |
| /0/3/3/1 | VRChat World Info/EventSystem/Occluder/Floor_9 | 2 | 2 | 0 |
| /0/3/3/2 | VRChat World Info/EventSystem/Occluder/Floor_8 | 2 | 2 | 0 |
| /0/3/3/3 | VRChat World Info/EventSystem/Occluder/Floor_7 | 10 | 10 | 0 |
| /0/3/3/4 | VRChat World Info/EventSystem/Occluder/Floor_6 | 2 | 2 | 0 |
| /0/3/3/5 | VRChat World Info/EventSystem/Occluder/Floor_5 | 2 | 2 | 0 |
| /0/3/3/6 | VRChat World Info/EventSystem/Occluder/Floor_4 | 2 | 2 | 0 |
| /0/3/3/7 | VRChat World Info/EventSystem/Occluder/Floor_3 | 2 | 2 | 0 |
| /0/3/3/8 | VRChat World Info/EventSystem/Occluder/Floor_2 | 2 | 2 | 0 |
| /0/3/3/9 | VRChat World Info/EventSystem/Occluder/Floor_1 | 2 | 2 | 0 |
| /0/3/3/10 | VRChat World Info/EventSystem/Occluder/Basement_1 | 2 | 2 | 0 |
| /0/3/3/11 | VRChat World Info/EventSystem/Occluder/Basement_2 | 3 | 3 | 0 |
| /0/3/4 | VRChat World Info/EventSystem/Currency_System | 7 | 7 | 0 |
| /0/3/4/0 | VRChat World Info/EventSystem/Currency_System/UdonChips | 2 | 2 | 0 |
| /0/3/4/1 | VRChat World Info/EventSystem/Currency_System/UdonGameChips | 1 | 1 | 0 |
| /0/3/4/2 | VRChat World Info/EventSystem/Currency_System/UdonChipsAutoGain | 1 | 1 | 0 |
| /0/3/4/3 | VRChat World Info/EventSystem/Currency_System/UdonChipsMoveSpeed | 1 | 1 | 0 |
| /0/3/4/4 | VRChat World Info/EventSystem/Currency_System/UdonChipsLoginBonus(Offline) | 1 | 1 | 0 |
| /0/3/5 | VRChat World Info/EventSystem/LTCGI Controller | 1 | 1 | 0 |
| /1 | Unity-RecorderBindings | 1 | 1 | 1 |
| /2 | World Layers | 32903 | 9664 | 18980 |
| /2/0 | World Layers/N.Luminous Hotel | 32901 | 9662 | 18980 |
| /2/0/0 | World Layers/N.Luminous Hotel/Rooftop | 7010 | 0 | 7010 |
| /2/0/0/0 | World Layers/N.Luminous Hotel/Rooftop/StairArea | 346 | 0 | 346 |
| /2/0/0/1 | World Layers/N.Luminous Hotel/Rooftop/AbstractEcho | 6663 | 0 | 6663 |
| /2/0/1 | World Layers/N.Luminous Hotel/R~F9 | 44 | 0 | 44 |
| /2/0/1/0 | World Layers/N.Luminous Hotel/R~F9/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/2 | World Layers/N.Luminous Hotel/Floor_9 | 484 | 0 | 484 |
| /2/0/2/0 | World Layers/N.Luminous Hotel/Floor_9/StairArea | 483 | 0 | 483 |
| /2/0/3 | World Layers/N.Luminous Hotel/F8~F9 | 44 | 0 | 44 |
| /2/0/3/0 | World Layers/N.Luminous Hotel/F8~F9/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/4 | World Layers/N.Luminous Hotel/Floor_8 | 483 | 0 | 483 |
| /2/0/4/0 | World Layers/N.Luminous Hotel/Floor_8/StairArea | 482 | 0 | 482 |
| /2/0/5 | World Layers/N.Luminous Hotel/F7~F8 | 44 | 0 | 44 |
| /2/0/5/0 | World Layers/N.Luminous Hotel/F7~F8/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/6 | World Layers/N.Luminous Hotel/Floor_7 | 12220 | 6736 | 1358 |
| /2/0/6/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea | 3815 | 1571 | 202 |
| /2/0/6/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace | 1533 | 817 | 514 |
| /2/0/6/2 | World Layers/N.Luminous Hotel/Floor_7/SmokingSpace | 65 | 58 | 24 |
| /2/0/6/3 | World Layers/N.Luminous Hotel/Floor_7/StairArea | 645 | 512 | 141 |
| /2/0/6/4 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms | 6161 | 3777 | 477 |
| /2/0/7 | World Layers/N.Luminous Hotel/F6~F7 | 44 | 0 | 44 |
| /2/0/7/0 | World Layers/N.Luminous Hotel/F6~F7/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/8 | World Layers/N.Luminous Hotel/Floor_6 | 485 | 0 | 485 |
| /2/0/8/0 | World Layers/N.Luminous Hotel/Floor_6/StairArea | 484 | 0 | 484 |
| /2/0/9 | World Layers/N.Luminous Hotel/F5~F6 | 44 | 0 | 44 |
| /2/0/9/0 | World Layers/N.Luminous Hotel/F5~F6/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/10 | World Layers/N.Luminous Hotel/Floor_5 | 485 | 0 | 485 |
| /2/0/10/0 | World Layers/N.Luminous Hotel/Floor_5/StairArea | 484 | 0 | 484 |
| /2/0/11 | World Layers/N.Luminous Hotel/F4~F5 | 44 | 0 | 44 |
| /2/0/11/0 | World Layers/N.Luminous Hotel/F4~F5/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/12 | World Layers/N.Luminous Hotel/Floor_4 | 485 | 0 | 485 |
| /2/0/12/0 | World Layers/N.Luminous Hotel/Floor_4/StairArea | 484 | 0 | 484 |
| /2/0/13 | World Layers/N.Luminous Hotel/F3~F4 | 44 | 0 | 44 |
| /2/0/13/0 | World Layers/N.Luminous Hotel/F3~F4/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/14 | World Layers/N.Luminous Hotel/Floor_3 | 485 | 0 | 485 |
| /2/0/14/0 | World Layers/N.Luminous Hotel/Floor_3/StairArea | 484 | 0 | 484 |
| /2/0/15 | World Layers/N.Luminous Hotel/F2~F3 | 44 | 0 | 44 |
| /2/0/15/0 | World Layers/N.Luminous Hotel/F2~F3/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/16 | World Layers/N.Luminous Hotel/Floor_2 | 485 | 0 | 485 |
| /2/0/16/0 | World Layers/N.Luminous Hotel/Floor_2/StairArea | 484 | 0 | 484 |
| /2/0/17 | World Layers/N.Luminous Hotel/F1~F2 | 44 | 0 | 44 |
| /2/0/17/0 | World Layers/N.Luminous Hotel/F1~F2/StairArea_FloorBase | 43 | 0 | 43 |
| /2/0/18 | World Layers/N.Luminous Hotel/Floor_1 | 5255 | 0 | 5255 |
| /2/0/18/0 | World Layers/N.Luminous Hotel/Floor_1/StairArea | 484 | 0 | 484 |
| /2/0/18/1 | World Layers/N.Luminous Hotel/Floor_1/Architecture | 3813 | 0 | 3813 |
| /2/0/18/2 | World Layers/N.Luminous Hotel/Floor_1/Environment | 21 | 0 | 21 |
| /2/0/18/3 | World Layers/N.Luminous Hotel/Floor_1/OcclusionCulling | 3 | 0 | 3 |
| /2/0/18/4 | World Layers/N.Luminous Hotel/Floor_1/Elevator_Root | 767 | 0 | 767 |
| /2/0/18/5 | World Layers/N.Luminous Hotel/Floor_1/UdonObject_Dcut | 166 | 0 | 166 |
| /2/0/19 | World Layers/N.Luminous Hotel/B1~F1 | 43 | 0 | 43 |
| /2/0/19/0 | World Layers/N.Luminous Hotel/B1~F1/StairArea_FloorBase_Ceil | 1 | 0 | 1 |
| /2/0/19/1 | World Layers/N.Luminous Hotel/B1~F1/StairArea_FloorBase_Floor | 1 | 0 | 1 |
| /2/0/19/2 | World Layers/N.Luminous Hotel/B1~F1/StairArea_FloorBase_InnerCorner_Center | 1 | 0 | 1 |
| /2/0/19/3 | World Layers/N.Luminous Hotel/B1~F1/StairArea_FloorBase_InnerCorner_Edge | 1 | 0 | 1 |
| /2/0/19/4 | World Layers/N.Luminous Hotel/B1~F1/StairArea_FloorBase_OuterCorner | 1 | 0 | 1 |
| /2/0/19/5 | World Layers/N.Luminous Hotel/B1~F1/Stairs_ExitDoor | 9 | 0 | 9 |
| /2/0/19/6 | World Layers/N.Luminous Hotel/B1~F1/HotelModular_EdgeEmission | 22 | 0 | 22 |
| /2/0/19/7 | World Layers/N.Luminous Hotel/B1~F1/HotelModular_WallPanel | 6 | 0 | 6 |
| /2/0/20 | World Layers/N.Luminous Hotel/Basement_1 | 485 | 0 | 485 |
| /2/0/20/0 | World Layers/N.Luminous Hotel/Basement_1/StairArea | 484 | 0 | 484 |
| /2/0/21 | World Layers/N.Luminous Hotel/B2~B1 | 43 | 0 | 43 |
| /2/0/21/0 | World Layers/N.Luminous Hotel/B2~B1/StairArea_FloorBase_Ceil | 1 | 0 | 1 |
| /2/0/21/1 | World Layers/N.Luminous Hotel/B2~B1/StairArea_FloorBase_Floor | 1 | 0 | 1 |
| /2/0/21/2 | World Layers/N.Luminous Hotel/B2~B1/StairArea_FloorBase_InnerCorner_Center | 1 | 0 | 1 |
| /2/0/21/3 | World Layers/N.Luminous Hotel/B2~B1/StairArea_FloorBase_InnerCorner_Edge | 1 | 0 | 1 |
| /2/0/21/4 | World Layers/N.Luminous Hotel/B2~B1/StairArea_FloorBase_OuterCorner | 1 | 0 | 1 |
| /2/0/21/5 | World Layers/N.Luminous Hotel/B2~B1/Stairs_ExitDoor | 9 | 0 | 9 |
| /2/0/21/6 | World Layers/N.Luminous Hotel/B2~B1/HotelModular_EdgeEmission | 22 | 0 | 22 |
| /2/0/21/7 | World Layers/N.Luminous Hotel/B2~B1/HotelModular_WallPanel | 6 | 0 | 6 |
| /2/0/22 | World Layers/N.Luminous Hotel/Basement_2 | 3107 | 2467 | 533 |
| /2/0/22/0 | World Layers/N.Luminous Hotel/Basement_2/StairArea | 247 | 217 | 33 |
| /2/0/22/1 | World Layers/N.Luminous Hotel/Basement_2/LuminousOasis_Common | 871 | 356 | 291 |
| /2/0/22/2 | World Layers/N.Luminous Hotel/Basement_2/EntranceHall | 438 | 420 | 25 |
| /2/0/22/3 | World Layers/N.Luminous Hotel/Basement_2/StairArea | 11 | 8 | 3 |
| /2/0/22/4 | World Layers/N.Luminous Hotel/Basement_2/PoolArea | 916 | 889 | 97 |
| /2/0/22/5 | World Layers/N.Luminous Hotel/Basement_2/LoungeArea | 536 | 489 | 84 |
| /2/0/22/6 | World Layers/N.Luminous Hotel/Basement_2/Sauna | 87 | 87 | 0 |
| /2/0/23 | World Layers/N.Luminous Hotel/-----Common_Gimmicks----- | 1 | 1 | 1 |
| /2/0/24 | World Layers/N.Luminous Hotel/WelcomeBoard | 99 | 93 | 0 |
| /2/0/24/0 | World Layers/N.Luminous Hotel/WelcomeBoard/WelcomeBoard_701 | 49 | 46 | 0 |
| /2/0/24/1 | World Layers/N.Luminous Hotel/WelcomeBoard/WelcomeBoard_702 | 49 | 46 | 0 |
| /2/0/25 | World Layers/N.Luminous Hotel/FloorGuides | 125 | 83 | 20 |
| /2/0/25/0 | World Layers/N.Luminous Hotel/FloorGuides/Floor_7 | 124 | 82 | 20 |
| /2/0/26 | World Layers/N.Luminous Hotel/Elevators | 724 | 281 | 444 |
| /2/0/26/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A | 237 | 27 | 213 |
| /2/0/26/1 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B | 236 | 26 | 213 |
| /2/0/26/2 | World Layers/N.Luminous Hotel/Elevators/- - - - - - - - - - - - - - - - - - - - | 1 | 1 | 1 |
| /2/0/26/3 | World Layers/N.Luminous Hotel/Elevators/Elevator_A | 109 | 109 | 8 |
| /2/0/26/4 | World Layers/N.Luminous Hotel/Elevators/Elevator_B | 139 | 116 | 9 |
| /2/0/26/5 | World Layers/N.Luminous Hotel/Elevators/N.ElevatorSystem | 1 | 1 | 0 |
| /2/1 | World Layers/N.Exploration Area  | 1 | 1 | 0 |
| /3 | Extra Assets | 2205 | 411 | 686 |
| /3/0 | Extra Assets/WorldIntegratedMenu | 686 | 0 | 686 |
| /3/0/0 | Extra Assets/WorldIntegratedMenu/Modules | 207 | 0 | 207 |
| /3/0/0/0 | Extra Assets/WorldIntegratedMenu/Modules/WorldChangelogModule | 11 | 0 | 11 |
| /3/0/0/1 | Extra Assets/WorldIntegratedMenu/Modules/AssetListModule | 13 | 0 | 13 |
| /3/0/0/2 | Extra Assets/WorldIntegratedMenu/Modules/FreeTextModule | 9 | 0 | 9 |
| /3/0/0/3 | Extra Assets/WorldIntegratedMenu/Modules/JoinLogModule | 37 | 0 | 37 |
| /3/0/0/4 | Extra Assets/WorldIntegratedMenu/Modules/PlayerListModule | 24 | 0 | 24 |
| /3/0/0/5 | Extra Assets/WorldIntegratedMenu/Modules/SoundSettingsModule | 28 | 0 | 28 |
| /3/0/0/6 | Extra Assets/WorldIntegratedMenu/Modules/ToggleSwitchV2Module | 31 | 0 | 31 |
| /3/0/0/7 | Extra Assets/WorldIntegratedMenu/Modules/ToggleSwitchV2Module | 31 | 0 | 31 |
| /3/0/0/8 | Extra Assets/WorldIntegratedMenu/Modules/TeleportModule | 18 | 0 | 18 |
| /3/0/0/9 | Extra Assets/WorldIntegratedMenu/Modules/N_WIMChatModule | 2 | 0 | 2 |
| /3/0/0/10 | Extra Assets/WorldIntegratedMenu/Modules/N_WIMInventoryModule | 2 | 0 | 2 |
| /3/0/1 | Extra Assets/WorldIntegratedMenu/Canvas | 64 | 0 | 64 |
| /3/0/1/0 | Extra Assets/WorldIntegratedMenu/Canvas/EventSystem | 1 | 0 | 1 |
| /3/0/1/1 | Extra Assets/WorldIntegratedMenu/Canvas/Background | 1 | 0 | 1 |
| /3/0/1/2 | Extra Assets/WorldIntegratedMenu/Canvas/Unavailable | 5 | 0 | 5 |
| /3/0/1/3 | Extra Assets/WorldIntegratedMenu/Canvas/Panel | 56 | 0 | 56 |
| /3/0/2 | Extra Assets/WorldIntegratedMenu/System | 414 | 0 | 414 |
| /3/0/2/0 | Extra Assets/WorldIntegratedMenu/System/TutorialOverlay | 8 | 0 | 8 |
| /3/0/2/1 | Extra Assets/WorldIntegratedMenu/System/QuickMenu | 11 | 0 | 11 |
| /3/0/2/2 | Extra Assets/WorldIntegratedMenu/System/MobileQMButton | 5 | 0 | 5 |
| /3/0/2/3 | Extra Assets/WorldIntegratedMenu/System/UIManager | 1 | 0 | 1 |
| /3/0/2/4 | Extra Assets/WorldIntegratedMenu/System/ModuleManager | 385 | 0 | 385 |
| /3/0/2/5 | Extra Assets/WorldIntegratedMenu/System/ThemeManager | 1 | 0 | 1 |
| /3/0/2/6 | Extra Assets/WorldIntegratedMenu/System/I18nManager | 1 | 0 | 1 |
| /3/0/2/7 | Extra Assets/WorldIntegratedMenu/System/CloudSyncManager | 1 | 0 | 1 |
| /3/1 | Extra Assets/SitLine | 5 | 1 | 0 |
| /3/1/0 | Extra Assets/SitLine/PlayerObject | 4 | 0 | 0 |
| /3/1/0/0 | Extra Assets/SitLine/PlayerObject/FlekSit | 3 | 0 | 0 |
| /3/2 | Extra Assets/UnyStylusPen | 361 | 0 | 0 |
| /3/2/0 | Extra Assets/UnyStylusPen/Model | 2 | 0 | 0 |
| /3/2/0/0 | Extra Assets/UnyStylusPen/Model/UnyStylus | 1 | 0 | 0 |
| /3/2/1 | Extra Assets/UnyStylusPen/UnyStylusController | 358 | 0 | 0 |
| /3/2/1/0 | Extra Assets/UnyStylusPen/UnyStylusController/PenTip | 55 | 0 | 0 |
| /3/2/1/1 | Extra Assets/UnyStylusPen/UnyStylusController/PenMenu | 283 | 0 | 0 |
| /3/2/1/2 | Extra Assets/UnyStylusPen/UnyStylusController/PenPopup | 10 | 0 | 0 |
| /3/2/1/3 | Extra Assets/UnyStylusPen/UnyStylusController/PlayerPopup | 8 | 0 | 0 |
| /3/2/1/4 | Extra Assets/UnyStylusPen/UnyStylusController/Desktop | 1 | 0 | 0 |
| /3/3 | Extra Assets/WeatherSystem | 5 | 1 | 0 |
| /3/3/0 | Extra Assets/WeatherSystem/Sunny | 1 | 0 | 0 |
| /3/3/1 | Extra Assets/WeatherSystem/Cloudy | 1 | 0 | 0 |
| /3/3/2 | Extra Assets/WeatherSystem/Rainy | 1 | 0 | 0 |
| /3/3/3 | Extra Assets/WeatherSystem/Snowy | 1 | 0 | 0 |
| /3/4 | Extra Assets/TIM_QM | 1070 | 340 | 0 |
| /3/4/0 | Extra Assets/TIM_QM/PlayerScale | 1 | 1 | 0 |
| /3/4/1 | Extra Assets/TIM_QM/TIM_Scripts | 708 | 28 | 0 |
| /3/4/1/0 | Extra Assets/TIM_QM/TIM_Scripts/[TIM_IME] | 704 | 24 | 0 |
| /3/4/1/1 | Extra Assets/TIM_QM/TIM_Scripts/UI_Localized | 1 | 1 | 0 |
| /3/4/1/2 | Extra Assets/TIM_QM/TIM_Scripts/ButtonSettings | 1 | 1 | 0 |
| /3/4/1/3 | Extra Assets/TIM_QM/TIM_Scripts/AdminTeleport(スタッフはここにテレポート) | 1 | 1 | 0 |
| /3/4/2 | Extra Assets/TIM_QM/SE | 2 | 2 | 0 |
| /3/4/2/0 | Extra Assets/TIM_QM/SE/UISound | 1 | 1 | 0 |
| /3/4/3 | Extra Assets/TIM_QM/TIM_QMTrigger_Root | 77 | 74 | 0 |
| /3/4/3/0 | Extra Assets/TIM_QM/TIM_QMTrigger_Root/TriggerAnchor | 76 | 73 | 0 |
| /3/4/4 | Extra Assets/TIM_QM/TIM_QMWhitelist | 27 | 0 | 0 |
| /3/4/4/0 | Extra Assets/TIM_QM/TIM_QMWhitelist/PadCanvas | 26 | 0 | 0 |
| /3/4/5 | Extra Assets/TIM_QM/TIM_QMNameTag | 254 | 234 | 0 |
| /3/4/5/0 | Extra Assets/TIM_QM/TIM_QMNameTag/TIM_NameTagSystem | 19 | 2 | 0 |
| /3/4/5/1 | Extra Assets/TIM_QM/TIM_QMNameTag/NameTagIconObject | 1 | 0 | 0 |
| /3/4/5/2 | Extra Assets/TIM_QM/TIM_QMNameTag/NameTagPreviewCamera | 1 | 1 | 0 |
| /3/4/5/3 | Extra Assets/TIM_QM/TIM_QMNameTag/MenuCanvas | 232 | 230 | 0 |
| /3/5 | Extra Assets/AuthorityKey | 10 | 9 | 0 |
| /3/5/0 | Extra Assets/AuthorityKey/CardKey | 8 | 8 | 0 |
| /3/5/0/0 | Extra Assets/AuthorityKey/CardKey/CardKey_Text_Front | 3 | 3 | 0 |
| /3/5/0/1 | Extra Assets/AuthorityKey/CardKey/CardKey_Text_Back | 4 | 4 | 0 |
| /3/5/1 | Extra Assets/AuthorityKey/CardKey_VIP | 1 | 0 | 0 |
| /3/6 | Extra Assets/UdonChipsWallet | 3 | 3 | 0 |
| /3/6/0 | Extra Assets/UdonChipsWallet/UdonChips_MoneyText | 2 | 2 | 0 |
| /3/6/0/0 | Extra Assets/UdonChipsWallet/UdonChips_MoneyText/MoneyLabel | 1 | 1 | 0 |
| /3/7 | Extra Assets/GameChipsWallet | 3 | 3 | 0 |
| /3/7/0 | Extra Assets/GameChipsWallet/UdonChips_MoneyText | 2 | 2 | 0 |
| /3/7/0/0 | Extra Assets/GameChipsWallet/UdonChips_MoneyText/MoneyLabel | 1 | 1 | 0 |
| /3/8 | Extra Assets/Chat System | 61 | 53 | 0 |
| /3/8/0 | Extra Assets/Chat System/Canvas | 47 | 41 | 0 |
| /3/8/0/0 | Extra Assets/Chat System/Canvas/Scroll View | 46 | 40 | 0 |
| /3/8/1 | Extra Assets/Chat System/Canvas | 11 | 9 | 0 |
| /3/8/1/0 | Extra Assets/Chat System/Canvas/Toggle | 5 | 4 | 0 |
| /3/8/1/1 | Extra Assets/Chat System/Canvas/Toggle | 5 | 4 | 0 |
| /3/8/2 | Extra Assets/Chat System/Camera | 1 | 1 | 0 |
| /3/8/3 | Extra Assets/Chat System/Audio Source | 1 | 1 | 0 |
| /4 | Experimental | 62 | 0 | 62 |
| /4/0 | Experimental/さたにあ式防音室 | 8 | 0 | 8 |
| /4/0/0 | Experimental/さたにあ式防音室/Room_1 | 5 | 0 | 5 |
| /4/0/0/0 | Experimental/さたにあ式防音室/Room_1/確認用 (EditorOnly) | 1 | 0 | 1 |
| /4/0/0/1 | Experimental/さたにあ式防音室/Room_1/Canvas | 3 | 0 | 3 |
| /4/0/1 | Experimental/さたにあ式防音室/PlayerVolumeController | 1 | 0 | 1 |
| /4/0/2 | Experimental/さたにあ式防音室/SoundProofRoomController | 1 | 0 | 1 |
| /4/1 | Experimental/さたにあ式マイク Reverb.ver | 20 | 0 | 20 |
| /4/1/0 | Experimental/さたにあ式マイク Reverb.ver/Canvas | 7 | 0 | 7 |
| /4/1/0/0 | Experimental/さたにあ式マイク Reverb.ver/Canvas/Image | 1 | 0 | 1 |
| /4/1/0/1 | Experimental/さたにあ式マイク Reverb.ver/Canvas/Text | 1 | 0 | 1 |
| /4/1/0/2 | Experimental/さたにあ式マイク Reverb.ver/Canvas/Toggle | 4 | 0 | 4 |
| /4/1/1 | Experimental/さたにあ式マイク Reverb.ver/BLACK | 2 | 0 | 2 |
| /4/1/1/0 | Experimental/さたにあ式マイク Reverb.ver/BLACK/Mic | 1 | 0 | 1 |
| /4/1/2 | Experimental/さたにあ式マイク Reverb.ver/BLACK 2 | 2 | 0 | 2 |
| /4/1/2/0 | Experimental/さたにあ式マイク Reverb.ver/BLACK 2/Mic | 1 | 0 | 1 |
| /4/1/3 | Experimental/さたにあ式マイク Reverb.ver/WHITE | 2 | 0 | 2 |
| /4/1/3/0 | Experimental/さたにあ式マイク Reverb.ver/WHITE/Mic | 1 | 0 | 1 |
| /4/1/4 | Experimental/さたにあ式マイク Reverb.ver/WHITE 2 | 2 | 0 | 2 |
| /4/1/4/0 | Experimental/さたにあ式マイク Reverb.ver/WHITE 2/Mic | 1 | 0 | 1 |
| /4/1/5 | Experimental/さたにあ式マイク Reverb.ver/PlayerVolumeController | 1 | 0 | 1 |
| /4/1/6 | Experimental/さたにあ式マイク Reverb.ver/SataniaMicManager | 1 | 0 | 1 |
| /4/1/7 | Experimental/さたにあ式マイク Reverb.ver/Reverb | 2 | 0 | 2 |
| /4/1/7/0 | Experimental/さたにあ式マイク Reverb.ver/Reverb/Main | 1 | 0 | 1 |
| /4/2 | Experimental/Attenuation Tool | 4 | 0 | 4 |
| /4/2/0 | Experimental/Attenuation Tool/Colliders | 1 | 0 | 1 |
| /4/2/1 | Experimental/Attenuation Tool/ログ用キャンバス(削除可能) | 2 | 0 | 2 |
| /4/2/1/0 | Experimental/Attenuation Tool/ログ用キャンバス(削除可能)/ログテキスト | 1 | 0 | 1 |
| /4/3 | Experimental/Audio Channel Manager | 1 | 0 | 1 |
| /4/4 | Experimental/Audio Channel Manager Panel | 11 | 0 | 11 |
| /4/4/0 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体 | 10 | 0 | 10 |
| /4/4/0/0 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/背景 | 1 | 0 | 1 |
| /4/4/0/1 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/タイトル | 1 | 0 | 1 |
| /4/4/0/2 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/チャンネル情報 | 1 | 0 | 1 |
| /4/4/0/3 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/区切り線 | 1 | 0 | 1 |
| /4/4/0/4 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/チャンネルID | 1 | 0 | 1 |
| /4/4/0/5 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/戻るボタン | 2 | 0 | 2 |
| /4/4/0/6 | Experimental/Audio Channel Manager Panel/オーディオチャンネル管理パネル本体/進むボタン | 2 | 0 | 2 |
| /4/5 | Experimental/Audio Channel Player List | 17 | 0 | 17 |
| /4/5/0 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト | 16 | 0 | 16 |
| /4/5/0/0 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/背景 | 1 | 0 | 1 |
| /4/5/0/1 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/タイトル | 1 | 0 | 1 |
| /4/5/0/2 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/区切り線 | 1 | 0 | 1 |
| /4/5/0/3 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/プレイヤーリスト一覧 | 7 | 0 | 7 |
| /4/5/0/4 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/チャンネルID | 1 | 0 | 1 |
| /4/5/0/5 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/戻るボタン | 2 | 0 | 2 |
| /4/5/0/6 | Experimental/Audio Channel Player List/オーディオチャンネルプレイヤーリスト/進むボタン | 2 | 0 | 2 |
| /5 | -----OldExtra_Assets----- | 6164 | 0 | 6164 |
| /5/0 | -----OldExtra_Assets-----/DayCycleSystem | 1 | 0 | 1 |
| /5/1 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager | 1055 | 0 | 1055 |
| /5/1/0 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Preset_Entrance | 1 | 0 | 1 |
| /5/1/1 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Range_Entrance | 1 | 0 | 1 |
| /5/1/2 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Preset_Room_701 | 1 | 0 | 1 |
| /5/1/3 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Range_Room_701 | 1 | 0 | 1 |
| /5/1/4 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Preset_Room_702 | 1 | 0 | 1 |
| /5/1/5 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/Range_Room_702 | 1 | 0 | 1 |
| /5/1/6 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_701 | 524 | 0 | 524 |
| /5/1/6/0 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_701/Controller | 104 | 0 | 104 |
| /5/1/6/1 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_701/Screen | 1 | 0 | 1 |
| /5/1/6/2 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_701/Audio Source | 1 | 0 | 1 |
| /5/1/6/3 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_701/ScreenUI | 417 | 0 | 417 |
| /5/1/7 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_702 | 524 | 0 | 524 |
| /5/1/7/0 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_702/Controller | 104 | 0 | 104 |
| /5/1/7/1 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_702/Screen | 1 | 0 | 1 |
| /5/1/7/2 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_702/Audio Source | 1 | 0 | 1 |
| /5/1/7/3 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager/N_YamaPool_702/ScreenUI | 417 | 0 | 417 |
| /5/2 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB | 582 | 0 | 582 |
| /5/2/0 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Pens | 527 | 0 | 527 |
| /5/2/0/0 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Pens/LaChicPens | 526 | 0 | 526 |
| /5/2/1 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Erasers | 26 | 0 | 26 |
| /5/2/1/0 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Erasers/LaChicErasers | 25 | 0 | 25 |
| /5/2/2 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Bureau | 28 | 0 | 28 |
| /5/2/2/0 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Bureau/Settings | 1 | 0 | 1 |
| /5/2/2/1 | -----OldExtra_Assets-----/LaChicPen_04_BlackWood_WithStandTypeB/Bureau/UI | 26 | 0 | 26 |
| /5/3 | -----OldExtra_Assets-----/RTab_Stand | 2514 | 0 | 2514 |
| /5/3/0 | -----OldExtra_Assets-----/RTab_Stand/TabletManager | 57 | 0 | 57 |
| /5/3/0/0 | -----OldExtra_Assets-----/RTab_Stand/TabletManager/Tablet | 3 | 0 | 3 |
| /5/3/0/1 | -----OldExtra_Assets-----/RTab_Stand/TabletManager/TabletCover | 15 | 0 | 15 |
| /5/3/0/2 | -----OldExtra_Assets-----/RTab_Stand/TabletManager/ColliderDetector | 3 | 0 | 3 |
| /5/3/0/3 | -----OldExtra_Assets-----/RTab_Stand/TabletManager/Canvas | 35 | 0 | 35 |
| /5/3/1 | -----OldExtra_Assets-----/RTab_Stand/Apps | 2456 | 0 | 2456 |
| /5/3/1/0 | -----OldExtra_Assets-----/RTab_Stand/Apps/CameraApp | 18 | 0 | 18 |
| /5/3/1/1 | -----OldExtra_Assets-----/RTab_Stand/Apps/PhotoViewer | 40 | 0 | 40 |
| /5/3/1/2 | -----OldExtra_Assets-----/RTab_Stand/Apps/VideoPlayer | 435 | 0 | 435 |
| /5/3/1/3 | -----OldExtra_Assets-----/RTab_Stand/Apps/PlayerLog | 158 | 0 | 158 |
| /5/3/1/4 | -----OldExtra_Assets-----/RTab_Stand/Apps/URLShare | 1630 | 0 | 1630 |
| /5/3/1/5 | -----OldExtra_Assets-----/RTab_Stand/Apps/ObjectSwitch | 89 | 0 | 89 |
| /5/3/1/6 | -----OldExtra_Assets-----/RTab_Stand/Apps/ScreenCast | 29 | 0 | 29 |
| /5/3/1/7 | -----OldExtra_Assets-----/RTab_Stand/Apps/Credit | 6 | 0 | 6 |
| /5/3/1/8 | -----OldExtra_Assets-----/RTab_Stand/Apps/VideoPlayerLinks | 50 | 0 | 50 |
| /5/4 | -----OldExtra_Assets-----/PortalManager | 6 | 0 | 6 |
| /5/4/0 | -----OldExtra_Assets-----/PortalManager/Portal_01 | 1 | 0 | 1 |
| /5/4/1 | -----OldExtra_Assets-----/PortalManager/Portal_02 | 1 | 0 | 1 |
| /5/4/2 | -----OldExtra_Assets-----/PortalManager/Portal_03 | 1 | 0 | 1 |
| /5/4/3 | -----OldExtra_Assets-----/PortalManager/Portal_04 | 1 | 0 | 1 |
| /5/4/4 | -----OldExtra_Assets-----/PortalManager/Portal_05 | 1 | 0 | 1 |
| /5/5 | -----OldExtra_Assets-----/AgentManager | 17 | 0 | 17 |
| /5/5/0 | -----OldExtra_Assets-----/AgentManager/PlayerTrackingDataProvider | 1 | 0 | 1 |
| /5/5/1 | -----OldExtra_Assets-----/AgentManager/LocomotionManager | 1 | 0 | 1 |
| /5/5/2 | -----OldExtra_Assets-----/AgentManager/Canvas | 9 | 0 | 9 |
| /5/5/2/0 | -----OldExtra_Assets-----/AgentManager/Canvas/Panel | 1 | 0 | 1 |
| /5/5/2/1 | -----OldExtra_Assets-----/AgentManager/Canvas/Image | 1 | 0 | 1 |
| /5/5/2/2 | -----OldExtra_Assets-----/AgentManager/Canvas/Version | 1 | 0 | 1 |
| /5/5/2/3 | -----OldExtra_Assets-----/AgentManager/Canvas/HeadTrackingData | 1 | 0 | 1 |
| /5/5/2/4 | -----OldExtra_Assets-----/AgentManager/Canvas/TrackingDataDebug | 2 | 0 | 2 |
| /5/5/2/5 | -----OldExtra_Assets-----/AgentManager/Canvas/Agent Debug Display | 2 | 0 | 2 |
| /5/5/3 | -----OldExtra_Assets-----/AgentManager/PlayerEyeDirection | 2 | 0 | 2 |
| /5/5/3/0 | -----OldExtra_Assets-----/AgentManager/PlayerEyeDirection/Cube | 1 | 0 | 1 |
| /5/5/4 | -----OldExtra_Assets-----/AgentManager/IgnoreToggle | 3 | 0 | 3 |
| /5/5/4/0 | -----OldExtra_Assets-----/AgentManager/IgnoreToggle/IgonrebyAgent | 2 | 0 | 2 |
| /5/6 | -----OldExtra_Assets-----/ClimbZoneController | 6 | 0 | 6 |
| /5/6/0 | -----OldExtra_Assets-----/ClimbZoneController/ClimbZoneController | 1 | 0 | 1 |
| /5/6/1 | -----OldExtra_Assets-----/ClimbZoneController/ClimbZoneControllerVR | 1 | 0 | 1 |
| /5/6/2 | -----OldExtra_Assets-----/ClimbZoneController/WallSample | 1 | 0 | 1 |
| /5/6/3 | -----OldExtra_Assets-----/ClimbZoneController/WallTriggerSample | 1 | 0 | 1 |
| /5/6/4 | -----OldExtra_Assets-----/ClimbZoneController/ClimbHandAnchor | 1 | 0 | 1 |
| /5/7 | -----OldExtra_Assets-----/DiceSet | 41 | 0 | 41 |
| /5/7/0 | -----OldExtra_Assets-----/DiceSet/Tablet | 17 | 0 | 17 |
| /5/7/0/0 | -----OldExtra_Assets-----/DiceSet/Tablet/DiceInfo | 16 | 0 | 16 |
| /5/7/1 | -----OldExtra_Assets-----/DiceSet/Dice_TeleportTarget | 2 | 0 | 2 |
| /5/7/1/0 | -----OldExtra_Assets-----/DiceSet/Dice_TeleportTarget/audioSourceBad | 1 | 0 | 1 |
| /5/7/2 | -----OldExtra_Assets-----/DiceSet/DiceArea | 1 | 0 | 1 |
| /5/7/3 | -----OldExtra_Assets-----/DiceSet/Dice | 17 | 0 | 17 |
| /5/7/3/0 | -----OldExtra_Assets-----/DiceSet/Dice/Dice_6 | 7 | 0 | 7 |
| /5/7/3/1 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourcePickup | 1 | 0 | 1 |
| /5/7/3/2 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourceGood | 1 | 0 | 1 |
| /5/7/3/3 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourceBad | 1 | 0 | 1 |
| /5/7/3/4 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourceDrop | 1 | 0 | 1 |
| /5/7/3/5 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourceJackpot | 1 | 0 | 1 |
| /5/7/3/6 | -----OldExtra_Assets-----/DiceSet/Dice/audioSourceJackpotLost | 1 | 0 | 1 |
| /5/7/3/7 | -----OldExtra_Assets-----/DiceSet/Dice/JackPotParticle | 1 | 0 | 1 |
| /5/7/3/8 | -----OldExtra_Assets-----/DiceSet/Dice/JackPotLostParticle | 2 | 0 | 2 |
| /5/7/4 | -----OldExtra_Assets-----/DiceSet/DiceInfoSync | 1 | 0 | 1 |
| /5/7/5 | -----OldExtra_Assets-----/DiceSet/DiceSign | 2 | 0 | 2 |
| /5/7/5/0 | -----OldExtra_Assets-----/DiceSet/DiceSign/Warning | 1 | 0 | 1 |
| /5/8 | -----OldExtra_Assets-----/WisperShisha | 122 | 0 | 122 |
| /5/8/0 | -----OldExtra_Assets-----/WisperShisha/Charcoals | 9 | 0 | 9 |
| /5/8/0/0 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_1 | 1 | 0 | 1 |
| /5/8/0/1 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_2 | 1 | 0 | 1 |
| /5/8/0/2 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_3 | 1 | 0 | 1 |
| /5/8/0/3 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_4 | 1 | 0 | 1 |
| /5/8/0/4 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_5 | 1 | 0 | 1 |
| /5/8/0/5 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_6 | 1 | 0 | 1 |
| /5/8/0/6 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_7 | 1 | 0 | 1 |
| /5/8/0/7 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_8 | 1 | 0 | 1 |
| /5/8/1 | -----OldExtra_Assets-----/WisperShisha/Shisha | 56 | 0 | 56 |
| /5/8/1/0 | -----OldExtra_Assets-----/WisperShisha/Shisha/PickPoint | 1 | 0 | 1 |
| /5/8/1/1 | -----OldExtra_Assets-----/WisperShisha/Shisha/Shisha | 54 | 0 | 54 |
| /5/8/2 | -----OldExtra_Assets-----/WisperShisha/Flavors | 23 | 0 | 23 |
| /5/8/2/0 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_MEBI | 1 | 0 | 1 |
| /5/8/2/1 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_WHITE | 1 | 0 | 1 |
| /5/8/2/2 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_TIRU | 1 | 0 | 1 |
| /5/8/2/3 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_PAREO | 1 | 0 | 1 |
| /5/8/2/4 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_EIKA | 1 | 0 | 1 |
| /5/8/2/5 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_AKANE | 1 | 0 | 1 |
| /5/8/2/6 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_TIKOKU | 1 | 0 | 1 |
| /5/8/2/7 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_MILK | 1 | 0 | 1 |
| /5/8/2/8 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_SENATI | 1 | 0 | 1 |
| /5/8/2/9 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_MOGI | 1 | 0 | 1 |
| /5/8/2/10 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_SINO | 1 | 0 | 1 |
| /5/8/2/11 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_HEARTBEAT | 1 | 0 | 1 |
| /5/8/2/12 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_CLOCK | 1 | 0 | 1 |
| /5/8/2/13 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_BIRD | 1 | 0 | 1 |
| /5/8/2/14 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_DROP | 1 | 0 | 1 |
| /5/8/2/15 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_FIRE | 1 | 0 | 1 |
| /5/8/2/16 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_RAIN | 1 | 0 | 1 |
| /5/8/2/17 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_THANDER | 1 | 0 | 1 |
| /5/8/2/18 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_NATUKITUNE | 1 | 0 | 1 |
| /5/8/2/19 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_RAKURIMA | 1 | 0 | 1 |
| /5/8/2/20 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_SORARA | 1 | 0 | 1 |
| /5/8/2/21 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_KRIS | 1 | 0 | 1 |
| /5/8/3 | -----OldExtra_Assets-----/WisperShisha/Tongs | 2 | 0 | 2 |
| /5/8/3/0 | -----OldExtra_Assets-----/WisperShisha/Tongs/pickPoint | 1 | 0 | 1 |
| /5/8/4 | -----OldExtra_Assets-----/WisperShisha/Heater | 3 | 0 | 3 |
| /5/8/4/0 | -----OldExtra_Assets-----/WisperShisha/Heater/col | 1 | 0 | 1 |
| /5/8/4/1 | -----OldExtra_Assets-----/WisperShisha/Heater/button | 1 | 0 | 1 |
| /5/8/5 | -----OldExtra_Assets-----/WisperShisha/Charcoal_Basket | 4 | 0 | 4 |
| /5/8/5/0 | -----OldExtra_Assets-----/WisperShisha/Charcoal_Basket/col | 1 | 0 | 1 |
| /5/8/5/1 | -----OldExtra_Assets-----/WisperShisha/Charcoal_Basket/zone | 1 | 0 | 1 |
| /5/8/5/2 | -----OldExtra_Assets-----/WisperShisha/Charcoal_Basket/holder | 1 | 0 | 1 |
| /5/8/6 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder | 7 | 0 | 7 |
| /5/8/6/0 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Ceramic_Bowl | 2 | 0 | 2 |
| /5/8/6/1 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Glass_Bowl | 2 | 0 | 2 |
| /5/8/6/2 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Silicone_Bowl | 2 | 0 | 2 |
| /5/8/7 | -----OldExtra_Assets-----/WisperShisha/Turkish_Lids | 5 | 0 | 5 |
| /5/8/7/0 | -----OldExtra_Assets-----/WisperShisha/Turkish_Lids/Turkish_Lid | 4 | 0 | 4 |
| /5/8/8 | -----OldExtra_Assets-----/WisperShisha/Head | 12 | 0 | 12 |
| /5/8/8/0 | -----OldExtra_Assets-----/WisperShisha/Head/Blur_Space | 1 | 0 | 1 |
| /5/8/8/1 | -----OldExtra_Assets-----/WisperShisha/Head/Audio_Space | 10 | 0 | 10 |
| /5/9 | -----OldExtra_Assets-----/FishingRodDark | 69 | 0 | 69 |
| /5/9/0 | -----OldExtra_Assets-----/FishingRodDark/RodHandle1 | 1 | 0 | 1 |
| /5/9/1 | -----OldExtra_Assets-----/FishingRodDark/ReelHandle | 1 | 0 | 1 |
| /5/9/2 | -----OldExtra_Assets-----/FishingRodDark/Syncs | 4 | 0 | 4 |
| /5/9/2/0 | -----OldExtra_Assets-----/FishingRodDark/Syncs/LinePos | 1 | 0 | 1 |
| /5/9/2/1 | -----OldExtra_Assets-----/FishingRodDark/Syncs/LineVel | 1 | 0 | 1 |
| /5/9/2/2 | -----OldExtra_Assets-----/FishingRodDark/Syncs/RodRot | 1 | 0 | 1 |
| /5/9/3 | -----OldExtra_Assets-----/FishingRodDark/Rod | 53 | 0 | 53 |
| /5/9/3/0 | -----OldExtra_Assets-----/FishingRodDark/Rod/Armature | 36 | 0 | 36 |
| /5/9/3/1 | -----OldExtra_Assets-----/FishingRodDark/Rod/Line | 1 | 0 | 1 |
| /5/9/3/2 | -----OldExtra_Assets-----/FishingRodDark/Rod/Lure | 2 | 0 | 2 |
| /5/9/3/3 | -----OldExtra_Assets-----/FishingRodDark/Rod/Reel | 10 | 0 | 10 |
| /5/9/3/4 | -----OldExtra_Assets-----/FishingRodDark/Rod/Rod | 1 | 0 | 1 |
| /5/9/3/5 | -----OldExtra_Assets-----/FishingRodDark/Rod/Rod2 | 1 | 0 | 1 |
| /5/9/3/6 | -----OldExtra_Assets-----/FishingRodDark/Rod/RodGrip1 | 1 | 0 | 1 |
| /5/9/4 | -----OldExtra_Assets-----/FishingRodDark/Arrow | 4 | 0 | 4 |
| /5/9/4/0 | -----OldExtra_Assets-----/FishingRodDark/Arrow/Name | 2 | 0 | 2 |
| /5/9/4/1 | -----OldExtra_Assets-----/FishingRodDark/Arrow/Plane | 1 | 0 | 1 |
| /5/9/5 | -----OldExtra_Assets-----/FishingRodDark/Fish | 3 | 0 | 3 |
| /5/9/5/0 | -----OldExtra_Assets-----/FishingRodDark/Fish/Left boot | 1 | 0 | 1 |
| /5/9/5/1 | -----OldExtra_Assets-----/FishingRodDark/Fish/right sandal | 1 | 0 | 1 |
| /5/9/6 | -----OldExtra_Assets-----/FishingRodDark/Splash | 2 | 0 | 2 |
| /5/9/6/0 | -----OldExtra_Assets-----/FishingRodDark/Splash/SplashAudioSource | 1 | 0 | 1 |
| /5/10 | -----OldExtra_Assets-----/KaraokeLink_Yama | 27 | 0 | 27 |
| /5/10/0 | -----OldExtra_Assets-----/KaraokeLink_Yama/MicroPhone | 11 | 0 | 11 |
| /5/10/0/0 | -----OldExtra_Assets-----/KaraokeLink_Yama/MicroPhone/Mic | 3 | 0 | 3 |
| /5/10/0/1 | -----OldExtra_Assets-----/KaraokeLink_Yama/MicroPhone/KaraokeReverb | 1 | 0 | 1 |
| /5/10/0/2 | -----OldExtra_Assets-----/KaraokeLink_Yama/MicroPhone/SingerMenu | 6 | 0 | 6 |
| /5/10/1 | -----OldExtra_Assets-----/KaraokeLink_Yama/Canvas | 13 | 0 | 13 |
| /5/10/1/0 | -----OldExtra_Assets-----/KaraokeLink_Yama/Canvas/Image | 1 | 0 | 1 |
| /5/10/1/1 | -----OldExtra_Assets-----/KaraokeLink_Yama/Canvas/UI | 11 | 0 | 11 |
| /5/10/2 | -----OldExtra_Assets-----/KaraokeLink_Yama/KaraokeStageArea | 2 | 0 | 2 |
| /5/10/2/0 | -----OldExtra_Assets-----/KaraokeLink_Yama/KaraokeStageArea/visual | 1 | 0 | 1 |
| /5/11 | -----OldExtra_Assets-----/NamehideSystem | 7 | 0 | 7 |
| /5/11/0 | -----OldExtra_Assets-----/NamehideSystem/NameHide_Player | 1 | 0 | 1 |
| /5/11/1 | -----OldExtra_Assets-----/NamehideSystem/NameHide_Camera | 1 | 0 | 1 |
| /5/11/2 | -----OldExtra_Assets-----/NamehideSystem/Camera_UIHideSystem | 1 | 0 | 1 |
| /5/11/3 | -----OldExtra_Assets-----/NamehideSystem/Camera_UIHideSystem_LocalCamera | 3 | 0 | 3 |
| /5/11/3/0 | -----OldExtra_Assets-----/NamehideSystem/Camera_UIHideSystem_LocalCamera/Camera_UIHideLocalCamera | 2 | 0 | 2 |
| /5/12 | -----OldExtra_Assets-----/Potato Chips | 69 | 0 | 69 |
| /5/12/0 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag | 31 | 0 | 31 |
| /5/12/0/0 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Armature_Chips_Bag | 10 | 0 | 10 |
| /5/12/0/1 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Chips_Bag | 1 | 0 | 1 |
| /5/12/0/2 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Unpack | 14 | 0 | 14 |
| /5/12/0/3 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Particles | 3 | 0 | 3 |
| /5/12/0/4 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Audio | 1 | 0 | 1 |
| /5/12/0/5 | -----OldExtra_Assets-----/Potato Chips/Potato Chips Bag/Chips_Parent | 1 | 0 | 1 |
| /5/12/1 | -----OldExtra_Assets-----/Potato Chips/Chips | 37 | 0 | 37 |
| /5/12/1/0 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_1 | 3 | 0 | 3 |
| /5/12/1/1 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_1 (1) | 3 | 0 | 3 |
| /5/12/1/2 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_1 (2) | 3 | 0 | 3 |
| /5/12/1/3 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_1 (3) | 3 | 0 | 3 |
| /5/12/1/4 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_2 | 3 | 0 | 3 |
| /5/12/1/5 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_2 (1) | 3 | 0 | 3 |
| /5/12/1/6 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_2 (2) | 3 | 0 | 3 |
| /5/12/1/7 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_2 (3) | 3 | 0 | 3 |
| /5/12/1/8 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_3 | 3 | 0 | 3 |
| /5/12/1/9 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_3 (1) | 3 | 0 | 3 |
| /5/12/1/10 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_3 (2) | 3 | 0 | 3 |
| /5/12/1/11 | -----OldExtra_Assets-----/Potato Chips/Chips/Chip_3 (3) | 3 | 0 | 3 |
| /5/13 | -----OldExtra_Assets-----/Prefab_CustomFog | 1 | 0 | 1 |
| /5/14 | -----OldExtra_Assets-----/RainyArea_v3 | 12 | 0 | 12 |
| /5/14/0 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem | 9 | 0 | 9 |
| /5/14/0/0 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/kosame Audio1 | 1 | 0 | 1 |
| /5/14/0/1 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/kosame Audio2 | 1 | 0 | 1 |
| /5/14/0/2 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/Gouu Audio | 1 | 0 | 1 |
| /5/14/0/3 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/Gouu Audio2 | 1 | 0 | 1 |
| /5/14/0/4 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/IndoorZone　屋内など雨音を小さくしたいエリアを設定 | 1 | 0 | 1 |
| /5/14/0/5 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/Light Rain Player | 1 | 0 | 1 |
| /5/14/0/6 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/Heavy Rain Player | 1 | 0 | 1 |
| /5/14/0/7 | -----OldExtra_Assets-----/RainyArea_v3/RainAudioSystem/WeatherController | 1 | 0 | 1 |
| /5/14/1 | -----OldExtra_Assets-----/RainyArea_v3/RPC　パーティクル数表示用 | 2 | 0 | 2 |
| /5/14/1/0 | -----OldExtra_Assets-----/RainyArea_v3/RPC　パーティクル数表示用/Emission | 1 | 0 | 1 |
| /5/15 | -----OldExtra_Assets-----/ViewTracker2 | 188 | 0 | 188 |
| /5/15/0 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody | 183 | 0 | 183 |
| /5/15/0/0 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody/Body | 1 | 0 | 1 |
| /5/15/0/1 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody/Left | 1 | 0 | 1 |
| /5/15/0/2 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody/Right | 1 | 0 | 1 |
| /5/15/0/3 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody/Display | 1 | 0 | 1 |
| /5/15/0/4 | -----OldExtra_Assets-----/ViewTracker2/ViewTrackerBody/Canvas | 178 | 0 | 178 |
| /5/15/1 | -----OldExtra_Assets-----/ViewTracker2/PlayerViewCapture | 4 | 0 | 4 |
| /5/15/1/0 | -----OldExtra_Assets-----/ViewTracker2/PlayerViewCapture/TPSCamera | 1 | 0 | 1 |
| /5/15/1/1 | -----OldExtra_Assets-----/ViewTracker2/PlayerViewCapture/Playspace | 2 | 0 | 2 |
| /5/16 | -----OldExtra_Assets-----/cooking | 3 | 0 | 3 |
| /5/16/0 | -----OldExtra_Assets-----/cooking/GameObject | 1 | 0 | 1 |
| /5/16/1 | -----OldExtra_Assets-----/cooking/GameObject (1) | 1 | 0 | 1 |
| /5/17 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich | 264 | 0 | 264 |
| /5/17/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_BackScreen | 1 | 0 | 1 |
| /5/17/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Bottom | 1 | 0 | 1 |
| /5/17/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Cabinet | 8 | 0 | 8 |
| /5/17/2/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Cabinet/AT_Cabinet_Dark | 5 | 0 | 5 |
| /5/17/2/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Cabinet/AT_Cabinet_Metal | 1 | 0 | 1 |
| /5/17/2/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Cabinet/AT_Cabinet_Light | 1 | 0 | 1 |
| /5/17/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_CO2cylinder | 4 | 0 | 4 |
| /5/17/3/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_CO2cylinder/Particle | 3 | 0 | 3 |
| /5/17/4 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_DriftWood_01 | 1 | 0 | 1 |
| /5/17/5 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_DriftWood_02 | 1 | 0 | 1 |
| /5/17/6 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Filter | 2 | 0 | 2 |
| /5/17/6/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Filter/Bubble | 1 | 0 | 1 |
| /5/17/7 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight | 18 | 0 | 18 |
| /5/17/7/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight/Cable | 1 | 0 | 1 |
| /5/17/7/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight/Frame | 1 | 0 | 1 |
| /5/17/7/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight/SpotLight | 5 | 0 | 5 |
| /5/17/7/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight/SpotLight (1) | 5 | 0 | 5 |
| /5/17/7/4 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_HanhingLight/SpotLight (2) | 5 | 0 | 5 |
| /5/17/8 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock | 9 | 0 | 9 |
| /5/17/8/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_01 | 1 | 0 | 1 |
| /5/17/8/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_02 | 1 | 0 | 1 |
| /5/17/8/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_03 | 1 | 0 | 1 |
| /5/17/8/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_04 | 1 | 0 | 1 |
| /5/17/8/4 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_05 | 1 | 0 | 1 |
| /5/17/8/5 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_06 | 1 | 0 | 1 |
| /5/17/8/6 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_07 | 1 | 0 | 1 |
| /5/17/8/7 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_Rock/Rock_08 | 1 | 0 | 1 |
| /5/17/9 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_WaterSurface | 1 | 0 | 1 |
| /5/17/10 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/AT_WaterTank | 1 | 0 | 1 |
| /5/17/11 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants | 164 | 0 | 164 |
| /5/17/11/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Anthurium | 1 | 0 | 1 |
| /5/17/11/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/AsianTam | 20 | 0 | 20 |
| /5/17/11/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Bromeliad | 3 | 0 | 3 |
| /5/17/11/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/JewelOrchid | 5 | 0 | 5 |
| /5/17/11/4 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Mashroom | 9 | 0 | 9 |
| /5/17/11/5 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Monstera | 1 | 0 | 1 |
| /5/17/11/6 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Moss | 79 | 0 | 79 |
| /5/17/11/7 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Nepenthes | 1 | 0 | 1 |
| /5/17/11/8 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Pilea | 1 | 0 | 1 |
| /5/17/11/9 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Pinnatifida | 4 | 0 | 4 |
| /5/17/11/10 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/Pothos | 1 | 0 | 1 |
| /5/17/11/11 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/TerrariumPlants/WaterClover | 38 | 0 | 38 |
| /5/17/12 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants | 10 | 0 | 10 |
| /5/17/12/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/TigerLotus | 1 | 0 | 1 |
| /5/17/12/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/TigerLotus (1) | 1 | 0 | 1 |
| /5/17/12/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_A | 1 | 0 | 1 |
| /5/17/12/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_A (1) | 1 | 0 | 1 |
| /5/17/12/4 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_A (2) | 1 | 0 | 1 |
| /5/17/12/5 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_B | 1 | 0 | 1 |
| /5/17/12/6 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_B (1) | 1 | 0 | 1 |
| /5/17/12/7 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_B (2) | 1 | 0 | 1 |
| /5/17/12/8 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/WaterPlants/Microsorum_B (3) | 1 | 0 | 1 |
| /5/17/13 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/FishSchool | 39 | 0 | 39 |
| /5/17/13/0 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/FishSchool/FishSchool_RummyNose | 11 | 0 | 11 |
| /5/17/13/1 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/FishSchool/FishSchool_CardinalTetra | 21 | 0 | 21 |
| /5/17/13/2 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/FishSchool/FishSchool_NeonDwarfGourami | 4 | 0 | 4 |
| /5/17/13/3 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/FishSchool/FishSchool_Sacabambaspis | 2 | 0 | 2 |
| /5/17/14 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/Directional Light_WaterSurface | 1 | 0 | 1 |
| /5/17/15 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/Light Probe Group | 1 | 0 | 1 |
| /5/17/16 | -----OldExtra_Assets-----/AquaTerrarium_PC_Rich/SlowSpeedArea | 1 | 0 | 1 |
| /5/18 | -----OldExtra_Assets-----/VirtualCalendar | 166 | 0 | 166 |
| /5/18/0 | -----OldExtra_Assets-----/VirtualCalendar/Calendar | 165 | 0 | 165 |
| /5/18/0/0 | -----OldExtra_Assets-----/VirtualCalendar/Calendar/Canvas | 164 | 0 | 164 |
| /5/19 | -----OldExtra_Assets-----/CashBlaster_Set | 128 | 0 | 128 |
| /5/19/0 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster-------------------------------------- | 101 | 0 | 101 |
| /5/19/0/0 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster--------------------------------------/CashBlaster_1 | 20 | 0 | 20 |
| /5/19/0/1 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster--------------------------------------/CashBlaster_2 | 20 | 0 | 20 |
| /5/19/0/2 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster--------------------------------------/CashBlaster_3 | 20 | 0 | 20 |
| /5/19/0/3 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster--------------------------------------/CashBlaster_4 | 20 | 0 | 20 |
| /5/19/0/4 | -----OldExtra_Assets-----/CashBlaster_Set/------CashBlaster--------------------------------------/CashBlaster_5 | 20 | 0 | 20 |
| /5/19/1 | -----OldExtra_Assets-----/CashBlaster_Set/------GunRestrictedArea(Don't Change Name)------ | 2 | 0 | 2 |
| /5/19/1/0 | -----OldExtra_Assets-----/CashBlaster_Set/------GunRestrictedArea(Don't Change Name)------/Gun_RestrictedArea | 1 | 0 | 1 |
| /5/19/2 | -----OldExtra_Assets-----/CashBlaster_Set/------Target--------------------------------------------- | 22 | 0 | 22 |
| /5/19/2/0 | -----OldExtra_Assets-----/CashBlaster_Set/------Target---------------------------------------------/MoneyTarget_OneShot | 4 | 0 | 4 |
| /5/19/2/1 | -----OldExtra_Assets-----/CashBlaster_Set/------Target---------------------------------------------/MoneyTarget_Recovery | 8 | 0 | 8 |
| /5/19/2/2 | -----OldExtra_Assets-----/CashBlaster_Set/------Target---------------------------------------------/MoneyTarget_Triple | 9 | 0 | 9 |
| /5/19/3 | -----OldExtra_Assets-----/CashBlaster_Set/------SpawnArea(Don't Change Name)-------------- | 2 | 0 | 2 |
| /5/19/3/0 | -----OldExtra_Assets-----/CashBlaster_Set/------SpawnArea(Don't Change Name)--------------/Target_SpawnArea | 1 | 0 | 1 |
| /5/20 | -----OldExtra_Assets-----/VRCTV-Timetable | 1 | 0 | 1 |
| /5/21 | -----OldExtra_Assets-----/BoatV2Set | 39 | 0 | 39 |
| /5/21/0 | -----OldExtra_Assets-----/BoatV2Set/BoatV2 | 33 | 0 | 33 |
| /5/21/0/0 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/OperatorSeat | 3 | 0 | 3 |
| /5/21/0/1 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/Mesh | 17 | 0 | 17 |
| /5/21/0/2 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/Colliders | 1 | 0 | 1 |
| /5/21/0/3 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/Sounds | 5 | 0 | 5 |
| /5/21/0/4 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/#Enter | 1 | 0 | 1 |
| /5/21/0/5 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/Exit | 1 | 0 | 1 |
| /5/21/0/6 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/#FixedAtWaterLevel | 1 | 0 | 1 |
| /5/21/0/7 | -----OldExtra_Assets-----/BoatV2Set/BoatV2/Particles | 3 | 0 | 3 |
| /5/21/1 | -----OldExtra_Assets-----/BoatV2Set/FixedAtWaterLevelChild | 2 | 0 | 2 |
| /5/21/1/0 | -----OldExtra_Assets-----/BoatV2Set/FixedAtWaterLevelChild/Foam | 1 | 0 | 1 |
| /5/21/2 | -----OldExtra_Assets-----/BoatV2Set/FlagTarget | 1 | 0 | 1 |
| /5/21/3 | -----OldExtra_Assets-----/BoatV2Set/BoatRespawnButton | 2 | 0 | 2 |
| /5/21/3/0 | -----OldExtra_Assets-----/BoatV2Set/BoatRespawnButton/Cube | 1 | 0 | 1 |
| /5/22 | -----OldExtra_Assets-----/OldFashionedBoatSet | 50 | 0 | 50 |
| /5/22/0 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat | 45 | 0 | 45 |
| /5/22/0/0 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/OperatorSeat | 4 | 0 | 4 |
| /5/22/0/1 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/Mesh | 12 | 0 | 12 |
| /5/22/0/2 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/Colliders | 1 | 0 | 1 |
| /5/22/0/3 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/Sounds | 5 | 0 | 5 |
| /5/22/0/4 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/#FixedAtWaterLevel | 1 | 0 | 1 |
| /5/22/0/5 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/Particles | 3 | 0 | 3 |
| /5/22/0/6 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/Exit | 1 | 0 | 1 |
| /5/22/0/7 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/LeftHand | 1 | 0 | 1 |
| /5/22/0/8 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/#OperatorEyeLevel | 1 | 0 | 1 |
| /5/22/0/9 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/GuestSit (1) | 3 | 0 | 3 |
| /5/22/0/10 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/GuestSit (2) | 3 | 0 | 3 |
| /5/22/0/11 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/GuestSit (3) | 3 | 0 | 3 |
| /5/22/0/12 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/GuestSit (4) | 3 | 0 | 3 |
| /5/22/0/13 | -----OldExtra_Assets-----/OldFashionedBoatSet/OldFashionedBoat/GuestSit (5) | 3 | 0 | 3 |
| /5/22/1 | -----OldExtra_Assets-----/OldFashionedBoatSet/FixedAtWaterLevelChild | 2 | 0 | 2 |
| /5/22/1/0 | -----OldExtra_Assets-----/OldFashionedBoatSet/FixedAtWaterLevelChild/Foam | 1 | 0 | 1 |
| /5/22/2 | -----OldExtra_Assets-----/OldFashionedBoatSet/BoatRespawnButton | 2 | 0 | 2 |
| /5/22/2/0 | -----OldExtra_Assets-----/OldFashionedBoatSet/BoatRespawnButton/Cube | 1 | 0 | 1 |
| /5/23 | -----OldExtra_Assets-----/Basic | 10 | 0 | 10 |
| /5/23/0 | -----OldExtra_Assets-----/Basic/Offset | 6 | 0 | 6 |
| /5/23/0/0 | -----OldExtra_Assets-----/Basic/Offset/Canvas | 5 | 0 | 5 |
| /5/23/1 | -----OldExtra_Assets-----/Basic/Sounds | 3 | 0 | 3 |
| /5/23/1/0 | -----OldExtra_Assets-----/Basic/Sounds/Join | 1 | 0 | 1 |
| /5/23/1/1 | -----OldExtra_Assets-----/Basic/Sounds/Leave | 1 | 0 | 1 |
| /5/24 | -----OldExtra_Assets-----/VVMW (On-Screen Controls) | 204 | 0 | 204 |
| /5/24/0 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/AVPro Module | 1 | 0 | 1 |
| /5/24/1 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Builtin Module | 1 | 0 | 1 |
| /5/24/2 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Image Module | 1 | 0 | 1 |
| /5/24/3 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Playlist Queue Handler | 1 | 0 | 1 |
| /5/24/4 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Locale | 1 | 0 | 1 |
| /5/24/5 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Active Region Manager | 1 | 0 | 1 |
| /5/24/6 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Rate Limit Resolver | 1 | 0 | 1 |
| /5/24/7 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Default Audio Source | 1 | 0 | 1 |
| /5/24/8 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Screen With Overlay | 195 | 0 | 195 |
| /5/24/8/0 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Screen With Overlay/Screen | 1 | 0 | 1 |
| /5/24/8/1 | -----OldExtra_Assets-----/VVMW (On-Screen Controls)/Screen With Overlay/MainUI | 193 | 0 | 193 |
| /5/25 | -----OldExtra_Assets-----/MaterialBrush | 15 | 0 | 15 |
| /5/25/0 | -----OldExtra_Assets-----/MaterialBrush/ParticleEmission_Change | 1 | 0 | 1 |
| /5/25/1 | -----OldExtra_Assets-----/MaterialBrush/AudioSource | 4 | 0 | 4 |
| /5/25/1/0 | -----OldExtra_Assets-----/MaterialBrush/AudioSource/Change | 1 | 0 | 1 |
| /5/25/1/1 | -----OldExtra_Assets-----/MaterialBrush/AudioSource/Click | 1 | 0 | 1 |
| /5/25/1/2 | -----OldExtra_Assets-----/MaterialBrush/AudioSource/ClickChange | 1 | 0 | 1 |
| /5/25/2 | -----OldExtra_Assets-----/MaterialBrush/Mesh | 6 | 0 | 6 |
| /5/25/2/0 | -----OldExtra_Assets-----/MaterialBrush/Mesh/Hake | 1 | 0 | 1 |
| /5/25/2/1 | -----OldExtra_Assets-----/MaterialBrush/Mesh/Hake_Brush | 1 | 0 | 1 |
| /5/25/2/2 | -----OldExtra_Assets-----/MaterialBrush/Mesh/pipette_top | 1 | 0 | 1 |
| /5/25/2/3 | -----OldExtra_Assets-----/MaterialBrush/Mesh/pipette_Glass | 1 | 0 | 1 |
| /5/25/2/4 | -----OldExtra_Assets-----/MaterialBrush/Mesh/pipette_GlassOuter | 1 | 0 | 1 |
| /5/25/3 | -----OldExtra_Assets-----/MaterialBrush/Trigger | 3 | 0 | 3 |
| /5/25/3/0 | -----OldExtra_Assets-----/MaterialBrush/Trigger/Hake_Brush_Trigger | 1 | 0 | 1 |
| /5/25/3/1 | -----OldExtra_Assets-----/MaterialBrush/Trigger/pipette_Glass_Trigger | 1 | 0 | 1 |
| /5/26 | -----OldExtra_Assets-----/MaterialResetter | 4 | 0 | 4 |
| /5/26/0 | -----OldExtra_Assets-----/MaterialResetter/Switch_Base | 1 | 0 | 1 |
| /5/26/1 | -----OldExtra_Assets-----/MaterialResetter/Switch_Return | 1 | 0 | 1 |
| /5/26/2 | -----OldExtra_Assets-----/MaterialResetter/Switch_Button | 1 | 0 | 1 |
| /5/27 | -----OldExtra_Assets-----/UdonKartSet | 62 | 0 | 62 |
| /5/27/0 | -----OldExtra_Assets-----/UdonKartSet/UdonKart | 56 | 0 | 56 |
| /5/27/0/0 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/Wheel | 5 | 0 | 5 |
| /5/27/0/1 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/UdonKart | 15 | 0 | 15 |
| /5/27/0/2 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/Seat | 3 | 0 | 3 |
| /5/27/0/3 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/EnterStation | 1 | 0 | 1 |
| /5/27/0/4 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/ExitStation | 1 | 0 | 1 |
| /5/27/0/5 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/DisplayWindow | 4 | 0 | 4 |
| /5/27/0/6 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/SettingWindow | 20 | 0 | 20 |
| /5/27/0/7 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/ExitCube | 3 | 0 | 3 |
| /5/27/0/8 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/TimeAttacker | 1 | 0 | 1 |
| /5/27/0/9 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/StateHolder | 1 | 0 | 1 |
| /5/27/0/10 | -----OldExtra_Assets-----/UdonKartSet/UdonKart/WheelGuard | 1 | 0 | 1 |
| /5/27/1 | -----OldExtra_Assets-----/UdonKartSet/ResetButton | 5 | 0 | 5 |
| /5/27/1/0 | -----OldExtra_Assets-----/UdonKartSet/ResetButton/Free | 2 | 0 | 2 |
| /5/27/1/1 | -----OldExtra_Assets-----/UdonKartSet/ResetButton/Occupied | 2 | 0 | 2 |
| /5/28 | -----OldExtra_Assets-----/ChipsExchange | 66 | 0 | 66 |
| /5/28/0 | -----OldExtra_Assets-----/ChipsExchange/ModeSwitch_Chips | 36 | 0 | 36 |
| /5/28/0/0 | -----OldExtra_Assets-----/ChipsExchange/ModeSwitch_Chips/Switch_Root | 35 | 0 | 35 |
| /5/28/1 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips | 29 | 0 | 29 |
| /5/28/1/0 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips/====TargetSetting==== | 1 | 0 | 1 |
| /5/28/1/1 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips/Slider_2DMode | 11 | 0 | 11 |
| /5/28/1/2 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips/Slider_3DMode | 9 | 0 | 9 |
| /5/28/1/3 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips/Slider_System | 3 | 0 | 3 |
| /5/28/1/4 | -----OldExtra_Assets-----/ChipsExchange/Slider_ExchangeChips/ObjectTarget | 4 | 0 | 4 |
| /5/29 | -----OldExtra_Assets-----/N_UdonGameChips | 1 | 0 | 1 |
| /5/30 | -----OldExtra_Assets-----/UMoffPen2Package | 433 | 0 | 433 |
| /5/30/0 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2 | 6 | 0 | 6 |
| /5/30/0/0 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2/[DO_NOT_TOUCH] | 5 | 0 | 5 |
| /5/30/1 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2Sys[DO_NOT_DISABLE_OR_SCALE] | 426 | 0 | 426 |
| /5/30/1/0 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2Sys[DO_NOT_DISABLE_OR_SCALE]/Settings | 1 | 0 | 1 |
| /5/30/1/1 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2Sys[DO_NOT_DISABLE_OR_SCALE]/UIThemeTool | 1 | 0 | 1 |
| /5/30/1/2 | -----OldExtra_Assets-----/UMoffPen2Package/UMoffPen2Sys[DO_NOT_DISABLE_OR_SCALE]/[DO_NOT_TOUCH] | 423 | 0 | 423 |
| /6 | GARAGE | 104 | 0 | 104 |
| /6/0 | GARAGE/R | 1 | 0 | 1 |
| /6/1 | GARAGE/Lighting | 8 | 0 | 8 |
| /6/1/0 | GARAGE/Lighting/Directional Light | 1 | 0 | 1 |
| /6/1/1 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/1/2 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/1/3 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/1/4 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/1/5 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/1/6 | GARAGE/Lighting/Area Light | 1 | 0 | 1 |
| /6/2 | GARAGE/ベース | 52 | 0 | 52 |
| /6/2/0 | GARAGE/ベース/ガラス | 1 | 0 | 1 |
| /6/2/1 | GARAGE/ベース/可動しないガラス | 1 | 0 | 1 |
| /6/2/2 | GARAGE/ベース/コンセント | 1 | 0 | 1 |
| /6/2/3 | GARAGE/ベース/H型鉄骨 | 1 | 0 | 1 |
| /6/2/4 | GARAGE/ベース/H型鉄骨 | 1 | 0 | 1 |
| /6/2/5 | GARAGE/ベース/H型鉄骨 | 1 | 0 | 1 |
| /6/2/6 | GARAGE/ベース/H型鉄骨 | 1 | 0 | 1 |
| /6/2/7 | GARAGE/ベース/蛍光灯 | 8 | 0 | 8 |
| /6/2/7/0 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/1 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/2 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/3 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/4 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/5 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/7/6 | GARAGE/ベース/蛍光灯/Spot Light | 1 | 0 | 1 |
| /6/2/8 | GARAGE/ベース/ガレージ がらがら | 1 | 0 | 1 |
| /6/2/9 | GARAGE/ベース/ガレージ 扉 枠 | 1 | 0 | 1 |
| /6/2/10 | GARAGE/ベース/コンセント | 1 | 0 | 1 |
| /6/2/11 | GARAGE/ベース/コンセント | 1 | 0 | 1 |
| /6/2/12 | GARAGE/ベース/コンセント | 1 | 0 | 1 |
| /6/2/13 | GARAGE/ベース/固定具 | 1 | 0 | 1 |
| /6/2/14 | GARAGE/ベース/固定具 | 1 | 0 | 1 |
| /6/2/15 | GARAGE/ベース/固定具 | 1 | 0 | 1 |
| /6/2/16 | GARAGE/ベース/壁 | 1 | 0 | 1 |
| /6/2/17 | GARAGE/ベース/天井 あみあみ | 1 | 0 | 1 |
| /6/2/18 | GARAGE/ベース/天井 あみあみ 枠 | 1 | 0 | 1 |
| /6/2/19 | GARAGE/ベース/天井 あみあみ 留め具 | 1 | 0 | 1 |
| /6/2/20 | GARAGE/ベース/壁 とたん | 1 | 0 | 1 |
| /6/2/21 | GARAGE/ベース/床・壁・天井 | 1 | 0 | 1 |
| /6/2/22 | GARAGE/ベース/窓枠 | 1 | 0 | 1 |
| /6/2/23 | GARAGE/ベース/ロールカーテン | 1 | 0 | 1 |
| /6/2/24 | GARAGE/ベース/ロールカーテン | 1 | 0 | 1 |
| /6/2/25 | GARAGE/ベース/補強板.002 | 1 | 0 | 1 |
| /6/2/26 | GARAGE/ベース/補強板.003 | 1 | 0 | 1 |
| /6/2/27 | GARAGE/ベース/補強板.005 | 1 | 0 | 1 |
| /6/2/28 | GARAGE/ベース/補強板.006 | 1 | 0 | 1 |
| /6/2/29 | GARAGE/ベース/配電ケーブル固定具 | 1 | 0 | 1 |
| /6/2/30 | GARAGE/ベース/配電ケーブル端子 | 1 | 0 | 1 |
| /6/2/31 | GARAGE/ベース/配電盤 固定具  | 1 | 0 | 1 |
| /6/2/32 | GARAGE/ベース/床・壁・天井.001 | 1 | 0 | 1 |
| /6/2/33 | GARAGE/ベース/H型鉄骨.004 | 1 | 0 | 1 |
| /6/2/34 | GARAGE/ベース/NVコンセント | 1 | 0 | 1 |
| /6/2/35 | GARAGE/ベース/NVコンセント | 1 | 0 | 1 |
| /6/2/36 | GARAGE/ベース/蛍光灯 ケーブル | 1 | 0 | 1 |
| /6/2/37 | GARAGE/ベース/配電ケーブル | 1 | 0 | 1 |
| /6/2/38 | GARAGE/ベース/配電盤 中 | 1 | 0 | 1 |
| /6/2/39 | GARAGE/ベース/配電盤 大 | 1 | 0 | 1 |
| /6/2/40 | GARAGE/ベース/配電盤 小 | 1 | 0 | 1 |
| /6/2/41 | GARAGE/ベース/配電盤 小 | 1 | 0 | 1 |
| /6/2/42 | GARAGE/ベース/配電盤 小 | 1 | 0 | 1 |
| /6/2/43 | GARAGE/ベース/ガレージ がらがら スイッチ | 1 | 0 | 1 |
| /6/3 | GARAGE/MINI NV BOX | 9 | 0 | 9 |
| /6/3/0 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/1 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/2 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/3 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/4 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/5 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/6 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/3/7 | GARAGE/MINI NV BOX/MINI NV BOX | 1 | 0 | 1 |
| /6/4 | GARAGE/NV BOX | 13 | 0 | 13 |
| /6/4/0 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/1 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/2 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/3 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/4 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/5 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/6 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/7 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/8 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/9 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/10 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/4/11 | GARAGE/NV BOX/NV BOX | 1 | 0 | 1 |
| /6/5 | GARAGE/NV蛍光灯 床起き | 4 | 0 | 4 |
| /6/5/0 | GARAGE/NV蛍光灯 床起き/NV蛍光灯 | 1 | 0 | 1 |
| /6/5/1 | GARAGE/NV蛍光灯 床起き/NV蛍光灯ガラス | 1 | 0 | 1 |
| /6/5/2 | GARAGE/NV蛍光灯 床起き/Point Light | 1 | 0 | 1 |
| /6/6 | GARAGE/STEEL RACK 壁用 | 4 | 0 | 4 |
| /6/6/0 | GARAGE/STEEL RACK 壁用/STEEL RACK 壁用 | 1 | 0 | 1 |
| /6/6/1 | GARAGE/STEEL RACK 壁用/STEEL RACK 壁用 | 1 | 0 | 1 |
| /6/6/2 | GARAGE/STEEL RACK 壁用/STEEL RACK 壁用 | 1 | 0 | 1 |
| /6/7 | GARAGE/STEEL RACK | 8 | 0 | 8 |
| /6/7/0 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/1 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/2 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/3 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/4 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/5 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/7/6 | GARAGE/STEEL RACK/STEEL RACK | 1 | 0 | 1 |
| /6/8 | GARAGE/靴用 棚 | 3 | 0 | 3 |
| /6/8/0 | GARAGE/靴用 棚/靴用 棚 | 1 | 0 | 1 |
| /6/8/1 | GARAGE/靴用 棚/靴用 棚 | 1 | 0 | 1 |
| /6/9 | GARAGE/レコード BOX | 1 | 0 | 1 |
| /7 | nadena.dev.ndmf__Activator | 1 | 1 | 0 |
| /8 | N.Console | 112 | 0 | 112 |
| /8/0 | N.Console/KeyBoard | 91 | 0 | 91 |
| /8/0/0 | N.Console/KeyBoard/Canvas_Output | 4 | 0 | 4 |
| /8/0/0/0 | N.Console/KeyBoard/Canvas_Output/InputField | 3 | 0 | 3 |
| /8/0/1 | N.Console/KeyBoard/Canvas_Input | 74 | 0 | 74 |
| /8/0/1/0 | N.Console/KeyBoard/Canvas_Input/Background | 1 | 0 | 1 |
| /8/0/1/1 | N.Console/KeyBoard/Canvas_Input/EventTrigger | 71 | 0 | 71 |
| /8/0/1/2 | N.Console/KeyBoard/Canvas_Input/Blocker | 1 | 0 | 1 |
| /8/0/2 | N.Console/KeyBoard/Mesh | 8 | 0 | 8 |
| /8/0/2/0 | N.Console/KeyBoard/Mesh/keyboard | 6 | 0 | 6 |
| /8/0/2/1 | N.Console/KeyBoard/Mesh/LOD_1 | 1 | 0 | 1 |
| /8/0/3 | N.Console/KeyBoard/Bureau | 3 | 0 | 3 |
| /8/0/3/0 | N.Console/KeyBoard/Bureau/EventSystem | 1 | 0 | 1 |
| /8/0/3/1 | N.Console/KeyBoard/Bureau/StringHolder | 1 | 0 | 1 |
| /8/0/4 | N.Console/KeyBoard/Handle | 1 | 0 | 1 |
| /8/1 | N.Console/DEMO | 20 | 0 | 20 |
| /8/1/0 | N.Console/DEMO/DEMO_PasswordEvent | 5 | 0 | 5 |
| /8/1/0/0 | N.Console/DEMO/DEMO_PasswordEvent/Cube | 1 | 0 | 1 |
| /8/1/0/1 | N.Console/DEMO/DEMO_PasswordEvent/Sphere | 1 | 0 | 1 |
| /8/1/0/2 | N.Console/DEMO/DEMO_PasswordEvent/Capsule | 1 | 0 | 1 |
| /8/1/0/3 | N.Console/DEMO/DEMO_PasswordEvent/Cylinder | 1 | 0 | 1 |
| /8/1/1 | N.Console/DEMO/DEMO_Command | 1 | 0 | 1 |
| /8/1/2 | N.Console/DEMO/DEMO_Chat | 1 | 0 | 1 |
| /8/1/3 | N.Console/DEMO/Canvas_DEMO | 12 | 0 | 12 |
| /8/1/3/0 | N.Console/DEMO/Canvas_DEMO/Scroll View | 8 | 0 | 8 |
| /8/1/3/1 | N.Console/DEMO/Canvas_DEMO/InputField | 3 | 0 | 3 |
| /9 | Experimentals_Weapons | 5121 | 0 | 5121 |
| /9/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black | 250 | 0 | 250 |
| /9/0/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/MODEL | 85 | 0 | 85 |
| /9/0/0/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/MODEL/Gun | 66 | 0 | 66 |
| /9/0/0/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/MODEL/Load | 18 | 0 | 18 |
| /9/0/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/SE | 18 | 0 | 18 |
| /9/0/1/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/SE/Gun | 11 | 0 | 11 |
| /9/0/1/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/SE/Shot | 6 | 0 | 6 |
| /9/0/2 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/PARTICLE_EFFECT | 101 | 0 | 101 |
| /9/0/2/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/PARTICLE_EFFECT/Shot | 45 | 0 | 45 |
| /9/0/2/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/PARTICLE_EFFECT/Cylinder | 55 | 0 | 55 |
| /9/0/3 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/CONST_SETTING | 28 | 0 | 28 |
| /9/0/3/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/CONST_SETTING/CONST_PARENT | 20 | 0 | 20 |
| /9/0/3/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/CONST_SETTING/CONST_GUNCHILD | 7 | 0 | 7 |
| /9/0/4 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/DAGs Bastionメニュー | 17 | 0 | 17 |
| /9/0/4/0 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/DAGs Bastionメニュー/セレクター | 3 | 0 | 3 |
| /9/0/4/1 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/DAGs Bastionメニュー/設定 | 9 | 0 | 9 |
| /9/0/4/2 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/DAGs Bastionメニュー/リロード方式 | 3 | 0 | 3 |
| /9/0/4/3 | Experimentals_Weapons/DAGsRB01_629Bastion_MA_General_Black/DAGs Bastionメニュー/ワールド固定 | 1 | 0 | 1 |
| /9/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black | 275 | 0 | 275 |
| /9/1/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/MODEL | 105 | 0 | 105 |
| /9/1/0/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/MODEL/Gun | 72 | 0 | 72 |
| /9/1/0/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/MODEL/Load | 19 | 0 | 19 |
| /9/1/0/2 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/MODEL/Load_Set | 13 | 0 | 13 |
| /9/1/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE | 23 | 0 | 23 |
| /9/1/1/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Shot | 3 | 0 | 3 |
| /9/1/1/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Ejection | 3 | 0 | 3 |
| /9/1/1/2 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Magazin | 3 | 0 | 3 |
| /9/1/1/3 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Slide | 4 | 0 | 4 |
| /9/1/1/4 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Trigger | 2 | 0 | 2 |
| /9/1/1/5 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/Attachment | 5 | 0 | 5 |
| /9/1/1/6 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/SE/TakePut | 2 | 0 | 2 |
| /9/1/2 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/PARTICLE_EFFECT | 83 | 0 | 83 |
| /9/1/2/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/PARTICLE_EFFECT/Shot | 64 | 0 | 64 |
| /9/1/2/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/PARTICLE_EFFECT/Ejection | 14 | 0 | 14 |
| /9/1/2/2 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/PARTICLE_EFFECT/Magazin | 4 | 0 | 4 |
| /9/1/3 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/CONST_SETTING | 41 | 0 | 41 |
| /9/1/3/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/CONST_SETTING/CONST_PARENT | 19 | 0 | 19 |
| /9/1/3/1 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/CONST_SETTING/CONST_CHILD | 21 | 0 | 21 |
| /9/1/4 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/EX_MENU_jp | 22 | 0 | 22 |
| /9/1/4/0 | Experimentals_Weapons/DAGsSR01_E24Sentinel_MA_Black/EX_MENU_jp/DAGs E24Sentinel メニュー | 21 | 0 | 21 |
| /9/2 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black | 288 | 0 | 288 |
| /9/2/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/MODEL | 81 | 0 | 81 |
| /9/2/0/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/MODEL/Gun | 64 | 0 | 64 |
| /9/2/0/1 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/MODEL/Load | 8 | 0 | 8 |
| /9/2/0/2 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/MODEL/Load_Set | 8 | 0 | 8 |
| /9/2/1 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE | 30 | 0 | 30 |
| /9/2/1/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/Shot | 14 | 0 | 14 |
| /9/2/1/1 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/Magazin | 1 | 0 | 1 |
| /9/2/1/2 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/Slide | 4 | 0 | 4 |
| /9/2/1/3 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/Trigger | 3 | 0 | 3 |
| /9/2/1/4 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/Stock | 3 | 0 | 3 |
| /9/2/1/5 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/SnapShot | 3 | 0 | 3 |
| /9/2/1/6 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/SE/TakePut | 1 | 0 | 1 |
| /9/2/2 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/PARTICLE_EFFECT | 107 | 0 | 107 |
| /9/2/2/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/PARTICLE_EFFECT/Shot | 91 | 0 | 91 |
| /9/2/2/1 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/PARTICLE_EFFECT/Ejection | 12 | 0 | 12 |
| /9/2/2/2 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/PARTICLE_EFFECT/Magazin | 3 | 0 | 3 |
| /9/2/3 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/CONST_SETTING | 45 | 0 | 45 |
| /9/2/3/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/CONST_SETTING/CONST_PARENT | 17 | 0 | 17 |
| /9/2/3/1 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/CONST_SETTING/CONST_CHILD | 27 | 0 | 27 |
| /9/2/4 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/EX_MENU_jp | 24 | 0 | 24 |
| /9/2/4/0 | Experimentals_Weapons/DAGsSMG01_LB5Liberator_Black/EX_MENU_jp/DAGs LB5L メニュー | 23 | 0 | 23 |
| /9/3 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black | 342 | 0 | 342 |
| /9/3/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/MODEL | 171 | 0 | 171 |
| /9/3/0/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/MODEL/Gun | 136 | 0 | 136 |
| /9/3/0/1 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/MODEL/Shotshell | 34 | 0 | 34 |
| /9/3/1 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/SE | 23 | 0 | 23 |
| /9/3/1/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/SE/Shot | 4 | 0 | 4 |
| /9/3/1/1 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/SE/Magazin | 7 | 0 | 7 |
| /9/3/1/2 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/SE/Slide | 7 | 0 | 7 |
| /9/3/1/3 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/SE/Trigger | 4 | 0 | 4 |
| /9/3/2 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/PARTICLE_EFFECT | 93 | 0 | 93 |
| /9/3/2/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/PARTICLE_EFFECT/Shot | 41 | 0 | 41 |
| /9/3/2/1 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/PARTICLE_EFFECT/Ejection | 51 | 0 | 51 |
| /9/3/3 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/CONST_SETTING | 31 | 0 | 31 |
| /9/3/3/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/CONST_SETTING/CONST_PARENT | 16 | 0 | 16 |
| /9/3/3/1 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/CONST_SETTING/CONST_CHILD | 14 | 0 | 14 |
| /9/3/4 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/EX_MENU_jp | 23 | 0 | 23 |
| /9/3/4/0 | Experimentals_Weapons/DAGsSG01_SGX870_MA_General_Black/EX_MENU_jp/DAGs SGX870メニュー | 22 | 0 | 22 |
| /9/4 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General | 205 | 0 | 205 |
| /9/4/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/MODEL | 47 | 0 | 47 |
| /9/4/0/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/MODEL/Gun | 34 | 0 | 34 |
| /9/4/0/1 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/MODEL/Magazin | 12 | 0 | 12 |
| /9/4/1 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/SE | 36 | 0 | 36 |
| /9/4/1/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/SE/Shot | 11 | 0 | 11 |
| /9/4/1/1 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/SE/Magazin | 7 | 0 | 7 |
| /9/4/1/2 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/SE/Slide | 13 | 0 | 13 |
| /9/4/1/3 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/SE/Trigger | 4 | 0 | 4 |
| /9/4/2 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/PARTICLE_EFFECT | 65 | 0 | 65 |
| /9/4/2/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/PARTICLE_EFFECT/Shot | 50 | 0 | 50 |
| /9/4/2/1 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/PARTICLE_EFFECT/Ejection | 11 | 0 | 11 |
| /9/4/2/2 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/PARTICLE_EFFECT/Magazin | 3 | 0 | 3 |
| /9/4/3 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/CONST_SETTING | 36 | 0 | 36 |
| /9/4/3/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/CONST_SETTING/CONST_PARENT | 15 | 0 | 15 |
| /9/4/3/1 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/CONST_SETTING/CONST_CHILD | 20 | 0 | 20 |
| /9/4/4 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/EX_MENU_v2_jp | 20 | 0 | 20 |
| /9/4/4/0 | Experimentals_Weapons/DAGsHG02_v2_M9A1_MA_General/EX_MENU_v2_jp/DAGs M9A1メニュー | 19 | 0 | 19 |
| /9/5 | Experimentals_Weapons/DAGsAR01_US416_MA_General | 303 | 0 | 303 |
| /9/5/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/MODEL | 126 | 0 | 126 |
| /9/5/0/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/MODEL/Gun | 78 | 0 | 78 |
| /9/5/0/1 | Experimentals_Weapons/DAGsAR01_US416_MA_General/MODEL/Magazin | 28 | 0 | 28 |
| /9/5/0/2 | Experimentals_Weapons/DAGsAR01_US416_MA_General/MODEL/Magazin_Set | 19 | 0 | 19 |
| /9/5/1 | Experimentals_Weapons/DAGsAR01_US416_MA_General/SE | 33 | 0 | 33 |
| /9/5/1/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/SE/Shot | 11 | 0 | 11 |
| /9/5/1/1 | Experimentals_Weapons/DAGsAR01_US416_MA_General/SE/Magazin | 7 | 0 | 7 |
| /9/5/1/2 | Experimentals_Weapons/DAGsAR01_US416_MA_General/SE/Slide | 10 | 0 | 10 |
| /9/5/1/3 | Experimentals_Weapons/DAGsAR01_US416_MA_General/SE/Trigger | 4 | 0 | 4 |
| /9/5/2 | Experimentals_Weapons/DAGsAR01_US416_MA_General/PARTICLE_EFFECT | 85 | 0 | 85 |
| /9/5/2/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/PARTICLE_EFFECT/Shot | 68 | 0 | 68 |
| /9/5/2/1 | Experimentals_Weapons/DAGsAR01_US416_MA_General/PARTICLE_EFFECT/Ejection | 13 | 0 | 13 |
| /9/5/2/2 | Experimentals_Weapons/DAGsAR01_US416_MA_General/PARTICLE_EFFECT/Magazin | 3 | 0 | 3 |
| /9/5/3 | Experimentals_Weapons/DAGsAR01_US416_MA_General/CONST_SETTING | 33 | 0 | 33 |
| /9/5/3/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/CONST_SETTING/CONST_PARENT | 16 | 0 | 16 |
| /9/5/3/1 | Experimentals_Weapons/DAGsAR01_US416_MA_General/CONST_SETTING/CONST_CHILD | 16 | 0 | 16 |
| /9/5/4 | Experimentals_Weapons/DAGsAR01_US416_MA_General/EX_MENU_jp | 25 | 0 | 25 |
| /9/5/4/0 | Experimentals_Weapons/DAGsAR01_US416_MA_General/EX_MENU_jp/DAGs US416メニュー | 24 | 0 | 24 |
| /9/6 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black | 253 | 0 | 253 |
| /9/6/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/MODEL | 79 | 0 | 79 |
| /9/6/0/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/MODEL/Gun | 53 | 0 | 53 |
| /9/6/0/1 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/MODEL/Load | 17 | 0 | 17 |
| /9/6/0/2 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/MODEL/Load_Set | 8 | 0 | 8 |
| /9/6/1 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE | 47 | 0 | 47 |
| /9/6/1/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/Shot | 9 | 0 | 9 |
| /9/6/1/1 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/Magazin | 7 | 0 | 7 |
| /9/6/1/2 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/Slide | 10 | 0 | 10 |
| /9/6/1/3 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/Trigger | 4 | 0 | 4 |
| /9/6/1/4 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/Attachment | 13 | 0 | 13 |
| /9/6/1/5 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/SE/TakePut | 3 | 0 | 3 |
| /9/6/2 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/PARTICLE_EFFECT | 68 | 0 | 68 |
| /9/6/2/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/PARTICLE_EFFECT/Shot | 53 | 0 | 53 |
| /9/6/2/1 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/PARTICLE_EFFECT/Ejection | 11 | 0 | 11 |
| /9/6/2/2 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/PARTICLE_EFFECT/Magazin | 3 | 0 | 3 |
| /9/6/3 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/CONST_SETTING | 36 | 0 | 36 |
| /9/6/3/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/CONST_SETTING/CONST_PARENT | 15 | 0 | 15 |
| /9/6/3/1 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/CONST_SETTING/CONST_CHILD | 20 | 0 | 20 |
| /9/6/4 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/EX_MENU_jp | 22 | 0 | 22 |
| /9/6/4/0 | Experimentals_Weapons/DAGsHG03_VS9Phantom_MA_Black/EX_MENU_jp/DAGs VS9P メニュー | 21 | 0 | 21 |
| /9/7 | Experimentals_Weapons/ZAG_ARAGAMI | 294 | 0 | 294 |
| /9/7/0 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R | 293 | 0 | 293 |
| /9/7/0/0 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R/ZAG_Aragami_body | 30 | 0 | 30 |
| /9/7/0/1 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R/ZAG_Parentset_R | 6 | 0 | 6 |
| /9/7/0/2 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R/ZAG_Contactset_R | 3 | 0 | 3 |
| /9/7/0/3 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R/ZAG_Effect_R | 98 | 0 | 98 |
| /9/7/0/4 | Experimentals_Weapons/ZAG_ARAGAMI/ZAG_Aragami_R/位置決めオブジェクト(アップロードされません) | 155 | 0 | 155 |
| /9/8 | Experimentals_Weapons/ZBM_BellowMaker_System_C01 | 237 | 0 | 237 |
| /9/8/0 | Experimentals_Weapons/ZBM_BellowMaker_System_C01/ZBM_R | 236 | 0 | 236 |
| /9/8/0/0 | Experimentals_Weapons/ZBM_BellowMaker_System_C01/ZBM_R/ZBM_Bellowmaker | 103 | 0 | 103 |
| /9/8/0/1 | Experimentals_Weapons/ZBM_BellowMaker_System_C01/ZBM_R/ZBM_Parentset_R | 3 | 0 | 3 |
| /9/8/0/2 | Experimentals_Weapons/ZBM_BellowMaker_System_C01/ZBM_R/ZBM_Contactset_R | 2 | 0 | 2 |
| /9/8/0/3 | Experimentals_Weapons/ZBM_BellowMaker_System_C01/ZBM_R/ZBM_位置合わせオブジェクト | 127 | 0 | 127 |
| /9/9 | Experimentals_Weapons/CB_CircleBrade_WH | 231 | 0 | 231 |
| /9/9/0 | Experimentals_Weapons/CB_CircleBrade_WH/CB_weapon | 230 | 0 | 230 |
| /9/9/0/0 | Experimentals_Weapons/CB_CircleBrade_WH/CB_weapon/CB_Circle | 180 | 0 | 180 |
| /9/9/0/1 | Experimentals_Weapons/CB_CircleBrade_WH/CB_weapon/Constraint_set | 13 | 0 | 13 |
| /9/9/0/2 | Experimentals_Weapons/CB_CircleBrade_WH/CB_weapon/Contact_set | 6 | 0 | 6 |
| /9/9/0/3 | Experimentals_Weapons/CB_CircleBrade_WH/CB_weapon/位置確認用（アップロード時には非表示にしてください） | 30 | 0 | 30 |
| /9/10 | Experimentals_Weapons/EIR_EisenRohr | 408 | 0 | 408 |
| /9/10/0 | Experimentals_Weapons/EIR_EisenRohr/EIR | 407 | 0 | 407 |
| /9/10/0/0 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_ConstTarget | 9 | 0 | 9 |
| /9/10/0/1 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_Dynamics | 22 | 0 | 22 |
| /9/10/0/2 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_Effect | 259 | 0 | 259 |
| /9/10/0/3 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_SE | 11 | 0 | 11 |
| /9/10/0/4 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_EisenRohr | 40 | 0 | 40 |
| /9/10/0/5 | Experimentals_Weapons/EIR_EisenRohr/EIR/EIR_bullet | 4 | 0 | 4 |
| /9/10/0/6 | Experimentals_Weapons/EIR_EisenRohr/EIR/位置合わせ | 61 | 0 | 61 |
| /9/11 | Experimentals_Weapons/EIR_EisenRohr_shield | 12 | 0 | 12 |
| /9/11/0 | Experimentals_Weapons/EIR_EisenRohr_shield/EIR | 11 | 0 | 11 |
| /9/11/0/0 | Experimentals_Weapons/EIR_EisenRohr_shield/EIR/EIR_shield_Parentset | 2 | 0 | 2 |
| /9/11/0/1 | Experimentals_Weapons/EIR_EisenRohr_shield/EIR/EIR_shield_Effect | 2 | 0 | 2 |
| /9/11/0/2 | Experimentals_Weapons/EIR_EisenRohr_shield/EIR/EIR_shield | 6 | 0 | 6 |
| /9/12 | Experimentals_Weapons/ZGR_Gunrod | 264 | 0 | 264 |
| /9/12/0 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R | 263 | 0 | 263 |
| /9/12/0/0 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/Gunrod_body | 49 | 0 | 49 |
| /9/12/0/1 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/ZGR_R_Cartholder_L | 9 | 0 | 9 |
| /9/12/0/2 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/Parentset | 7 | 0 | 7 |
| /9/12/0/3 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/ContactSet | 7 | 0 | 7 |
| /9/12/0/4 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/Effect | 111 | 0 | 111 |
| /9/12/0/5 | Experimentals_Weapons/ZGR_Gunrod/ZGR_Gunrod_R/位置決めオブジェクト | 79 | 0 | 79 |
| /9/13 | Experimentals_Weapons/HAK_HAKUGEI | 127 | 0 | 127 |
| /9/13/0 | Experimentals_Weapons/HAK_HAKUGEI/HAK_Hakugei_System | 126 | 0 | 126 |
| /9/13/0/0 | Experimentals_Weapons/HAK_HAKUGEI/HAK_Hakugei_System/HAK_Hakugei_body | 95 | 0 | 95 |
| /9/13/0/1 | Experimentals_Weapons/HAK_HAKUGEI/HAK_Hakugei_System/HAK_Parentset | 27 | 0 | 27 |
| /9/13/0/2 | Experimentals_Weapons/HAK_HAKUGEI/HAK_Hakugei_System/HAK_Contactset | 2 | 0 | 2 |
| /9/13/0/3 | Experimentals_Weapons/HAK_HAKUGEI/HAK_Hakugei_System/HAK_Empty | 1 | 0 | 1 |
| /9/14 | Experimentals_Weapons/HNG_Honegami_L | 340 | 0 | 340 |
| /9/14/0 | Experimentals_Weapons/HNG_Honegami_L/HNG | 339 | 0 | 339 |
| /9/14/0/0 | Experimentals_Weapons/HNG_Honegami_L/HNG/HNG_ConstTarget | 6 | 0 | 6 |
| /9/14/0/1 | Experimentals_Weapons/HNG_Honegami_L/HNG/HNG_Honegami | 83 | 0 | 83 |
| /9/14/0/2 | Experimentals_Weapons/HNG_Honegami_L/HNG/HNG_particle | 46 | 0 | 46 |
| /9/14/0/3 | Experimentals_Weapons/HNG_Honegami_L/HNG/HNG_Dynamics | 10 | 0 | 10 |
| /9/14/0/4 | Experimentals_Weapons/HNG_Honegami_L/HNG/位置合わせ | 193 | 0 | 193 |
| /9/15 | Experimentals_Weapons/NRK_NARUKAMI_L | 164 | 0 | 164 |
| /9/15/0 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK | 163 | 0 | 163 |
| /9/15/0/0 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/NRK_Constraint | 2 | 0 | 2 |
| /9/15/0/1 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/NRK_ConstTarget | 13 | 0 | 13 |
| /9/15/0/2 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/NRK_Dynamics | 14 | 0 | 14 |
| /9/15/0/3 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/NRK_Effect | 24 | 0 | 24 |
| /9/15/0/4 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/NRK_Narukami | 24 | 0 | 24 |
| /9/15/0/5 | Experimentals_Weapons/NRK_NARUKAMI_L/NRK/位置合わせ | 85 | 0 | 85 |
| /9/16 | Experimentals_Weapons/ORT_Orthrus | 347 | 0 | 347 |
| /9/16/0 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System | 346 | 0 | 346 |
| /9/16/0/0 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System/ORT_Orthrus_body | 140 | 0 | 140 |
| /9/16/0/1 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System/ORT_Parentset | 23 | 0 | 23 |
| /9/16/0/2 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System/ORT_Contact | 7 | 0 | 7 |
| /9/16/0/3 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System/ORT_Constraintset | 8 | 0 | 8 |
| /9/16/0/4 | Experimentals_Weapons/ORT_Orthrus/ORT_Orthrus_System/ORT_Particle | 167 | 0 | 167 |
| /9/17 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー | 60 | 0 | 60 |
| /9/17/0 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]kaba | 1 | 0 | 1 |
| /9/17/1 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]kaba (1) | 1 | 0 | 1 |
| /9/17/2 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ469 | 1 | 0 | 1 |
| /9/17/3 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ505 | 1 | 0 | 1 |
| /9/17/4 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ508 | 1 | 0 | 1 |
| /9/17/5 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ515 | 1 | 0 | 1 |
| /9/17/6 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ534 | 1 | 0 | 1 |
| /9/17/7 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ558 | 1 | 0 | 1 |
| /9/17/8 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ559 | 1 | 0 | 1 |
| /9/17/9 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ560 | 1 | 0 | 1 |
| /9/17/10 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ581 | 1 | 0 | 1 |
| /9/17/11 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ583 | 1 | 0 | 1 |
| /9/17/12 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ584 | 1 | 0 | 1 |
| /9/17/13 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ593 | 1 | 0 | 1 |
| /9/17/14 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ595 | 1 | 0 | 1 |
| /9/17/15 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ596 | 1 | 0 | 1 |
| /9/17/16 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ617 | 1 | 0 | 1 |
| /9/17/17 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ629 | 1 | 0 | 1 |
| /9/17/18 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ630 | 1 | 0 | 1 |
| /9/17/19 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ631 | 1 | 0 | 1 |
| /9/17/20 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ632 | 1 | 0 | 1 |
| /9/17/21 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ634 | 1 | 0 | 1 |
| /9/17/22 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ637 | 1 | 0 | 1 |
| /9/17/23 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ460 | 1 | 0 | 1 |
| /9/17/24 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ521 | 1 | 0 | 1 |
| /9/17/25 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ535 | 1 | 0 | 1 |
| /9/17/26 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ561 | 1 | 0 | 1 |
| /9/17/27 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ582 | 1 | 0 | 1 |
| /9/17/28 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ462 | 1 | 0 | 1 |
| /9/17/29 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ585 | 1 | 0 | 1 |
| /9/17/30 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ586 | 1 | 0 | 1 |
| /9/17/31 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ463 | 1 | 0 | 1 |
| /9/17/32 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ466 | 1 | 0 | 1 |
| /9/17/33 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ473 | 1 | 0 | 1 |
| /9/17/34 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ490 | 1 | 0 | 1 |
| /9/17/35 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ502 | 1 | 0 | 1 |
| /9/17/36 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ504 | 1 | 0 | 1 |
| /9/17/37 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ509 | 1 | 0 | 1 |
| /9/17/38 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ511 | 1 | 0 | 1 |
| /9/17/39 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ513 | 1 | 0 | 1 |
| /9/17/40 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ514 | 1 | 0 | 1 |
| /9/17/41 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ516 | 1 | 0 | 1 |
| /9/17/42 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ578 | 1 | 0 | 1 |
| /9/17/43 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ580 | 1 | 0 | 1 |
| /9/17/44 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ591 | 1 | 0 | 1 |
| /9/17/45 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ613 | 1 | 0 | 1 |
| /9/17/46 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ614 | 1 | 0 | 1 |
| /9/17/47 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ506 | 1 | 0 | 1 |
| /9/17/48 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ510 | 1 | 0 | 1 |
| /9/17/49 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ512 | 1 | 0 | 1 |
| /9/17/50 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ519 | 1 | 0 | 1 |
| /9/17/51 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ579 | 1 | 0 | 1 |
| /9/17/52 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ618 | 1 | 0 | 1 |
| /9/17/53 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ622 | 1 | 0 | 1 |
| /9/17/54 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ623 | 1 | 0 | 1 |
| /9/17/55 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ625 | 1 | 0 | 1 |
| /9/17/56 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ626 | 1 | 0 | 1 |
| /9/17/57 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ628 | 1 | 0 | 1 |
| /9/17/58 | Experimentals_Weapons/SFでサイバーな加速重槌式ハンマー/[Bone]ボディ636 | 1 | 0 | 1 |
| /9/18 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード | 33 | 0 | 33 |
| /9/18/0 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体 | 16 | 0 | 16 |
| /9/18/0/0 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ518 | 1 | 0 | 1 |
| /9/18/0/1 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ519 | 1 | 0 | 1 |
| /9/18/0/2 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ520 | 1 | 0 | 1 |
| /9/18/0/3 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ523 | 1 | 0 | 1 |
| /9/18/0/4 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ524 | 1 | 0 | 1 |
| /9/18/0/5 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ526 | 1 | 0 | 1 |
| /9/18/0/6 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ527 | 1 | 0 | 1 |
| /9/18/0/7 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ528 | 1 | 0 | 1 |
| /9/18/0/8 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ498 | 1 | 0 | 1 |
| /9/18/0/9 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ525 | 1 | 0 | 1 |
| /9/18/0/10 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ515 | 1 | 0 | 1 |
| /9/18/0/11 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ496 | 1 | 0 | 1 |
| /9/18/0/12 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ494 | 1 | 0 | 1 |
| /9/18/0/13 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ499 | 1 | 0 | 1 |
| /9/18/0/14 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/ブレード本体/[Bone]ボディ497 | 1 | 0 | 1 |
| /9/18/1 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや | 16 | 0 | 16 |
| /9/18/1/0 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ532 | 1 | 0 | 1 |
| /9/18/1/1 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ504 | 1 | 0 | 1 |
| /9/18/1/2 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ505 | 1 | 0 | 1 |
| /9/18/1/3 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ535 | 1 | 0 | 1 |
| /9/18/1/4 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ503 | 1 | 0 | 1 |
| /9/18/1/5 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ502 | 1 | 0 | 1 |
| /9/18/1/6 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ534 | 1 | 0 | 1 |
| /9/18/1/7 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ533 | 1 | 0 | 1 |
| /9/18/1/8 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ501 | 1 | 0 | 1 |
| /9/18/1/9 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ531 | 1 | 0 | 1 |
| /9/18/1/10 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ511 | 1 | 0 | 1 |
| /9/18/1/11 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ512 | 1 | 0 | 1 |
| /9/18/1/12 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ529 | 1 | 0 | 1 |
| /9/18/1/13 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ507 | 1 | 0 | 1 |
| /9/18/1/14 | Experimentals_Weapons/SFでサイバーな強襲被覆刀ブレード/さや/[Bone]ボディ516 | 1 | 0 | 1 |
| /9/19 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード | 90 | 0 | 90 |
| /9/19/0 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体 | 89 | 0 | 89 |
| /9/19/0/0 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody11 | 1 | 0 | 1 |
| /9/19/0/1 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody29 | 1 | 0 | 1 |
| /9/19/0/2 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody34 | 1 | 0 | 1 |
| /9/19/0/3 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody36 | 1 | 0 | 1 |
| /9/19/0/4 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody50 | 1 | 0 | 1 |
| /9/19/0/5 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody12 | 1 | 0 | 1 |
| /9/19/0/6 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody22 | 1 | 0 | 1 |
| /9/19/0/7 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody24 | 1 | 0 | 1 |
| /9/19/0/8 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody27 | 1 | 0 | 1 |
| /9/19/0/9 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody28 | 1 | 0 | 1 |
| /9/19/0/10 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody38 | 1 | 0 | 1 |
| /9/19/0/11 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody54 | 1 | 0 | 1 |
| /9/19/0/12 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody55 | 1 | 0 | 1 |
| /9/19/0/13 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody56 | 1 | 0 | 1 |
| /9/19/0/14 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody66 | 1 | 0 | 1 |
| /9/19/0/15 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody75 | 1 | 0 | 1 |
| /9/19/0/16 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody76 | 1 | 0 | 1 |
| /9/19/0/17 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody79 | 1 | 0 | 1 |
| /9/19/0/18 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody80 | 1 | 0 | 1 |
| /9/19/0/19 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody87 | 1 | 0 | 1 |
| /9/19/0/20 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody88 | 1 | 0 | 1 |
| /9/19/0/21 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody93 | 1 | 0 | 1 |
| /9/19/0/22 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody95 | 1 | 0 | 1 |
| /9/19/0/23 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody97 | 1 | 0 | 1 |
| /9/19/0/24 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody98 | 1 | 0 | 1 |
| /9/19/0/25 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody13 | 1 | 0 | 1 |
| /9/19/0/26 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody15 | 1 | 0 | 1 |
| /9/19/0/27 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody16 | 1 | 0 | 1 |
| /9/19/0/28 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody17 | 1 | 0 | 1 |
| /9/19/0/29 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody18 | 1 | 0 | 1 |
| /9/19/0/30 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody19 | 1 | 0 | 1 |
| /9/19/0/31 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody20 | 1 | 0 | 1 |
| /9/19/0/32 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody23 | 1 | 0 | 1 |
| /9/19/0/33 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody30 | 1 | 0 | 1 |
| /9/19/0/34 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody32 | 1 | 0 | 1 |
| /9/19/0/35 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody33 | 1 | 0 | 1 |
| /9/19/0/36 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody37 | 1 | 0 | 1 |
| /9/19/0/37 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody40 | 1 | 0 | 1 |
| /9/19/0/38 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody41 | 1 | 0 | 1 |
| /9/19/0/39 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody42 | 1 | 0 | 1 |
| /9/19/0/40 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody44 | 1 | 0 | 1 |
| /9/19/0/41 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody45 | 1 | 0 | 1 |
| /9/19/0/42 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody46 | 1 | 0 | 1 |
| /9/19/0/43 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody47 | 1 | 0 | 1 |
| /9/19/0/44 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody49 | 1 | 0 | 1 |
| /9/19/0/45 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody51 | 1 | 0 | 1 |
| /9/19/0/46 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody52 | 1 | 0 | 1 |
| /9/19/0/47 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody58 | 1 | 0 | 1 |
| /9/19/0/48 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody59 | 1 | 0 | 1 |
| /9/19/0/49 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody61 | 1 | 0 | 1 |
| /9/19/0/50 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody63 | 1 | 0 | 1 |
| /9/19/0/51 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody64 | 1 | 0 | 1 |
| /9/19/0/52 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody65 | 1 | 0 | 1 |
| /9/19/0/53 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody67 | 1 | 0 | 1 |
| /9/19/0/54 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody74 | 1 | 0 | 1 |
| /9/19/0/55 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody14 | 1 | 0 | 1 |
| /9/19/0/56 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody21 | 1 | 0 | 1 |
| /9/19/0/57 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody25 | 1 | 0 | 1 |
| /9/19/0/58 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody35 | 1 | 0 | 1 |
| /9/19/0/59 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody43 | 1 | 0 | 1 |
| /9/19/0/60 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody48 | 1 | 0 | 1 |
| /9/19/0/61 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody68 | 1 | 0 | 1 |
| /9/19/0/62 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody69 | 1 | 0 | 1 |
| /9/19/0/63 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody70 | 1 | 0 | 1 |
| /9/19/0/64 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody71 | 1 | 0 | 1 |
| /9/19/0/65 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody72 | 1 | 0 | 1 |
| /9/19/0/66 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody73 | 1 | 0 | 1 |
| /9/19/0/67 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody77 | 1 | 0 | 1 |
| /9/19/0/68 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody81 | 1 | 0 | 1 |
| /9/19/0/69 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody26 | 1 | 0 | 1 |
| /9/19/0/70 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody31 | 1 | 0 | 1 |
| /9/19/0/71 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody39 | 1 | 0 | 1 |
| /9/19/0/72 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody53 | 1 | 0 | 1 |
| /9/19/0/73 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody57 | 1 | 0 | 1 |
| /9/19/0/74 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody60 | 1 | 0 | 1 |
| /9/19/0/75 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody62 | 1 | 0 | 1 |
| /9/19/0/76 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody82 | 1 | 0 | 1 |
| /9/19/0/77 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody83 | 1 | 0 | 1 |
| /9/19/0/78 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody84 | 1 | 0 | 1 |
| /9/19/0/79 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody85 | 1 | 0 | 1 |
| /9/19/0/80 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody86 | 1 | 0 | 1 |
| /9/19/0/81 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody89 | 1 | 0 | 1 |
| /9/19/0/82 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody90 | 1 | 0 | 1 |
| /9/19/0/83 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody91 | 1 | 0 | 1 |
| /9/19/0/84 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody92 | 1 | 0 | 1 |
| /9/19/0/85 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody94 | 1 | 0 | 1 |
| /9/19/0/86 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody96 | 1 | 0 | 1 |
| /9/19/0/87 | Experimentals_Weapons/SFでサイバーな生体刀剣ブレード/剣本体/[Bone]MeshBody78 | 1 | 0 | 1 |
| /9/20 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド | 203 | 0 | 203 |
| /9/20/0 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分 | 67 | 0 | 67 |
| /9/20/0/0 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ242 | 1 | 0 | 1 |
| /9/20/0/1 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ206 | 1 | 0 | 1 |
| /9/20/0/2 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ240 | 1 | 0 | 1 |
| /9/20/0/3 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ207 | 1 | 0 | 1 |
| /9/20/0/4 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ243 | 1 | 0 | 1 |
| /9/20/0/5 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ208 | 1 | 0 | 1 |
| /9/20/0/6 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ220 | 1 | 0 | 1 |
| /9/20/0/7 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ244 | 1 | 0 | 1 |
| /9/20/0/8 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ222 | 1 | 0 | 1 |
| /9/20/0/9 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ50 | 1 | 0 | 1 |
| /9/20/0/10 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ62 | 1 | 0 | 1 |
| /9/20/0/11 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ61 | 1 | 0 | 1 |
| /9/20/0/12 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ265 | 1 | 0 | 1 |
| /9/20/0/13 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ247 | 1 | 0 | 1 |
| /9/20/0/14 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ56 | 1 | 0 | 1 |
| /9/20/0/15 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ54 | 1 | 0 | 1 |
| /9/20/0/16 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ52 | 1 | 0 | 1 |
| /9/20/0/17 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ221 | 1 | 0 | 1 |
| /9/20/0/18 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ245 | 1 | 0 | 1 |
| /9/20/0/19 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ241 | 1 | 0 | 1 |
| /9/20/0/20 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ237 | 1 | 0 | 1 |
| /9/20/0/21 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ230 | 1 | 0 | 1 |
| /9/20/0/22 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ238 | 1 | 0 | 1 |
| /9/20/0/23 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ236 | 1 | 0 | 1 |
| /9/20/0/24 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ232 | 1 | 0 | 1 |
| /9/20/0/25 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ227 | 1 | 0 | 1 |
| /9/20/0/26 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ233 | 1 | 0 | 1 |
| /9/20/0/27 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ234 | 1 | 0 | 1 |
| /9/20/0/28 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ59 | 1 | 0 | 1 |
| /9/20/0/29 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ224 | 1 | 0 | 1 |
| /9/20/0/30 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ223 | 1 | 0 | 1 |
| /9/20/0/31 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ225 | 1 | 0 | 1 |
| /9/20/0/32 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ235 | 1 | 0 | 1 |
| /9/20/0/33 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ228 | 1 | 0 | 1 |
| /9/20/0/34 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ229 | 1 | 0 | 1 |
| /9/20/0/35 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ231 | 1 | 0 | 1 |
| /9/20/0/36 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ34 | 1 | 0 | 1 |
| /9/20/0/37 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ239 | 1 | 0 | 1 |
| /9/20/0/38 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ33 | 1 | 0 | 1 |
| /9/20/0/39 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ209 | 1 | 0 | 1 |
| /9/20/0/40 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ32 | 1 | 0 | 1 |
| /9/20/0/41 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ210 | 1 | 0 | 1 |
| /9/20/0/42 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ218 | 1 | 0 | 1 |
| /9/20/0/43 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ195 | 1 | 0 | 1 |
| /9/20/0/44 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ219 | 1 | 0 | 1 |
| /9/20/0/45 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ217 | 1 | 0 | 1 |
| /9/20/0/46 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ202 | 1 | 0 | 1 |
| /9/20/0/47 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ211 | 1 | 0 | 1 |
| /9/20/0/48 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ214 | 1 | 0 | 1 |
| /9/20/0/49 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ213 | 1 | 0 | 1 |
| /9/20/0/50 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ35 | 1 | 0 | 1 |
| /9/20/0/51 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ216 | 1 | 0 | 1 |
| /9/20/0/52 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ49 | 1 | 0 | 1 |
| /9/20/0/53 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ226 | 1 | 0 | 1 |
| /9/20/0/54 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ58 | 1 | 0 | 1 |
| /9/20/0/55 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ212 | 1 | 0 | 1 |
| /9/20/0/56 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ192 | 1 | 0 | 1 |
| /9/20/0/57 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ196 | 1 | 0 | 1 |
| /9/20/0/58 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ203 | 1 | 0 | 1 |
| /9/20/0/59 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ201 | 1 | 0 | 1 |
| /9/20/0/60 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ45 | 1 | 0 | 1 |
| /9/20/0/61 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ215 | 1 | 0 | 1 |
| /9/20/0/62 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ197 | 1 | 0 | 1 |
| /9/20/0/63 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ57 | 1 | 0 | 1 |
| /9/20/0/64 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ31 | 1 | 0 | 1 |
| /9/20/0/65 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/杖中心部分/[Bone]ボディ37 | 1 | 0 | 1 |
| /9/20/1 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/回転中心 | 135 | 0 | 135 |
| /9/20/1/0 | Experimentals_Weapons/SFでサイバーな装甲飛行杖型ロッド/回転中心/回転ユニット | 134 | 0 | 134 |
| /9/21 | Experimentals_Weapons/TSM_TISAME_c01_L | 226 | 0 | 226 |
| /9/21/0 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM | 225 | 0 | 225 |
| /9/21/0/0 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/TSM_Parentset | 22 | 0 | 22 |
| /9/21/0/1 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/TSM_Constraintset_L | 10 | 0 | 10 |
| /9/21/0/2 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/TSM_contact&PB | 16 | 0 | 16 |
| /9/21/0/3 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/TSM_tisame | 22 | 0 | 22 |
| /9/21/0/4 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/位置合わせ | 36 | 0 | 36 |
| /9/21/0/5 | Experimentals_Weapons/TSM_TISAME_c01_L/TSM/TSM_Effect | 118 | 0 | 118 |
| /9/22 | Experimentals_Weapons/Unixis | 168 | 0 | 168 |
| /9/22/0 | Experimentals_Weapons/Unixis/Unixis_Sword | 26 | 0 | 26 |
| /9/22/0/0 | Experimentals_Weapons/Unixis/Unixis_Sword/Mesh | 5 | 0 | 5 |
| /9/22/0/1 | Experimentals_Weapons/Unixis/Unixis_Sword/Slash_Front | 2 | 0 | 2 |
| /9/22/0/2 | Experimentals_Weapons/Unixis/Unixis_Sword/Slash_Back | 2 | 0 | 2 |
| /9/22/0/3 | Experimentals_Weapons/Unixis/Unixis_Sword/Strat | 2 | 0 | 2 |
| /9/22/0/4 | Experimentals_Weapons/Unixis/Unixis_Sword/Audio | 12 | 0 | 12 |
| /9/22/0/5 | Experimentals_Weapons/Unixis/Unixis_Sword/ULTCharge | 2 | 0 | 2 |
| /9/22/1 | Experimentals_Weapons/Unixis/Unixis_Saya | 9 | 0 | 9 |
| /9/22/1/0 | Experimentals_Weapons/Unixis/Unixis_Saya/PhysBone | 3 | 0 | 3 |
| /9/22/1/1 | Experimentals_Weapons/Unixis/Unixis_Saya/LockPhysbone | 2 | 0 | 2 |
| /9/22/1/2 | Experimentals_Weapons/Unixis/Unixis_Saya/Saya_Particle | 3 | 0 | 3 |
| /9/22/2 | Experimentals_Weapons/Unixis/Head | 2 | 0 | 2 |
| /9/22/2/0 | Experimentals_Weapons/Unixis/Head/HandTrackerRotation | 1 | 0 | 1 |
| /9/22/3 | Experimentals_Weapons/Unixis/Chest | 5 | 0 | 5 |
| /9/22/3/0 | Experimentals_Weapons/Unixis/Chest/Nageposition | 2 | 0 | 2 |
| /9/22/3/1 | Experimentals_Weapons/Unixis/Chest/SayaInitialPosition | 2 | 0 | 2 |
| /9/22/4 | Experimentals_Weapons/Unixis/RightHand | 31 | 0 | 31 |
| /9/22/4/0 | Experimentals_Weapons/Unixis/RightHand/SayaGrabPosition | 2 | 0 | 2 |
| /9/22/4/1 | Experimentals_Weapons/Unixis/RightHand/Unixis_Sword_BattouR | 1 | 0 | 1 |
| /9/22/4/2 | Experimentals_Weapons/Unixis/RightHand/FripPhysbone | 2 | 0 | 2 |
| /9/22/4/3 | Experimentals_Weapons/Unixis/RightHand/SlashPhysbone | 2 | 0 | 2 |
| /9/22/4/4 | Experimentals_Weapons/Unixis/RightHand/SayaGrabPosition2 | 1 | 0 | 1 |
| /9/22/4/5 | Experimentals_Weapons/Unixis/RightHand/HandTrackContact | 1 | 0 | 1 |
| /9/22/4/6 | Experimentals_Weapons/Unixis/RightHand/ColorChengeUIObject | 20 | 0 | 20 |
| /9/22/4/7 | Experimentals_Weapons/Unixis/RightHand/GameObject | 1 | 0 | 1 |
| /9/22/5 | Experimentals_Weapons/Unixis/LeftHand | 5 | 0 | 5 |
| /9/22/5/0 | Experimentals_Weapons/Unixis/LeftHand/Unixis_Sword_BattouL | 1 | 0 | 1 |
| /9/22/5/1 | Experimentals_Weapons/Unixis/LeftHand/FripPhysbone | 2 | 0 | 2 |
| /9/22/5/2 | Experimentals_Weapons/Unixis/LeftHand/HandContact | 1 | 0 | 1 |
| /9/22/6 | Experimentals_Weapons/Unixis/Unixis | 1 | 0 | 1 |
| /9/22/7 | Experimentals_Weapons/Unixis/GimmickObject | 4 | 0 | 4 |
| /9/22/7/0 | Experimentals_Weapons/Unixis/GimmickObject/RLHandTracker | 3 | 0 | 3 |
| /9/22/8 | Experimentals_Weapons/Unixis/Particle | 22 | 0 | 22 |
| /9/22/8/0 | Experimentals_Weapons/Unixis/Particle/SlashParticle | 15 | 0 | 15 |
| /9/22/8/1 | Experimentals_Weapons/Unixis/Particle/Skill1 | 6 | 0 | 6 |
| /9/22/9 | Experimentals_Weapons/Unixis/EditorOnlyObject | 62 | 0 | 62 |
| /9/22/9/0 | Experimentals_Weapons/Unixis/EditorOnlyObject/Unixis_Sword (1) | 26 | 0 | 26 |
| /9/22/9/1 | Experimentals_Weapons/Unixis/EditorOnlyObject/Unixis_Sword (2) | 26 | 0 | 26 |
| /9/22/9/2 | Experimentals_Weapons/Unixis/EditorOnlyObject/Unixis_Saya | 9 | 0 | 9 |

## 全コンポーネント種類
| 型 | 全数 | activeオブジェクト上 | EditorOnly祖先含む |
|---|---|---|---|
| Transform | 32989 | 8275 | 24330 |
| MeshFilter | 16494 | 4239 | 11947 |
| MeshRenderer | 16426 | 4128 | 12035 |
| RectTransform | 13861 | 1973 | 6905 |
| CanvasRenderer | 11045 | 1405 | 5415 |
| Image | 5850 | 861 | 3091 |
| UdonBehaviour | 3334 | 841 | 1492 |
| Light | 2762 | 798 | 2356 |
| LayoutElement | 2263 | 136 | 1745 |
| TextMeshProUGUI | 2254 | 299 | 1209 |
| ParticleSystem | 1899 | 74 | 1790 |
| ParticleSystemRenderer | 1899 | 74 | 1790 |
| Text | 1764 | 69 | 790 |
| MeshCollider | 1659 | 596 | 1037 |
| BoxCollider | 1556 | 656 | 743 |
| Button | 1444 | 107 | 627 |
| CanvasGroup | 1072 | 151 | 537 |
| ContentSizeFitter | 829 | 44 | 503 |
| EventTrigger | 723 | 115 | 193 |
| Canvas | 632 | 169 | 410 |
| AudioSource | 610 | 212 | 328 |
| Animator | 546 | 150 | 316 |
| GraphicRaycaster | 486 | 128 | 323 |
| HorizontalLayoutGroup | 486 | 35 | 340 |
| VerticalLayoutGroup | 481 | 24 | 369 |
| CanvasScaler | 434 | 167 | 216 |
| VRCSpatialAudioSource | 429 | 212 | 147 |
| Mask | 399 | 10 | 336 |
| VRCContactReceiver | 384 | 115 | 177 |
| ApplyTheme | 367 | 0 | 367 |
| ColorDefinition | 334 | 15 | 173 |
| Rigidbody | 329 | 130 | 117 |
| Toggle | 290 | 25 | 137 |
| eventcalendar_showcontent | 256 | 0 | 0 |
| TIM_IMEKey | 252 | 0 | 0 |
| ParentConstraint | 235 | 11 | 220 |
| VRCPickup | 227 | 85 | 97 |
| SkinnedMeshRenderer | 220 | 35 | 166 |
| VRCUiShape | 214 | 93 | 65 |
| RectMask2D | 198 | 47 | 116 |
| SphereCollider | 192 | 132 | 52 |
| TextMeshPro | 164 | 63 | 96 |
| ApplyI18n | 148 | 0 | 148 |
| ModularAvatarMenuItem | 148 | 0 | 148 |
| RawImage | 128 | 4 | 93 |
| ModularAvatarBoneProxy | 128 | 0 | 128 |
| GraphicAutoConfigurator | 126 | 0 | 126 |
| Slider | 123 | 23 | 68 |
| VRCObjectSync | 117 | 56 | 58 |
| AudioReverbFilter | 100 | 54 | 46 |
| VRCUrlInputField | 94 | 6 | 78 |
| ReflectionProbe | 86 | 42 | 44 |
| ScrollRect | 85 | 3 | 55 |
| NDynamicObject | 84 | 10 | 38 |
| VRCPhysBone | 84 | 26 | 58 |
| ToggleGroup | 82 | 6 | 42 |
| NTouchPanelButton | 74 | 20 | 0 |
| Scrollbar | 74 | 3 | 46 |
| Switch_Trigger | 70 | 23 | 4 |
| MessageManager | 64 | 0 | 64 |
| Selector | 64 | 0 | 64 |
| GridLayoutGroup | 63 | 9 | 34 |
| VendingMachineShopButton | 60 | 60 | 0 |
| VRCContactSender | 55 | 0 | 55 |
| ScaleConstraint | 54 | 0 | 53 |
| NElevatorButton | 52 | 30 | 22 |
| CalendarCellObject | 49 | 0 | 49 |
| TMP_SubMeshUI | 48 | 48 | 0 |
| TIM_ButtonAnimation | 48 | 43 | 0 |
| VRCParentConstraint | 47 | 0 | 47 |
| IndexTrigger | 45 | 0 | 23 |
| LODGroup | 44 | 6 | 38 |
| SwitchBase | 42 | 40 | 2 |
| Elevator | 42 | 0 | 42 |
| LightProbeGroup | 41 | 13 | 28 |
| LineRenderer | 41 | 0 | 15 |
| PointLightVolumeInstance | 39 | 39 | 0 |
| LatteCupSurfaceReceiver | 36 | 0 | 0 |
| FishAgent | 34 | 0 | 34 |
| Slider2D_EventSender | 33 | 18 | 3 |
| CapsuleCollider | 32 | 14 | 17 |
| VRCMirrorReflection | 31 | 0 | 11 |
| NEventButton | 30 | 3 | 0 |
| YamaPlayerModuleDefinition | 29 | 9 | 20 |
| VRCPhysBoneCollider | 28 | 2 | 26 |
| SliderValueHelper | 27 | 0 | 27 |
| NBoothItem | 24 | 0 | 0 |
| NTagCenterWidth | 24 | 0 | 0 |
| NTagRightXPosition | 24 | 0 | 0 |
| PostProcessVolume | 23 | 16 | 7 |
| AspectRatioFitter | 23 | 0 | 13 |
| flavor | 22 | 0 | 22 |
| OcclusionArea | 21 | 21 | 0 |
| InputField | 21 | 2 | 10 |
| MirrorActivator | 20 | 10 | 0 |
| PickupAutoHoldSwitcher | 20 | 20 | 0 |
| TACEventTrigger | 20 | 0 | 3 |
| PositionConstraint | 20 | 0 | 19 |
| ModularAvatarParameters | 20 | 0 | 20 |
| SliderSwitch | 19 | 18 | 1 |
| SliderSwitch_Pickup | 19 | 12 | 1 |
| VendingMachineObjectPool | 18 | 18 | 0 |
| SignPlate_Receiver | 18 | 18 | 0 |
| FlekSitHelper | 17 | 12 | 5 |
| QvPen_Manager | 17 | 0 | 17 |
| QvPen_InteractButton | 17 | 0 | 17 |
| eventcalendar_checkbox | 16 | 0 | 0 |
| SignPlate | 16 | 16 | 0 |
| LuraSlot_Buttons | 16 | 16 | 0 |
| RotationConstraint | 16 | 0 | 16 |
| LoopScroll | 15 | 1 | 8 |
| Outline | 15 | 0 | 10 |
| QvPen_PenManager | 15 | 0 | 15 |
| QvPen_Pen | 15 | 0 | 15 |
| QvPen_LateSync | 15 | 0 | 15 |
| TrailRenderer | 15 | 0 | 15 |
| QvPen_ClearButton | 15 | 0 | 15 |
| ModuleMetadata | 14 | 0 | 14 |
| Menu_ColorWheel_ColorTemplate | 14 | 0 | 0 |
| ModularAvatarWorldFixedObject | 14 | 0 | 14 |
| LightVolumeInstance | 13 | 13 | 0 |
| SwitchSelector | 13 | 12 | 1 |
| I18nManager | 13 | 0 | 13 |
| TIM_ToggleButtonAnimation | 13 | 12 | 0 |
| LanguageReceiver | 13 | 0 | 13 |
| ButtonWithState | 13 | 0 | 13 |
| Camera | 12 | 4 | 7 |
| VRCAvatarPedestal | 12 | 12 | 0 |
| NThumbnailButton | 12 | 12 | 0 |
| BaseVideoPlayerHandler | 12 | 2 | 6 |
| SliderHelper | 12 | 2 | 6 |
| SpringJoint | 12 | 12 | 0 |
| HingeJoint | 12 | 12 | 0 |
| AudioLowPassFilter | 12 | 7 | 4 |
| Chip | 12 | 0 | 12 |
| StudioCapsule | 11 | 11 | 0 |
| TMProMigratable | 11 | 0 | 11 |
| VRCUnityVideoPlayer | 10 | 3 | 4 |
| MirrorController | 10 | 10 | 0 |
| MirrorAreaPreview | 10 | 0 | 10 |
| MirrorTrigger | 10 | 10 | 0 |
| Controller_MirrorOpacity | 10 | 10 | 0 |
| CashBlaster | 10 | 0 | 10 |
| VRCRotationConstraint | 10 | 0 | 10 |
| LightVolumeTrigger | 9 | 9 | 0 |
| SpriteRenderer | 9 | 0 | 8 |
| VRCAVProVideoPlayer | 9 | 3 | 4 |
| VRCAVProVideoSpeaker | 9 | 3 | 4 |
| DoorHandle | 9 | 9 | 0 |
| VRCStation | 9 | 0 | 8 |
| AudioReverbActivator | 8 | 0 | 0 |
| Elevator_Switch | 8 | 7 | 1 |
| TACScrollRectSync | 8 | 0 | 8 |
| VideoPlayerLinkCard | 8 | 0 | 8 |
| chacoal | 8 | 0 | 8 |
| ImageViewerHandler | 7 | 1 | 4 |
| ModuleManager | 7 | 1 | 4 |
| RangeSlider | 7 | 0 | 4 |
| PFDisableGameObject | 7 | 0 | 7 |
| TIM_QMContentHover | 7 | 6 | 0 |
| TIM_LocalizedText | 7 | 7 | 0 |
| ToggleSwitch | 7 | 0 | 7 |
| VRCAimConstraint | 7 | 0 | 7 |
| YamaPlayer | 6 | 1 | 3 |
| Controller | 6 | 1 | 3 |
| VRCAVProVideoScreen | 6 | 1 | 3 |
| QueueList | 6 | 1 | 3 |
| HistoryList | 6 | 1 | 3 |
| PlaylistManager | 6 | 1 | 3 |
| YamaPlayerScreen | 6 | 1 | 3 |
| YamaPlayerSpeaker | 6 | 1 | 3 |
| AppearanceSettings | 6 | 1 | 3 |
| LocalizationSettings | 6 | 1 | 3 |
| UIController | 6 | 1 | 3 |
| Modal | 6 | 0 | 3 |
| Controller_AudioVolume | 6 | 6 | 0 |
| MoneyTarget | 6 | 0 | 6 |
| ApplyTimeI18n | 6 | 0 | 6 |
| AimConstraint | 6 | 0 | 6 |
| VRCPositionConstraint | 6 | 0 | 6 |
| NBorder | 5 | 4 | 0 |
| LurasSwitch | 5 | 0 | 5 |
| TMP_InputField | 5 | 2 | 1 |
| PlaylistItem | 5 | 1 | 4 |
| SingleUsePickup | 5 | 5 | 0 |
| SingleUsePickupSync | 5 | 5 | 0 |
| RoomOwnerDisplay | 5 | 5 | 0 |
| RadioButtonHelper | 5 | 0 | 5 |
| VRCPlayerObject | 5 | 1 | 0 |
| VRCPortalMarker | 5 | 0 | 5 |
| InteractToSit | 5 | 0 | 5 |
| UGuiPenCommitTarget | 5 | 0 | 5 |
| SwitchSyncer | 4 | 4 | 0 |
| NBoothItemContainer | 4 | 0 | 0 |
| NGetBoothItemsRequest | 4 | 0 | 0 |
| NAllowButton | 4 | 4 | 0 |
| Dropdown | 4 | 0 | 3 |
| VendingMachineTrigger | 4 | 2 | 0 |
| VendingMachineFlap | 4 | 4 | 0 |
| LatteCup | 4 | 4 | 0 |
| CupAttachDetector | 4 | 4 | 0 |
| LatteCupParticleReceiver | 4 | 4 | 0 |
| LatteCupSaucer | 4 | 4 | 0 |
| NightModeActivator | 4 | 0 | 0 |
| VoiceSilencer | 4 | 0 | 0 |
| NDynamicObjectSnapPoint | 4 | 4 | 0 |
| FlashClicker | 4 | 0 | 4 |
| CausticsTrigger | 4 | 4 | 0 |
| CancelMove | 4 | 0 | 0 |
| AudioListener | 4 | 2 | 2 |
| SataniaMic | 4 | 0 | 4 |
| FishSchoolController | 4 | 0 | 4 |
| WheelCollider | 4 | 0 | 4 |
| EventSystem | 3 | 1 | 2 |
| StandaloneInputModule | 3 | 1 | 2 |
| AudioReverbZone | 3 | 1 | 2 |
| AudioLinkAdaptor | 3 | 1 | 2 |
| AudioLinkAdaptorUI | 3 | 1 | 2 |
| AutoPlay | 3 | 1 | 2 |
| LightVolumeAdaptor | 3 | 1 | 2 |
| LTCGIAdaptor | 3 | 1 | 2 |
| PermissionManagement | 3 | 1 | 2 |
| PermissionManagementUI | 3 | 1 | 2 |
| Persistence | 3 | 1 | 2 |
| SlideShower | 3 | 1 | 2 |
| SlideShowerUI | 3 | 1 | 2 |
| TimelineSync | 3 | 1 | 2 |
| VideoInfoDownloader | 3 | 1 | 2 |
| LTCGI_Screen | 3 | 1 | 2 |
| VendingMachineTouchTrigger | 3 | 3 | 0 |
| SwitchBoard | 3 | 3 | 0 |
| Controller_TransformChange | 3 | 2 | 1 |
| PlayerNameCapture | 3 | 3 | 0 |
| DoorTrigger | 3 | 3 | 0 |
| ColliderProvider | 3 | 0 | 3 |
| LowPassTrigger | 3 | 3 | 0 |
| WelcomeWindow_System | 3 | 3 | 0 |
| Elevator_Floor | 3 | 3 | 0 |
| ToggleSwitchHelper | 3 | 0 | 3 |
| TeleportTarget | 3 | 0 | 3 |
| TIM_IMEDict | 3 | 3 | 0 |
| TIM_QMUISpinner | 3 | 2 | 0 |
| ChatMessageRef | 3 | 3 | 0 |
| QvPen_ToggleModeButton | 3 | 0 | 3 |
| TouchZoneTracker | 3 | 0 | 3 |
| bowl | 3 | 0 | 3 |
| Sync | 3 | 0 | 3 |
| VRCScaleConstraint | 3 | 0 | 3 |
| UMoffPen2AnchorFrameTransformEditorSync | 3 | 0 | 3 |
| ModularAvatarVisibleHeadAccessory | 3 | 0 | 3 |
| UdonChips | 2 | 1 | 1 |
| UdonChipsOffline | 2 | 1 | 1 |
| NUdonGameChips | 2 | 1 | 1 |
| TankCausticsBoxBinder | 2 | 2 | 0 |
| DistanceCuller | 2 | 2 | 0 |
| FishManager | 2 | 2 | 0 |
| NBoothCategoryButton | 2 | 0 | 0 |
| NShowSelectorUiButton | 2 | 1 | 0 |
| ImageLoader | 2 | 1 | 1 |
| VendingMachine | 2 | 2 | 0 |
| VendingMachineCoinTrigger | 2 | 2 | 0 |
| despawnTimer | 2 | 0 | 0 |
| FlagSync | 2 | 2 | 0 |
| MilkPack | 2 | 2 | 0 |
| MilkPackSync | 2 | 2 | 0 |
| MilkPitcher | 2 | 2 | 0 |
| MilkPitcherSync | 2 | 2 | 0 |
| MilkPitcherParticleReceiver | 2 | 2 | 0 |
| MilkPitcherNozzleDetector | 2 | 2 | 0 |
| MilkPitcherAttachDetector | 2 | 2 | 0 |
| Tablet | 2 | 1 | 1 |
| StudioCapsuleRack | 2 | 2 | 0 |
| StudioCup | 2 | 2 | 0 |
| StudioLiquidTimeline | 2 | 2 | 0 |
| StudioCupContent | 2 | 2 | 0 |
| ObjectLock_Toggle | 2 | 0 | 0 |
| VacuumCleaner | 2 | 2 | 0 |
| Jumper | 2 | 2 | 0 |
| AnimationActivator | 2 | 0 | 0 |
| SwitchFunction_SavePoint | 2 | 2 | 0 |
| SavePoint_Activator | 2 | 0 | 0 |
| NDoorPhysBoneHandleInput | 2 | 2 | 0 |
| NDoorAuthZone | 2 | 2 | 0 |
| NDoorTeleportInput | 2 | 2 | 0 |
| NDoorHandleInput | 2 | 2 | 0 |
| Mood_Manager | 2 | 2 | 0 |
| SilenceArea_Trigger | 2 | 2 | 0 |
| SliderChanger | 2 | 0 | 0 |
| HeightOffsetter | 2 | 2 | 0 |
| HeightOffsetterPreview | 2 | 0 | 2 |
| OwnerLocker | 2 | 2 | 0 |
| LuraSlot | 2 | 2 | 0 |
| Cardkey_Receiver | 2 | 2 | 0 |
| MaterialChanger | 2 | 1 | 1 |
| MaterialResetter | 2 | 1 | 1 |
| ButtonBackground | 2 | 0 | 0 |
| Gun_RestrictedArea | 2 | 0 | 2 |
| AutoDoor | 2 | 2 | 0 |
| LurasWaterStairFlag | 2 | 2 | 0 |
| LurasVoiceShutter_RoomTrigger | 2 | 2 | 0 |
| ToggleSwitchV2Module | 2 | 0 | 2 |
| TSV2SwitchHandler | 2 | 0 | 2 |
| TSV2SliderHandler | 2 | 0 | 2 |
| TSV2TriggerHandler | 2 | 0 | 2 |
| ModuleExecutor | 2 | 0 | 2 |
| DeselectTargetHelper | 2 | 0 | 2 |
| QuickMenuCanvas | 2 | 0 | 2 |
| TouchableCanvas | 2 | 0 | 1 |
| TIM_IMEAttach | 2 | 2 | 0 |
| TIM_QMPanelAnchor | 2 | 1 | 0 |
| TIM_ToggleSwitch | 2 | 1 | 0 |
| MessageFader | 2 | 2 | 0 |
| LanguageSwitch | 2 | 2 | 0 |
| PlayerVolumeController | 2 | 0 | 2 |
| PitchShifter | 2 | 0 | 2 |
| PitchShifterUI | 2 | 0 | 2 |
| QvPen_EraserManager | 2 | 0 | 2 |
| QvPen_Eraser | 2 | 0 | 2 |
| PhotoIcon | 2 | 0 | 2 |
| Shadow | 2 | 0 | 2 |
| CameraHide | 2 | 0 | 2 |
| UnpackGrab | 2 | 0 | 2 |
| RainClipPlayer | 2 | 0 | 2 |
| ViewTrackerTexts | 2 | 0 | 2 |
| FloatingEntity | 2 | 0 | 2 |
| VideoPlayerHandler | 2 | 0 | 2 |
| HideIfIdleTextureAvailable | 2 | 0 | 2 |
| PooledScrollView | 2 | 0 | 2 |
| ListEntry | 2 | 0 | 2 |
| ListEntryColorAutoConfigurator | 2 | 0 | 2 |
| UdonCarThrottle | 2 | 0 | 2 |
| SimpleSwitch | 2 | 0 | 2 |
| UKeyboard | 2 | 0 | 2 |
| VRCSceneDescriptor | 1 | 1 | 0 |
| PipelineManager | 1 | 1 | 0 |
| NAdvancedWorldSettings | 1 | 1 | 0 |
| PostProcessLayer | 1 | 1 | 0 |
| NBorderManager | 1 | 1 | 0 |
| NVirtualInputManager | 1 | 0 | 1 |
| NDoorSystem | 1 | 1 | 0 |
| AreaCullinger | 1 | 1 | 0 |
| NSwimSystem | 1 | 1 | 0 |
| NFlyingSystem | 1 | 1 | 0 |
| NStatusSystem | 1 | 1 | 0 |
| NSecuritySystem | 1 | 1 | 0 |
| NSecurityZone | 1 | 1 | 0 |
| NSecurityObjectGuard | 1 | 1 | 0 |
| NInventoryManager | 1 | 1 | 0 |
| NMovementSystem | 1 | 1 | 0 |
| NDebugVisualizationManager | 1 | 0 | 1 |
| NAuthorityLevelManager | 1 | 1 | 0 |
| NDynamicObjectManager | 1 | 1 | 0 |
| NUdonChipsExchangeSystem | 1 | 1 | 0 |
| NChipsExchangeButton | 1 | 1 | 0 |
| NWeaponsManager | 1 | 1 | 0 |
| LightVolumeManager | 1 | 1 | 0 |
| UdonChipsAutoGain | 1 | 1 | 0 |
| UdonChipsMoveSpeed | 1 | 1 | 0 |
| UdonChipsLoginBonus | 1 | 1 | 0 |
| LTCGI_Controller | 1 | 1 | 0 |
| LTCGI_UdonAdapter | 1 | 1 | 0 |
| LV_LTCGI_Adapter | 1 | 1 | 0 |
| LV_LTCGI_EditorUpdator | 1 | 1 | 0 |
| PolybrushMesh | 1 | 0 | 1 |
| NBoothPoster | 1 | 0 | 0 |
| NUrlWindow | 1 | 0 | 0 |
| NServerErrorWindow | 1 | 0 | 0 |
| NUntrustedUrlsWindow | 1 | 0 | 0 |
| NAvatarNow | 1 | 1 | 0 |
| NLoadingManeger | 1 | 1 | 0 |
| NSelectorDecoder | 1 | 1 | 0 |
| NThumbnailDecoder | 1 | 1 | 0 |
| NAvatarSelector | 1 | 1 | 0 |
| NAudioControl | 1 | 1 | 0 |
| cuckoo_VRChatEventCalendar_v3 | 1 | 0 | 0 |
| FAquariumTank | 1 | 1 | 0 |
| EspressoMachine | 1 | 1 | 0 |
| EspressoMachineOptions | 1 | 1 | 0 |
| EspressoMachineMilkPitcherReceiver | 1 | 1 | 0 |
| EspressoMachinePortaFilterReceiver | 1 | 1 | 0 |
| EspressoMachineCupReceiver | 1 | 1 | 0 |
| EspressoMachineBrewLever | 1 | 1 | 0 |
| EspressoMachineWaterLever | 1 | 1 | 0 |
| EspressoMachineSteamLever | 1 | 1 | 0 |
| EspressoGrinder | 1 | 1 | 0 |
| EspressoGrinderManualSwitch | 1 | 1 | 0 |
| EspressoGrinderColliderReceiver | 1 | 1 | 0 |
| PortaFilter | 1 | 1 | 0 |
| PortaFilterSync | 1 | 1 | 0 |
| PortaFilterParticleReceiver | 1 | 1 | 0 |
| PortaFilterAttachDetector | 1 | 1 | 0 |
| Tamper | 1 | 1 | 0 |
| LatteCupSync | 1 | 1 | 0 |
| TabletSync | 1 | 1 | 0 |
| StudioStatusLight | 1 | 1 | 0 |
| StudioMachineController | 1 | 1 | 0 |
| StudioLever | 1 | 1 | 0 |
| StudioCupSocket | 1 | 1 | 0 |
| StudioCapsulePort | 1 | 1 | 0 |
| StudioResetButton | 1 | 1 | 0 |
| StudioRecipeLibrary | 1 | 1 | 0 |
| Microwave | 1 | 1 | 0 |
| FixedJoint | 1 | 1 | 0 |
| MicrowaveDoor | 1 | 1 | 0 |
| Microwave_Switch | 1 | 1 | 0 |
| DoorSystem | 1 | 1 | 0 |
| PortalLibrarySystem2 | 1 | 0 | 0 |
| CategorySelector | 1 | 0 | 0 |
| CategoryButton | 1 | 0 | 0 |
| WorldSelector | 1 | 0 | 0 |
| WorldButton | 1 | 0 | 0 |
| Information | 1 | 0 | 0 |
| WorldDataProcessor | 1 | 0 | 0 |
| JsonWorldData | 1 | 0 | 0 |
| StaticWorldData | 1 | 0 | 0 |
| Categorys | 1 | 0 | 0 |
| Roles | 1 | 0 | 0 |
| ElevatorState | 1 | 0 | 1 |
| MusicSequencer | 1 | 1 | 0 |
| CardKey | 1 | 0 | 0 |
| DoorSystem_Unlocker | 1 | 1 | 0 |
| DoorLock_Toggler | 1 | 1 | 0 |
| ForceRespawn_Lv2 | 1 | 1 | 0 |
| TeleportSystem | 1 | 1 | 0 |
| TeleportTrigger | 1 | 1 | 0 |
| LurasSimpleWaterSystem | 1 | 1 | 0 |
| HeadFollower | 1 | 1 | 0 |
| HotSpringSoundController | 1 | 1 | 0 |
| LurasVoiceShutter | 1 | 1 | 0 |
| NElevatorSystem | 1 | 1 | 0 |
| WIMCore | 1 | 0 | 1 |
| WorldChangelogModule | 1 | 0 | 1 |
| AssetListModule | 1 | 0 | 1 |
| FreeTextModule | 1 | 0 | 1 |
| JoinLogModule | 1 | 0 | 1 |
| PlayerListModule | 1 | 0 | 1 |
| SoundSettingsModule | 1 | 0 | 1 |
| SoundToggleHandler | 1 | 0 | 1 |
| VolumeChangeHandler | 1 | 0 | 1 |
| TeleportModule | 1 | 0 | 1 |
| TeleportHandler | 1 | 0 | 1 |
| NWIMChatModule | 1 | 0 | 1 |
| NWIMInventoryModule | 1 | 0 | 1 |
| HomeAppLinkHelper | 1 | 0 | 1 |
| ModalWindowHelper | 1 | 0 | 1 |
| Selectable | 1 | 0 | 1 |
| TutorialOverlayManager | 1 | 0 | 1 |
| QuickMenuManager | 1 | 0 | 1 |
| MobileQuickMenuToggleButton | 1 | 0 | 1 |
| UIManager | 1 | 0 | 1 |
| VersionInfoModule | 1 | 0 | 1 |
| TextRebuildHelper | 1 | 0 | 1 |
| SystemSettingsModule | 1 | 0 | 1 |
| CloudSyncModule | 1 | 0 | 1 |
| ThemeManager | 1 | 0 | 1 |
| CloudSyncUtils | 1 | 0 | 1 |
| CloudSyncManager | 1 | 0 | 1 |
| SitLine | 1 | 1 | 0 |
| FlekSit | 1 | 0 | 0 |
| UnyStylus | 1 | 0 | 0 |
| UnyStylusController | 1 | 0 | 0 |
| Pen | 1 | 0 | 0 |
| Eraser | 1 | 0 | 0 |
| LineSelector | 1 | 0 | 0 |
| ColorPicker | 1 | 0 | 0 |
| TACPointer | 1 | 0 | 0 |
| PenMenu | 1 | 0 | 0 |
| Menu_WidthSlider | 1 | 0 | 0 |
| Menu_PenMode | 1 | 0 | 0 |
| Menu_Clear | 1 | 0 | 0 |
| Menu_ColorWheel | 1 | 0 | 0 |
| Menu_Export | 1 | 0 | 0 |
| PenPopup | 1 | 0 | 0 |
| PlayerPopup | 1 | 0 | 0 |
| DesktopTextureChanger | 1 | 0 | 0 |
| WeatherSystem | 1 | 1 | 0 |
| TIM_QMTrigger | 1 | 1 | 0 |
| TIM_IMECore | 1 | 1 | 0 |
| TIM_IMEKeyFx | 1 | 1 | 0 |
| TIM_IMEPanelGrab | 1 | 1 | 0 |
| TIM_IMETranslate | 1 | 1 | 0 |
| TIM_IMEHangul | 1 | 1 | 0 |
| TIM_IMEBopomofo | 1 | 1 | 0 |
| TIM_IMEChatManager | 1 | 1 | 0 |
| TIM_IMEChatSlot | 1 | 0 | 0 |
| TIM_IMEQMButton | 1 | 1 | 0 |
| TimHoverLine | 1 | 1 | 0 |
| TIM_LocalizationManager | 1 | 1 | 0 |
| TIM_QMLocaleResolver | 1 | 1 | 0 |
| TIM_ButtonSettings | 1 | 1 | 0 |
| TIM_QMTextContent | 1 | 1 | 0 |
| TIM_QMWeatherUtils | 1 | 1 | 0 |
| TIM_QMWeatherData | 1 | 1 | 0 |
| TIM_QMWeatherView | 1 | 1 | 0 |
| TIM_QMCatButton | 1 | 1 | 0 |
| TIM_QMLuraButton | 1 | 1 | 0 |
| TIM_QMNameTagButton | 1 | 1 | 0 |
| TIM_QMTooltipControl | 1 | 1 | 0 |
| TIM_QMDatePanel | 1 | 1 | 0 |
| TIM_QMWhitelistManager | 1 | 0 | 0 |
| TIM_QMWhitelistObjectGate | 1 | 0 | 0 |
| TIM_QMWhitelistLayout | 1 | 0 | 0 |
| TIM_QMWhitelistPad | 1 | 0 | 0 |
| TIM_QMWhitelistPadRow | 1 | 0 | 0 |
| TIM_NameTagManager | 1 | 1 | 0 |
| TIM_NameTagIconObject | 1 | 0 | 0 |
| TIM_QMNameTagPreviewCam | 1 | 1 | 0 |
| TIM_QMNameTagPad | 1 | 1 | 0 |
| TIM_NameTagPanel | 1 | 1 | 0 |
| VRModeSwitch | 1 | 1 | 0 |
| ChatSystem | 1 | 1 | 0 |
| AnimatorToggle | 1 | 1 | 0 |
| SoundProofRoom | 1 | 0 | 1 |
| SoundProofRoomController | 1 | 0 | 1 |
| SataniaMicManager | 1 | 0 | 1 |
| ReverbFilter | 1 | 0 | 1 |
| AttenuationTool | 1 | 0 | 1 |
| AudioChannelManager | 1 | 0 | 1 |
| AudioChannelManagerPanel | 1 | 0 | 1 |
| AudioChannelPlayerList | 1 | 0 | 1 |
| DayCycleSystem | 1 | 0 | 1 |
| NDynamicYamaPlayerManager | 1 | 0 | 1 |
| QvPen_Settings | 1 | 0 | 1 |
| QvPen_ShowOrHideButton | 1 | 0 | 1 |
| QvPen_ResetAllButton | 1 | 0 | 1 |
| QvPen_ClearAllButton | 1 | 0 | 1 |
| TabletPickup | 1 | 0 | 1 |
| TabletManager | 1 | 0 | 1 |
| TabletCover | 1 | 0 | 1 |
| ColliderDetector | 1 | 0 | 1 |
| Home | 1 | 0 | 1 |
| JoinLog | 1 | 0 | 1 |
| Lock | 1 | 0 | 1 |
| Slideshow | 1 | 0 | 1 |
| DigitalClock | 1 | 0 | 1 |
| HomeButton | 1 | 0 | 1 |
| PointerModeChanger | 1 | 0 | 1 |
| CameraApp | 1 | 0 | 1 |
| PhotoViewer | 1 | 0 | 1 |
| VideoPlayer | 1 | 0 | 1 |
| PlayerLog | 1 | 0 | 1 |
| URLShare | 1 | 0 | 1 |
| TabletAppBehaviour | 1 | 0 | 1 |
| ScreenCast | 1 | 0 | 1 |
| CastScreenCard | 1 | 0 | 1 |
| Credit | 1 | 0 | 1 |
| VideoPlayerLinks | 1 | 0 | 1 |
| PortalManager | 1 | 0 | 1 |
| EnvironmentAgentManager | 1 | 0 | 1 |
| PlayerAdvancedTrackingDataProvider | 1 | 0 | 1 |
| LocomotionsManager | 1 | 0 | 1 |
| ClimbZoneController | 1 | 0 | 1 |
| ClimbZoneControllerVR | 1 | 0 | 1 |
| RiskyDice | 1 | 0 | 1 |
| DiceInfo | 1 | 0 | 1 |
| shishaStem | 1 | 0 | 1 |
| PWS_UdonIK | 1 | 0 | 1 |
| handlePickup | 1 | 0 | 1 |
| ownerHead | 1 | 0 | 1 |
| flavorList | 1 | 0 | 1 |
| tongue | 1 | 0 | 1 |
| charcoalHeater | 1 | 0 | 1 |
| heaterButton | 1 | 0 | 1 |
| pickUpTransfer | 1 | 0 | 1 |
| chacoalHolder | 1 | 0 | 1 |
| BowlList | 1 | 0 | 1 |
| HeatManagementList | 1 | 0 | 1 |
| hms | 1 | 0 | 1 |
| head | 1 | 0 | 1 |
| FishingRod | 1 | 0 | 1 |
| RodHandle1 | 1 | 0 | 1 |
| ReelHandle | 1 | 0 | 1 |
| Fish | 1 | 0 | 1 |
| KaraokeLink | 1 | 0 | 1 |
| MicLinkPickup | 1 | 0 | 1 |
| KaraokeReverb | 1 | 0 | 1 |
| KaraokeReverbArea | 1 | 0 | 1 |
| NameHide | 1 | 0 | 1 |
| CameraHide_LocalCamera | 1 | 0 | 1 |
| PotatoChips | 1 | 0 | 1 |
| PotatoChipsBag | 1 | 0 | 1 |
| UnpackController | 1 | 0 | 1 |
| UnpackPCUIDisplay | 1 | 0 | 1 |
| UnpackSlide | 1 | 0 | 1 |
| CustomFogHelper | 1 | 0 | 1 |
| RainVolumeController | 1 | 0 | 1 |
| LightProbeProxyVolume | 1 | 0 | 1 |
| RainAudioZone | 1 | 0 | 1 |
| WeatherController | 1 | 0 | 1 |
| ViewTrackerSettings | 1 | 0 | 1 |
| TrackingTargetManager | 1 | 0 | 1 |
| ScaleChanger | 1 | 0 | 1 |
| LeftWingToggle | 1 | 0 | 1 |
| RightWingToggle | 1 | 0 | 1 |
| PlayerViewTracker | 1 | 0 | 1 |
| PlayerViewCapture | 1 | 0 | 1 |
| CookingHolder | 1 | 0 | 1 |
| CookingItem | 1 | 0 | 1 |
| CookingItemReset | 1 | 0 | 1 |
| SlowSpeedArea | 1 | 0 | 1 |
| CalendarManager | 1 | 0 | 1 |
| time | 1 | 0 | 1 |
| date | 1 | 0 | 1 |
| ProgressBar | 1 | 0 | 1 |
| WheelControlledEngine | 1 | 0 | 1 |
| TillerHandleEngine | 1 | 0 | 1 |
| notificationsystem | 1 | 0 | 1 |
| Core | 1 | 0 | 1 |
| FrontendHandler | 1 | 0 | 1 |
| LanguageManager | 1 | 0 | 1 |
| ActiveRegionManager | 1 | 0 | 1 |
| RateLimitResolver | 1 | 0 | 1 |
| UIHandler | 1 | 0 | 1 |
| ScreenConfigurator | 1 | 0 | 1 |
| ColorConfig | 1 | 0 | 1 |
| VRCCanvasUtility | 1 | 0 | 1 |
| LaserTargetResizer | 1 | 0 | 1 |
| ColorTintAutoConfigurator | 1 | 0 | 1 |
| ToggleGroupHelper | 1 | 0 | 1 |
| LanguageSetter | 1 | 0 | 1 |
| VersionDisplay | 1 | 0 | 1 |
| ButtonEntry | 1 | 0 | 1 |
| LazySwitch | 1 | 0 | 1 |
| UdonCarSystem | 1 | 0 | 1 |
| UdonCarWheelVisual | 1 | 0 | 1 |
| SimplePickUpHide | 1 | 0 | 1 |
| VehicleHandle | 1 | 0 | 1 |
| UdonCarSeat | 1 | 0 | 1 |
| UdonCarSettings | 1 | 0 | 1 |
| UdonTimeAttack | 1 | 0 | 1 |
| UdonCarState | 1 | 0 | 1 |
| UsingStatusDisplay | 1 | 0 | 1 |
| UMoffPen2 | 1 | 0 | 1 |
| UMoffPen2Sys | 1 | 0 | 1 |
| UMoffPen2Settings | 1 | 0 | 1 |
| UMoffPen2UiThemeTool | 1 | 0 | 1 |
| SystemMain | 1 | 0 | 1 |
| CommManager | 1 | 0 | 1 |
| CommDataGroupManager | 1 | 0 | 1 |
| CanvasRenderCore | 1 | 0 | 1 |
| TouchableVisibilityController | 1 | 0 | 1 |
| UMoffPen2TouchableVisibilityEditorSync | 1 | 0 | 1 |
| Digitizer | 1 | 0 | 1 |
| AntiPostProcess | 1 | 0 | 1 |
| UGuiDigitizerRoot | 1 | 0 | 1 |
| UGuiRenderDistanceController | 1 | 0 | 1 |
| UGuiDrawingCanvas | 1 | 0 | 1 |
| UGuiDebugDisplay | 1 | 0 | 1 |
| UGuiColorPicker | 1 | 0 | 1 |
| UGuiTwoDimensionalSlider | 1 | 0 | 1 |
| UGuiToolPanel | 1 | 0 | 1 |
| UGuiLayerPanel | 1 | 0 | 1 |
| UGuiLayerCell | 1 | 0 | 1 |
| UGuiLayerControls | 1 | 0 | 1 |
| UGuiLayerPreviewPopup | 1 | 0 | 1 |
| UGuiMiscPanel | 1 | 0 | 1 |
| UGuiConfirmDialog | 1 | 0 | 1 |
| UGuiPassThroughBlocker | 1 | 0 | 1 |
| UGuiPenRaycaster | 1 | 0 | 1 |
| UGuiPenInteractor | 1 | 0 | 1 |
| Stylus | 1 | 0 | 1 |
| DropperCamera | 1 | 0 | 1 |
| ButtonDevice | 1 | 0 | 1 |
| ApplyOnPlayGlobalActivator | 1 | 1 | 0 |
| NConsole | 1 | 0 | 1 |
| PasswordEvent | 1 | 0 | 1 |
| Command | 1 | 0 | 1 |
| Chat | 1 | 0 | 1 |

## N系コンポーネントの全配置
Nで始まる型名を抽出した配置索引。名前がNで始まらない第三者Dependencyは上の全型索引に含まれる。
| key | パス | GameObject状態 | EditorOnly分類 | N型 |
|---|---|---|---|---|
| /0 | VRChat World Info | active | candidate | NAdvancedWorldSettings |
| /0/2/0 | VRChat World Info/N.Systems/N.Borders | active | candidate | NBorderManager |
| /0/2/0/0 | VRChat World Info/N.Systems/N.Borders/N.Border_01 | active | candidate | NBorder |
| /0/2/0/1 | VRChat World Info/N.Systems/N.Borders/N.Border_02 | active | candidate | NBorder |
| /0/2/0/2 | VRChat World Info/N.Systems/N.Borders/N.Border_03 | inactive | candidate | NBorder |
| /0/2/0/3 | VRChat World Info/N.Systems/N.Borders/N.Border_04 | active | candidate | NBorder |
| /0/2/0/4 | VRChat World Info/N.Systems/N.Borders/N.Border_05 | active | candidate | NBorder |
| /0/2/1 | VRChat World Info/N.Systems/N.VirtualInput | inactive | excluded | NVirtualInputManager |
| /0/2/2 | VRChat World Info/N.Systems/N.DoorSystem | active | candidate | NDoorSystem |
| /0/2/4 | VRChat World Info/N.Systems/N.SwimSystem | active | candidate | NSwimSystem |
| /0/2/5 | VRChat World Info/N.Systems/N.FlyingSystem | active | candidate | NFlyingSystem |
| /0/2/6 | VRChat World Info/N.Systems/N.StatusSystem | active | candidate | NStatusSystem |
| /0/2/7 | VRChat World Info/N.Systems/N.SecuritySystem | active | candidate | NSecuritySystem |
| /0/2/7/0/0 | VRChat World Info/N.Systems/N.SecuritySystem/N.SecurityZones/001 | active | candidate | NSecurityZone |
| /0/2/7/1/0 | VRChat World Info/N.Systems/N.SecuritySystem/N.SecurityObject Guarders/GameObject | active | candidate | NSecurityObjectGuard |
| /0/2/8 | VRChat World Info/N.Systems/N.InventorySystem | active | candidate | NInventoryManager |
| /0/2/9 | VRChat World Info/N.Systems/N.MovementSystem | active | candidate | NMovementSystem |
| /0/2/10 | VRChat World Info/N.Systems/N.DebugVisualization | inactive | excluded | NDebugVisualizationManager |
| /0/2/11 | VRChat World Info/N.Systems/N.Authority Level_Manager | active | candidate | NAuthorityLevelManager |
| /0/2/12 | VRChat World Info/N.Systems/N.Dynamic Object_Manager | active | candidate | NDynamicObjectManager |
| /0/2/13 | VRChat World Info/N.Systems/N.UdonChipsExchangeSystem | active | candidate | NUdonChipsExchangeSystem |
| /0/2/13/0 | VRChat World Info/N.Systems/N.UdonChipsExchangeSystem/N.ChipsExchangeButtonManager | active | candidate | NChipsExchangeButton |
| /0/2/14 | VRChat World Info/N.Systems/N.Weapons_Manager | active | candidate | NWeaponsManager |
| /0/3/4/1 | VRChat World Info/EventSystem/Currency_System/UdonGameChips | active | candidate | NUdonGameChips |
| /2/0/6/0/6/2/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster | inactive | candidate | NBoothPoster |
| /2/0/6/0/6/2/0/1/1/0/2/0/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1 | inactive | candidate | NBoothItemContainer, NGetBoothItemsRequest |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_1 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_1/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_1/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_2 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/1/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_2/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/1/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_2/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_3 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/2/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_3/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/2/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_3/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_4 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/3/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_4/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/1/3/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_1/Item_4/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2 | inactive | candidate | NBoothItemContainer, NGetBoothItemsRequest |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_1 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_1/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_1/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_2 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/1/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_2/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/1/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_2/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_3 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/2/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_3/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/2/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_3/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_4 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/3/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_4/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/2/3/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/LatestBoothItems_2/Item_4/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1 | inactive | candidate | NBoothItemContainer, NGetBoothItemsRequest |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_1 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_1/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_1/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_2 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/1/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_2/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/1/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_2/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_3 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/2/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_3/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/2/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_3/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_4 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/3/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_4/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/3/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_4/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_5 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/4/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_5/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/4/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_5/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/5 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_6 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/5/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_6/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/5/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_6/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/6 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_7 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/6/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_7/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/6/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_7/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/7 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_8 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/7/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_8/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/4/7/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_1/Item_8/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2 | inactive | candidate | NBoothItemContainer, NGetBoothItemsRequest |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_1 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_1/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_1/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_2 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/1/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_2/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/1/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_2/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_3 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/2/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_3/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/2/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_3/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_4 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/3/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_4/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/3/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_4/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_5 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/4/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_5/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/4/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_5/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/5 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_6 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/5/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_6/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/5/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_6/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/6 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_7 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/6/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_7/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/6/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_7/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/7 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_8 | inactive | candidate | NBoothItem, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/7/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_8/Tag/Tag_Center | inactive | candidate | NTagCenterWidth |
| /2/0/6/0/6/2/0/1/1/0/2/0/5/7/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/MainWindow/NewBoothItems_2/Item_8/Tag/Tag_Right | inactive | candidate | NTagRightXPosition |
| /2/0/6/0/6/2/0/1/1/0/2/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/URLWindow | inactive | candidate | NUrlWindow |
| /2/0/6/0/6/2/0/1/1/0/2/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/ServerErrorWindow | inactive | candidate | NServerErrorWindow |
| /2/0/6/0/6/2/0/1/1/0/2/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/Body/UntraustedUrlsWindow | inactive | candidate | NUntrustedUrlsWindow |
| /2/0/6/0/6/2/0/1/1/0/3/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/N.CategorySelector/PreviousCategory | inactive | candidate | NBoothCategoryButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/1/0/3/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.BoothPoster/BoothPosterCanvas/N.CategorySelector/NextCategory | inactive | candidate | NBoothCategoryButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow | active | candidate | NAvatarNow |
| /2/0/6/0/6/2/0/1/2/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/LoadingManeger | active | candidate | NLoadingManeger |
| /2/0/6/0/6/2/0/1/2/0/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/LoadingManeger/SelectorDecoder | active | candidate | NSelectorDecoder |
| /2/0/6/0/6/2/0/1/2/0/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/LoadingManeger/ThumbnailDecoder | active | candidate | NThumbnailDecoder |
| /2/0/6/0/6/2/0/1/2/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector | active | candidate | NAvatarSelector |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_1 | active | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_2 | active | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_3 | active | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_4 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_5 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/5 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_6 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/6 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_7 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/7 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_8 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/8 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_9 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/9 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_10 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/10 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_11 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/11 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_12 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/12 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_13 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/13 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_14 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/14 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_15 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/15 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_16 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/16 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_17 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/17 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_18 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/18 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_19 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/19 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_20 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/20 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_21 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/21 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_22 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/22 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_23 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/23 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_24 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/24 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_25 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/25 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_26 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/26 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_27 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/27 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_28 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/28 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_29 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/1/0/0/29 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Scroll View/Viewport/Content/EventButton_30 | inactive | candidate | NEventButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/0 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_1 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_2 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_3 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_4 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_5 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/5 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_6 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/6 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_7 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/7 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_8 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/8 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_9 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/9 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_10 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/10 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_11 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/3/11 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/ThumbnailButtons/ThumbnailButton_12 | active | candidate | NThumbnailButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/7/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Pagenation/AllowButton_R | active | candidate | NAllowButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/7/2 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Pagenation/AllowButton_L | active | candidate | NAllowButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/7/3 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Pagenation/AllowFastButton_R | active | candidate | NAllowButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/7/4 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/Pagenation/AllowFastButton_L | active | candidate | NAllowButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/0/8 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/MainUi/InfoButton | active | candidate | NShowSelectorUiButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/0/9/9 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/UiParent/InfoCover/InfoButton | inactive | candidate | NShowSelectorUiButton, NTouchPanelButton |
| /2/0/6/0/6/2/0/1/2/1/1 | World Layers/N.Luminous Hotel/Floor_7/EntranceArea/RestArea_Poster/WelcomeBoard_Monitor/RoomOuer_Monitor_Canvas/Overlay/N.AvatarNow/AvatarSelector/Audio Source | active | candidate | NAudioControl |
| /2/0/6/1/5/0/4/0/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_01_HousenBicha_HQ_Gimick/01_HousenBicha_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/0/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_01_HousenBicha_HQ_Gimick/01_HousenBicha_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/1/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_02_Housenbicha_Mini_HQ_Gimick/02_Housenbicha_Mini_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/1/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_02_Housenbicha_Mini_HQ_Gimick/02_Housenbicha_Mini_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/2/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_03_GravityTea_HQ_Gimick/03_GravityTea_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/2/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_03_GravityTea_HQ_Gimick/03_GravityTea_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/3/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_04_GravityTea_Mini_HQ_Gimick/04_GravityTea_Mini_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/3/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_04_GravityTea_Mini_HQ_Gimick/04_GravityTea_Mini_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/4/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_05_Antialias_HQ_Gimick/05_Antialias_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/4/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_05_Antialias_HQ_Gimick/05_Antialias_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/5/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_06_AntialiasZero_HQ_Gimick/06_AntialiasZero_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/5/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_06_AntialiasZero_HQ_Gimick/06_AntialiasZero_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/6/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_07_MeshCola_HQ_Gimick/07_MeshCola_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/6/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_07_MeshCola_HQ_Gimick/07_MeshCola_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/7/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_08_MeshColaZERO_HQ_Gimick/08_MeshColaZERO_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/7/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_08_MeshColaZERO_HQ_Gimick/08_MeshColaZERO_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/8/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_09_ColliderEnergy_HQ_Gimick/09_ColliderEnergy_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/8/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_09_ColliderEnergy_HQ_Gimick/09_ColliderEnergy_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/9/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_10_MeshColliderEnergy_HQ_Gimick/10_MeshColliderEnergy_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/9/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_10_MeshColliderEnergy_HQ_Gimick/10_MeshColliderEnergy_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/10/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_11_EmeraldTerrain_HQ_Gimick/11_EmeraldTerrain_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/10/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_11_EmeraldTerrain_HQ_Gimick/11_EmeraldTerrain_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/11/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_12_EmeraldTerrain_Blank_HQ_Gimick/12_EmeraldTerrain_Blank_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/11/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_12_EmeraldTerrain_Blank_HQ_Gimick/12_EmeraldTerrain_Blank_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/12/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_13_MeshCola_Mini_HQ_Gimick/13_MeshCola_Mini_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/12/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_13_MeshCola_Mini_HQ_Gimick/13_MeshCola_Mini_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/13/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_14_MeshColaZERO_Mini_HQ_Gimick/14_MeshColaZERO_Mini_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/13/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_14_MeshColaZERO_Mini_HQ_Gimick/14_MeshColaZERO_Mini_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/14/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_15_CraftBoss_MilkTea_HQ_Gimick/15_CraftBoss_MilkTea_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/14/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_15_CraftBoss_MilkTea_HQ_Gimick/15_CraftBoss_MilkTea_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/15/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_16_CraftBoss_Lemonade_HQ_Gimick/16_CraftBoss_Lemonade_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/15/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_16_CraftBoss_Lemonade_HQ_Gimick/16_CraftBoss_Lemonade_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/16/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_17_CraftBoss_CeylonTea_HQ_Gimick/17_CraftBoss_CeylonTea_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/16/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_17_CraftBoss_CeylonTea_HQ_Gimick/17_CraftBoss_CeylonTea_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/17/0 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_18_CraftBoss_FruitTea_HQ_Gimick/18_CraftBoss_FruitTea_HQ_Gimick_0 | inactive | candidate | NDynamicObject |
| /2/0/6/1/5/0/4/17/1 | World Layers/N.Luminous Hotel/Floor_7/RestSpace/GIMMICK/VendingMachines/VendingMachine_Pools/Pool_18_CraftBoss_FruitTea_HQ_Gimick/18_CraftBoss_FruitTea_HQ_Gimick_1 | inactive | candidate | NDynamicObject |
| /2/0/6/4/0/7/6/0/0/0/0 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Inner/Armature/Inner_Handle | active | candidate | NDoorPhysBoneHandleInput |
| /2/0/6/4/0/7/6/0/0/1 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Inner/CardKey_Inner | active | candidate | NDoorAuthZone |
| /2/0/6/4/0/7/6/0/0/3 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Inner/Entrance_Door_Inner | active | candidate | NDoorTeleportInput |
| /2/0/6/4/0/7/6/0/1/0/0 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Outer/Armature/Outer_Handle | active | candidate | NDoorPhysBoneHandleInput |
| /2/0/6/4/0/7/6/0/1/1 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Outer/CardKey_Outer | active | candidate | NDoorAuthZone |
| /2/0/6/4/0/7/6/0/1/3 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/Door_Anchor/Door_Outer/Entrance_Door_Outer | active | candidate | NDoorTeleportInput |
| /2/0/6/4/0/7/6/5/0 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/N.Desktop_Handle_Proxies/Inner_Handle(DeskTopOnly) | active | candidate | NDoorHandleInput |
| /2/0/6/4/0/7/6/5/1 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/DoorLocker_701/N.Desktop_Handle_Proxies/Outer_Handle(DeskTopOnly) | active | candidate | NDoorHandleInput |
| /2/0/6/4/0/7/7/0/1/1/1 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_1 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/2 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_2 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/3 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_3 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/4 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_4 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/5 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_5 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/6 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_6 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/7/0/1/1/7 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/MoodBoard/MoodBoard_701/SignPlate/SignPlate/SignPlate_7 | active | candidate | NDynamicObject |
| /2/0/6/4/0/7/8/0/0 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/AuthorityKey_RoomStands/AuthorityKeyStand_0/SnapAnchor | active | candidate | NDynamicObjectSnapPoint |
| /2/0/6/4/0/7/8/1/0 | World Layers/N.Luminous Hotel/Floor_7/PrivateRooms/PrivateRoom_701/Gimmicks/AuthorityKey_RoomStands/AuthorityKeyStand_1/SnapAnchor | active | candidate | NDynamicObjectSnapPoint |
| /2/0/24/0/2/3/1 | World Layers/N.Luminous Hotel/WelcomeBoard/WelcomeBoard_701/CardBox/CardBox_Mover/Snap_Anchor | active | candidate | NDynamicObjectSnapPoint |
| /2/0/24/1/2/3/1 | World Layers/N.Luminous Hotel/WelcomeBoard/WelcomeBoard_702/CardBox/CardBox_Mover/Snap_Anchor | active | candidate | NDynamicObjectSnapPoint |
| /2/0/26/0/0/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/R/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/1/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/9F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/2/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/8F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/3/0/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/7F/Elevator_Switch_Floor/Button_Square_Base | active | candidate | NElevatorButton |
| /2/0/26/0/4/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/6F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/5/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/5F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/6/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/4F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/7/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/3F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/8/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/2F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/9/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/1F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/10/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/B1/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/0/11/2/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_A/B2/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/0/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/R/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/1/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/9F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/2/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/8F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/3/0/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/7F/Elevator_Switch_Floor/Button_Square_Base | active | candidate | NElevatorButton |
| /2/0/26/1/4/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/6F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/5/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/5F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/6/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/4F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/7/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/3F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/8/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/2F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/9/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/1F/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/10/1/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/B1/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/1/11/2/0 | World Layers/N.Luminous Hotel/Elevators/Hierarchical_Coordinates_B/B2/Elevator_Switch_Floor/Button_Square_Base | inactive | excluded | NElevatorButton |
| /2/0/26/3/0/0/6/0 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_R | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/1 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_9 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/2 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_8 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/3 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_7 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/4 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_6 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/5 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_5 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/6 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_4 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/7 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_3 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/8 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_2 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/9 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_1 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/10 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_B1 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/11 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_B2 | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/12 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_Open | active | candidate | NElevatorButton |
| /2/0/26/3/0/0/6/13 | World Layers/N.Luminous Hotel/Elevators/Elevator_A/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_Close | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/0 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_R | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/1 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_9 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/2 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_8 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/3 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_7 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/4 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_6 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/5 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_5 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/6 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_4 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/7 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_3 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/8 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_2 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/9 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_1 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/10 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_B1 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/11 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_B2 | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/12 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_Open | active | candidate | NElevatorButton |
| /2/0/26/4/0/1/12/13 | World Layers/N.Luminous Hotel/Elevators/Elevator_B/MESH/Gondola/Elevator_Gondola_Buttons/Button_Square_Close | active | candidate | NElevatorButton |
| /2/0/26/5 | World Layers/N.Luminous Hotel/Elevators/N.ElevatorSystem | active | candidate | NElevatorSystem |
| /3/0/0/9/0 | Extra Assets/WorldIntegratedMenu/Modules/N_WIMChatModule/Content | inactive | excluded | NWIMChatModule |
| /3/0/0/10/0 | Extra Assets/WorldIntegratedMenu/Modules/N_WIMInventoryModule/Content | inactive | excluded | NWIMInventoryModule |
| /3/5 | Extra Assets/AuthorityKey | active | candidate | NDynamicObject |
| /3/6 | Extra Assets/UdonChipsWallet | active | candidate | NDynamicObject |
| /3/7 | Extra Assets/GameChipsWallet | active | candidate | NDynamicObject |
| /5/1 | -----OldExtra_Assets-----/N_DynamicYamaPlayerManager | inactive | excluded | NDynamicYamaPlayerManager |
| /5/8/0/0 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_1 | inactive | excluded | NDynamicObject |
| /5/8/0/1 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_2 | inactive | excluded | NDynamicObject |
| /5/8/0/2 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_3 | inactive | excluded | NDynamicObject |
| /5/8/0/3 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_4 | inactive | excluded | NDynamicObject |
| /5/8/0/4 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_5 | inactive | excluded | NDynamicObject |
| /5/8/0/5 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_6 | inactive | excluded | NDynamicObject |
| /5/8/0/6 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_7 | inactive | excluded | NDynamicObject |
| /5/8/0/7 | -----OldExtra_Assets-----/WisperShisha/Charcoals/Charcoal_8 | inactive | excluded | NDynamicObject |
| /5/8/1/0 | -----OldExtra_Assets-----/WisperShisha/Shisha/PickPoint | inactive | excluded | NDynamicObject |
| /5/8/1/1/0/0/0/5 | -----OldExtra_Assets-----/WisperShisha/Shisha/Shisha/Armature/shishaBottle/shishaStem/end | inactive | excluded | NDynamicObject |
| /5/8/2/0 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_MEBI | inactive | excluded | NDynamicObject |
| /5/8/2/1 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_WHITE | inactive | excluded | NDynamicObject |
| /5/8/2/2 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_TIRU | inactive | excluded | NDynamicObject |
| /5/8/2/3 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_PAREO | inactive | excluded | NDynamicObject |
| /5/8/2/4 | -----OldExtra_Assets-----/WisperShisha/Flavors/MISTARIA_EIKA | inactive | excluded | NDynamicObject |
| /5/8/2/5 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_AKANE | inactive | excluded | NDynamicObject |
| /5/8/2/6 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_TIKOKU | inactive | excluded | NDynamicObject |
| /5/8/2/7 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_MILK | inactive | excluded | NDynamicObject |
| /5/8/2/8 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_SENATI | inactive | excluded | NDynamicObject |
| /5/8/2/9 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_MOGI | inactive | excluded | NDynamicObject |
| /5/8/2/10 | -----OldExtra_Assets-----/WisperShisha/Flavors/AEROME_SINO | inactive | excluded | NDynamicObject |
| /5/8/2/11 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_HEARTBEAT | inactive | excluded | NDynamicObject |
| /5/8/2/12 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_CLOCK | inactive | excluded | NDynamicObject |
| /5/8/2/13 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_BIRD | inactive | excluded | NDynamicObject |
| /5/8/2/14 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_DROP | inactive | excluded | NDynamicObject |
| /5/8/2/15 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_FIRE | inactive | excluded | NDynamicObject |
| /5/8/2/16 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_RAIN | inactive | excluded | NDynamicObject |
| /5/8/2/17 | -----OldExtra_Assets-----/WisperShisha/Flavors/Noise_THANDER | inactive | excluded | NDynamicObject |
| /5/8/2/18 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_NATUKITUNE | inactive | excluded | NDynamicObject |
| /5/8/2/19 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_RAKURIMA | inactive | excluded | NDynamicObject |
| /5/8/2/20 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_SORARA | inactive | excluded | NDynamicObject |
| /5/8/2/21 | -----OldExtra_Assets-----/WisperShisha/Flavors/IGNIS_KRIS | inactive | excluded | NDynamicObject |
| /5/8/3 | -----OldExtra_Assets-----/WisperShisha/Tongs | inactive | excluded | NDynamicObject |
| /5/8/5 | -----OldExtra_Assets-----/WisperShisha/Charcoal_Basket | inactive | excluded | NDynamicObject |
| /5/8/6/0 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Ceramic_Bowl | inactive | excluded | NDynamicObject |
| /5/8/6/1 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Glass_Bowl | inactive | excluded | NDynamicObject |
| /5/8/6/2 | -----OldExtra_Assets-----/WisperShisha/Bowl_Holder/Silicone_Bowl | inactive | excluded | NDynamicObject |
| /5/8/7/0 | -----OldExtra_Assets-----/WisperShisha/Turkish_Lids/Turkish_Lid | inactive | excluded | NDynamicObject |
| /5/29 | -----OldExtra_Assets-----/N_UdonGameChips | inactive | excluded | NUdonGameChips |
| /8 | N.Console | inactive | excluded | NConsole |
