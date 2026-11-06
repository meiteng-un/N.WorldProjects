# 型付き参照のフィールド索引

C#上で型を特定できた 141 フィールド。シーンでの割り当て有無は別ページを参照。汎用 `UdonBehaviour`、UnityEvent、文字列イベント、外部アセットへの参照はこの抽出の対象外です。

<details>
<summary>N.AbilitySystem（6件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.AbilitySystem / NMaterialPotential.cs | `materialModifiers` | N.AbilitySystem / `NEntityAbilityState` |
| N.AbilitySystem / NEntityAbilityState.cs | `inheritanceParent` | N.AbilitySystem / `NEntityAbilityState` |
| N.AbilitySystem / NAbilitySystem.cs | `titleSystem` | N.TitleSystem / `NTitleSystem` |
| N.AbilitySystem / NAbilitySystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.AbilitySystem / NEnhancementProcess.cs | `inputMaterials` | N.AbilitySystem / `NMaterialPotential[]` |
| N.AbilitySystem / NEnhancementProcess.cs | `targetState` | N.AbilitySystem / `NEntityAbilityState` |

</details>

<details>
<summary>N.Console（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.Console / NConsole.cs | `gameChips` | N.UdonGameChips / `NUdonGameChips` |

</details>

<details>
<summary>N.DynamicObject（14件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.DynamicObject / NDynamicObjectSnapPoint.cs | `manager` | N.DynamicObject / `NDynamicObjectManager` |
| N.DynamicObject / NDynamicObjectPaymentTerminal.cs | `dynamicObjectManager` | N.DynamicObject / `NDynamicObjectManager` |
| N.DynamicObject / NDynamicObjectPaymentTerminal.cs | `gameChips` | N.UdonGameChips / `NUdonGameChips` |
| N.DynamicObject / NDynamicObjectManager.cs | `dynamicObjects` | N.DynamicObject / `NDynamicObject[]` |
| N.DynamicObject / NDynamicObjectManager.cs | `snapPoints` | N.DynamicObject / `NDynamicObjectSnapPoint[]` |
| N.DynamicObject / NDynamicObjectLoanPool.cs | `personalTemplate` | N.DynamicObject / `NDynamicObject` |
| N.DynamicObject / NDynamicObjectLoanPool.cs | `sharedItems` | N.DynamicObject / `NDynamicObject[]` |
| N.DynamicObject / NDynamicObject.cs | `manager` | N.DynamicObject / `NDynamicObjectManager` |
| N.DynamicObject / NDynamicObject.cs | `loanPool` | N.DynamicObject / `NDynamicObjectLoanPool` |
| N.DynamicObject / NDynamicObject.cs | `inventoryRecipeExtraOutputs` | N.DynamicObject / `NDynamicObject[]` |
| N.DynamicObject / NDynamicObject.cs | `inventoryPurchaseCostItems` | N.DynamicObject / `NDynamicObject[]` |
| N.DynamicObject / NDynamicObject.cs | `inventoryRecipeIngredients` | N.DynamicObject / `NDynamicObject[]` |
| N.DynamicObject / NDynamicObject.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.DynamicObject / NDynamicObject.cs | `initialFollowTarget` | N.DynamicObject / `NDynamicObject` |

</details>

<details>
<summary>N.Border（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.Border / NBorderManager.cs | `borders` | N.Border / `NBorder[]` |

</details>

<details>
<summary>N.Inventory（5件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.Inventory / NInventoryInserter.cs | `manager` | N.Inventory / `NInventoryManager` |
| N.Inventory / NInventoryManager.cs | `dynamicObjectManager` | N.DynamicObject / `NDynamicObjectManager` |
| N.Inventory / NInventoryManager.cs | `itemCatalog` | N.DynamicObject / `NDynamicObject[]` |
| N.Inventory / NInventoryStatusTestItem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.Inventory / NInventoryWithdrawButton.cs | `manager` | N.Inventory / `NInventoryManager` |

</details>

<details>
<summary>N.FishingSystem（11件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.FishingSystem / NFishingAquarium.cs | `acceptedPools` | N.FishingSystem / `NFishingItemPool[]` |
| N.FishingSystem / NFishingModule.cs | `item` | N.DynamicObject / `NDynamicObject` |
| N.FishingSystem / NFishingZone.cs | `catchItems` | N.DynamicObject / `NDynamicObject[]` |
| N.FishingSystem / NFishingCatchReceiver.cs | `inventory` | N.Inventory / `NInventoryManager` |
| N.FishingSystem / NFishingItemPool.cs | `inventory` | N.Inventory / `NInventoryManager` |
| N.FishingSystem / NFishingItemPool.cs | `definition` | N.DynamicObject / `NDynamicObject` |
| N.FishingSystem / NFishingItemPool.cs | `items` | N.DynamicObject / `NDynamicObject[]` |
| N.FishingSystem / NFishingSystem.cs | `dynamicObject` | N.DynamicObject / `NDynamicObject` |
| N.FishingSystem / NFishingSystem.cs | `catchReceiver` | N.FishingSystem / `NFishingCatchReceiver` |
| N.FishingSystem / NFishingSystem.cs | `zones` | N.FishingSystem / `NFishingZone[]` |
| N.FishingSystem / NFishingSystem.cs | `modules` | N.FishingSystem / `NFishingModule[]` |

</details>

<details>
<summary>N.DoorSystem（9件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.DoorSystem / NDoorTeleportInput.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.DoorSystem / NDoorSystem.cs | `dynamicObjectManager` | N.DynamicObject / `NDynamicObjectManager` |
| N.DoorSystem / NDoorSystem.cs | `cardStandPoints` | N.DynamicObject / `NDynamicObjectSnapPoint[]` |
| N.DoorSystem / NDoorSystem.cs | `temporaryWelcomeSnapPoint` | N.DynamicObject / `NDynamicObjectSnapPoint` |
| N.DoorSystem / NDoorPhysBoneHandleInput.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.DoorSystem / NDoorModeSwitch.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.DoorSystem / NDoorHandleInput.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.DoorSystem / NDoorCardKey.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.DoorSystem / NDoorAuthZone.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |

</details>

<details>
<summary>N.GimmickTransformationSystem（7件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.GimmickTransformationSystem / NWorldAnimatorMenuButton.cs | `manager` | N.GimmickTransformationSystem / `NWorldAnimatorParameterManager` |
| N.GimmickTransformationSystem / NWorldWeaponContactAction.cs | `controller` | N.GimmickTransformationSystem / `NWorldWeaponController` |
| N.GimmickTransformationSystem / NWorldWeaponController.cs | `weaponsManager` | N.WeaponsManager / `NWeaponsManager` |
| N.GimmickTransformationSystem / NWorldWeaponController.cs | `weaponState` | N.WeaponsManager / `NWeaponState` |
| N.GimmickTransformationSystem / NWorldWeaponController.cs | `desktopAnimatorActions` | N.GimmickTransformationSystem / `NWorldAnimatorMenuButton[]` |
| N.GimmickTransformationSystem / NWorldWeaponPhysBoneAnimatorBridge.cs | `controller` | N.GimmickTransformationSystem / `NWorldWeaponController` |
| N.GimmickTransformationSystem / NWorldWeaponPhysBoneAnimatorBridge.cs | `parameterManager` | N.GimmickTransformationSystem / `NWorldAnimatorParameterManager` |

</details>

<details>
<summary>N.DriftCorrection（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.DriftCorrection / NDriftCorrection.cs | `movementSystem` | N.MovementSystem / `NMovementSystem` |

</details>

<details>
<summary>N.FlyingSystem（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.FlyingSystem / NFlyingSystem.cs | `movementSystem` | N.MovementSystem / `NMovementSystem` |
| N.FlyingSystem / NFlyingSystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |

</details>

<details>
<summary>N.NavigateHierarchySystem（4件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.NavigateHierarchySystem / NNavigateHierarchySystem.cs | `floorPolicySystem` | N.ElevatorSystem / `NElevatorSystem` |
| N.NavigateHierarchySystem / NNavigateHierarchySystem.cs | `borders` | N.Border / `NBorder[]` |
| N.NavigateHierarchySystem / NNavigateHierarchySystem.cs | `lowerEntrance` | N.Border / `NBorder` |
| N.NavigateHierarchySystem / NNavigateHierarchySystem.cs | `upperEntrance` | N.Border / `NBorder` |

</details>

<details>
<summary>N.FarmerSimulation（3件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.FarmerSimulation / NFarmerSimulationPlot.cs | `seedItems` | N.DynamicObject / `NDynamicObject[]` |
| N.FarmerSimulation / NFarmerSimulationPlot.cs | `fertilizerItems` | N.DynamicObject / `NDynamicObject[]` |
| N.FarmerSimulation / NFarmerSimulationPlot.cs | `harvestVariants` | N.DynamicObject / `NDynamicObject[]` |

</details>

<details>
<summary>N.SecuritySystem（7件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.SecuritySystem / NSecurityZone.cs | `securitySystem` | N.SecuritySystem / `NSecuritySystem` |
| N.SecuritySystem / NSecuritySystem.cs | `zones` | N.SecuritySystem / `NSecurityZone[]` |
| N.SecuritySystem / NSecuritySystem.cs | `objectGuards` | N.SecuritySystem / `NSecurityObjectGuard[]` |
| N.SecuritySystem / NSecurityObjectGuard.cs | `securitySystem` | N.SecuritySystem / `NSecuritySystem` |
| N.SecuritySystem / NSecurityObjectGuard.cs | `dynamicObject` | N.DynamicObject / `NDynamicObject` |
| N.SecuritySystem / NSecurityObjectGuard.cs | `allowedZones` | N.SecuritySystem / `NSecurityZone[]` |
| N.SecuritySystem / NSecurityObjectGuard.cs | `forbiddenZones` | N.SecuritySystem / `NSecurityZone[]` |

</details>

<details>
<summary>N.MovementSystem（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.MovementSystem / NMovementSystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |

</details>

<details>
<summary>N.RoomRespawnSystem（5件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.RoomRespawnSystem / NRoomRespawnSystem.cs | `roomPoints` | N.RoomRespawnSystem / `NRoomReturnPoint[]` |
| N.RoomRespawnSystem / NRoomRespawnSystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.RoomRespawnSystem / NRoomReturnPoint.cs | `doorSystem` | N.DoorSystem / `NDoorSystem` |
| N.RoomRespawnSystem / NRoomReturnPoint.cs | `cardStand` | N.DynamicObject / `NDynamicObjectSnapPoint` |
| N.RoomRespawnSystem / NRoomReturnPoint.cs | `identityCardTemplate` | N.DynamicObject / `NDynamicObject` |

</details>

<details>
<summary>N.ElevatorSystem（5件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.ElevatorSystem / NElevatorSystem.cs | `dynamicObjectManager` | N.DynamicObject / `NDynamicObjectManager` |
| N.ElevatorSystem / NElevatorSystem.cs | `manualDynamicObjects` | N.DynamicObject / `NDynamicObject[]` |
| N.ElevatorSystem / NElevatorSystem.cs | `autoCollectedButtons` | N.ElevatorSystem / `NElevatorButtonsManager[]` |
| N.ElevatorSystem / NElevatorSystem.cs | `manualButtonOverrides` | N.ElevatorSystem / `NElevatorButtonsManager[]` |
| N.ElevatorSystem / NElevatorButtonsManager.cs | `elevatorSystem` | N.ElevatorSystem / `NElevatorSystem` |

</details>

<details>
<summary>N.RTabIntegration（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.RTabIntegration / NRTabRecipeBook.cs | `inventory` | N.Inventory / `NInventoryManager` |
| N.RTabIntegration / NRTabRecipeBook.cs | `publishedRecipes` | N.DynamicObject / `NDynamicObject[]` |

</details>

<details>
<summary>N.VirtualInput（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.VirtualInput / NVirtualInputContactGate.cs | `manager` | N.VirtualInput / `NVirtualInputManager` |
| N.VirtualInput / NVirtualInputPhysBoneGate.cs | `manager` | N.VirtualInput / `NVirtualInputManager` |

</details>

<details>
<summary>N.WorldEntry（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.WorldEntry / NWorldEntry.cs | `worldReveal` | N.WorldEntry / `NWorldMeshReveal` |

</details>

<details>
<summary>N.MainMenu（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.MainMenu / NIntegratedMenuPointer.cs | `windows` | N.MainMenu / `NMainMenuFollower[]` |
| N.MainMenu / NMainMenuFollower.cs | `lifecycleOwner` | N.MainMenu / `NMainMenuFollower` |

</details>

<details>
<summary>N.SwimSystem（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.SwimSystem / NSwimSystem.cs | `movementSystem` | N.MovementSystem / `NMovementSystem` |
| N.SwimSystem / NSwimSystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |

</details>

<details>
<summary>N.UdonChipsExchangeSystem（2件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.UdonChipsExchangeSystem / NUdonChipsExchangeSystem.cs | `BalancesReference` | N.UdonGameChips / `NUdonGameChips` |
| N.UdonChipsExchangeSystem / NChipsExchangeButton.cs | `ExchangeSystem` | N.UdonChipsExchangeSystem / `NUdonChipsExchangeSystem` |

</details>

<details>
<summary>N.VehicleManager（12件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.VehicleManager / NAircraftSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NBoatSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NCarSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NDroneSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NFighterSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NHelicopterSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NMotorcycleSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NTrainSystem.cs | `vehicleControl` | N.VehicleManager / `NVehicleSystem` |
| N.VehicleManager / NVehicleSystem.cs | `vehicleManager` | N.VehicleManager / `NVehicleManager` |
| N.VehicleManager / NVehicleManager.cs | `movementSystem` | N.MovementSystem / `NMovementSystem` |
| N.VehicleManager / NVehicleManager.cs | `swimSystem` | N.SwimSystem / `NSwimSystem` |
| N.VehicleManager / NVehicleManager.cs | `flyingSystem` | N.FlyingSystem / `NFlyingSystem` |

</details>

<details>
<summary>N.WeaponsManager（3件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.WeaponsManager / NWeaponState.cs | `manager` | N.WeaponsManager / `NWeaponsManager` |
| N.WeaponsManager / NWeaponState.cs | `dynamicObject` | N.DynamicObject / `NDynamicObject` |
| N.WeaponsManager / NWeaponsManager.cs | `weapons` | N.WeaponsManager / `NWeaponState[]` |

</details>

<details>
<summary>N.TitleSystem（1件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.TitleSystem / NTitleSystem.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |

</details>

<details>
<summary>N.WIMExtensions（22件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.WIMExtensions / NWIMCraftPage.cs | `shell` | N.WIMExtensions / `NWIMMenuShell` |
| N.WIMExtensions / NWIMCraftPage.cs | `recipes` | N.DynamicObject / `NDynamicObject[]` |
| N.WIMExtensions / NWIMEquipmentPage.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.WIMExtensions / NWIMEquipmentPage.cs | `inventoryManager` | N.Inventory / `NInventoryManager` |
| N.WIMExtensions / NWIMInventoryModule.cs | `inventoryManager` | N.Inventory / `NInventoryManager` |
| N.WIMExtensions / NWIMInventoryModule.cs | `gameChips` | N.UdonGameChips / `NUdonGameChips` |
| N.WIMExtensions / NWIMInventoryModule.cs | `exchangeSystem` | N.UdonChipsExchangeSystem / `NUdonChipsExchangeSystem` |
| N.WIMExtensions / NWIMInventoryModule.cs | `statusSystem` | N.StatusSystem / `NStatusSystem` |
| N.WIMExtensions / NWIMInventoryModule.cs | `menuShell` | N.WIMExtensions / `NWIMMenuShell` |
| N.WIMExtensions / NWIMMenuShell.cs | `linkedShells` | N.WIMExtensions / `NWIMMenuShell[]` |
| N.WIMExtensions / NWIMMenuShell.cs | `inventoryView` | N.WIMExtensions / `NWIMInventoryModule` |
| N.WIMExtensions / NWIMMenuShell.cs | `exchangeSystem` | N.UdonChipsExchangeSystem / `NUdonChipsExchangeSystem` |
| N.WIMExtensions / NWIMMenuShell.cs | `swimSystem` | N.SwimSystem / `NSwimSystem` |
| N.WIMExtensions / NWIMMenuShell.cs | `flyingSystem` | N.FlyingSystem / `NFlyingSystem` |
| N.WIMExtensions / NWIMMenuShell.cs | `shopPage` | N.WIMExtensions / `NWIMShopPage` |
| N.WIMExtensions / NWIMMenuShell.cs | `mapPage` | N.WIMExtensions / `NWIMMapPage` |
| N.WIMExtensions / NWIMMenuShell.cs | `settingsPage` | N.WIMExtensions / `NWIMSettingsPage` |
| N.WIMExtensions / NWIMMenuShell.cs | `equipmentPage` | N.WIMExtensions / `NWIMEquipmentPage` |
| N.WIMExtensions / NWIMMenuShell.cs | `craftPage` | N.WIMExtensions / `NWIMCraftPage` |
| N.WIMExtensions / NWIMMenuShell.cs | `adminFishingDebugSessionOwner` | N.WIMExtensions / `NWIMMenuShell` |
| N.WIMExtensions / NWIMShopPage.cs | `sceneProducts` | N.DynamicObject / `NDynamicObject[]` |
| N.WIMExtensions / NWIMShopPage.cs | `sceneRecipes` | N.DynamicObject / `NDynamicObject[]` |

</details>

<details>
<summary>N.VirtualLensWorld（10件）</summary>

| 参照元 | フィールド | 参照先 |
|---|---|---|
| N.VirtualLensWorld / NPersonalCameraInstance.cs | `inventory` | N.Inventory / `NInventoryManager` |
| N.VirtualLensWorld / NPersonalCameraInstance.cs | `item` | N.DynamicObject / `NDynamicObject` |
| N.VirtualLensWorld / NPersonalCameraInstance.cs | `loanPool` | N.DynamicObject / `NDynamicObjectLoanPool` |
| N.VirtualLensWorld / NPersonalCameraService.cs | `personalTemplate` | N.VirtualLensWorld / `NPersonalCameraInstance` |
| N.VirtualLensWorld / NPersonalCameraService.cs | `catalogDefinition` | N.DynamicObject / `NDynamicObject` |
| N.VirtualLensWorld / NPersonalCameraService.cs | `loanPool` | N.DynamicObject / `NDynamicObjectLoanPool` |
| N.VirtualLensWorld / NPersonalCameraService.cs | `inventory` | N.Inventory / `NInventoryManager` |
| N.VirtualLensWorld / NPersonalCameraService.cs | `exchangeSystem` | N.UdonChipsExchangeSystem / `NUdonChipsExchangeSystem` |
| N.VirtualLensWorld / NVirtualLensWorld.cs | `operationSource` | N.DynamicObject / `NDynamicObject` |
| N.VirtualLensWorld / NVirtualLensWorld.cs | `optics` | N.VirtualLensWorld / `NWorldCameraOptics` |

</details>
