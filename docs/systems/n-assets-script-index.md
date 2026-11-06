# N.Assets 全C#ファイル索引
2026-10-12。全ファイルを読取・SHA256記録し、宣言と呼出しの構造を抽出。正規表現による静的索引で、全メソッドの意味・実操作の検証結果ではない。Dependency、EditorをRuntimeと分ける。公開API欄は先頭8件の抜粋、全公開API数は別記。

## N.AdvancedWorldSettings

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.AdvancedWorldSettings/NAdvancedWorldSettingsEditor.cs | Editor / 651 | NAdvancedWorldSettingsEditor, NAdvancedWorldSettingsSetup | UdonSharpBehaviour[], UdonSharpBehaviour |  / synced=0 / — |  | PreviewMigration, MigrateActiveSceneMenu, MigrateActiveScene, EnsureProgramAsset, AutoCollectAndWire / 5 |
| Assets/N.Assets/N.Script/N.AdvancedWorldSettings/NAdvancedWorldSettings.cs | Runtime / 397 | NAdvancedWorldSettings | NDynamicObjectManager, NMovementSystem, NStatusSystem, NSwimSystem, NFlyingSystem, UdonSharpBehaviour, UdonSharpBehaviour[], NAdvancedWorldSettingsInitializeEyeHeightTypes | NoVariableSync / synced=0 / — | Start, OnPlayerJoined | OnPlayerJoined, OnAvatarChanged, OnAvatarEyeHeightChanged, ConfigureLinkedSystems, ScheduleDerivedSystemsRefresh, RefreshDerivedSystems, ReapplyLocalSettings / 7 |

## N.AvatarNow

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.AvatarNow/NAvatarNowEditors.cs | Editor / 191 | NAvatarNowEditorBase, NAvatarNowEditor, NLoadingManegerEditor, NSelectorDecoderEditor, NThumbnailDecoderEditor, NAvatarSelectorEditor, NEventButtonEditor, NThumbnailButtonEditor, NAllowButtonEditor, NShowSelectorUiButtonEditor, NAudioControlEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.AvatarNow/NAvatarNowSceneMigration.cs | Editor / 569 | NAvatarNowSceneMigration | UdonSharpBehaviour[] |  / synced=0 / — |  | Preview, EnsureProgramAssets, Migrate, RepairCurrentSceneNAvatarReferences / 4 |
| Assets/N.Assets/N.Script/N.AvatarNow/Core/Decoders/NSelectorDecoder.cs | Runtime / 295 | NSelectorDecoder |  |  / synced=0 / — |  | GetSelectorInfo, OnStringLoadSuccess, OnStringLoadError, PreSplitString, JsonDecode, MakeEventBunnerPrepare, MakeOneEventBunner, DecodeComplete / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Core/Decoders/NThumbnailDecoder.cs | Runtime / 366 | NThumbnailDecoder | UdonSharpBehaviour |  / synced=0 / — | Start | GetThumbnail, OnStringLoadSuccess, OnStringLoadError, PreSplitString, JsonDecode, MakeTexturesBytesPrepare, MakeOneTextureBytes, MakeThumbnailAndPushBuffer / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Core/Loading/NLoadingManeger.cs | Runtime / 77 | NLoadingManeger | NSelectorDecoder, NThumbnailDecoder | NoVariableSync / synced=0 / — |  | TrySelectorDecodeStart, OnSelectorDecodeEnd, TryGetThumbnailStart, OnThumbnailDecodeEnd / 4 |
| Assets/N.Assets/N.Script/N.AvatarNow/Core/NAvatarNow.cs | Runtime / 261 | NAvatarNow | NLoadingManeger, NAvatarSelector | Manual / synced=1 / — | Start, Update | OnSelectorDecodeEnd, OnPushSyncButton, OnPushSelectLockButton, ChangeSyncValue, ApplySyncSharedIndex, OnThumbnaiDecodeEnd / 6 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/AvatarSelector.cs | Dependency / 388 | AvatarSelector |  |  / synced=0 / — |  | OnPushAllowButton, SelectThumnailButtons, OnPushEventButton, SelectIdLockUI, ViewUI, OnPushThumbnailButton, SelectThumbnail, InitAvatarSelector / 15 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/Button/AllowButton.cs | Dependency / 77 | AllowButton |  |  / synced=0 / — | Start, OnEnable | OnOver, OnExit, OnPush, OnRelease, OnClick, ButtonEnable / 6 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/Button/EventButton.cs | Dependency / 33 | EventButton |  |  / synced=0 / — |  | SetEventButton, SetCheckMark, OnPush / 3 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/Button/ShowSelectorUiButton.cs | Dependency / 21 | ShowSelectorUiButton |  |  / synced=0 / — |  | OnPush / 1 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/Common/SwitchDebug.cs | Dependency / 14 | SwitchDebug |  |  / synced=0 / — |  | Log / 1 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarSelector/Script/Common/ThumbnailButton.cs | Dependency / 115 | ThumbnailButton |  |  / synced=0 / — | Start, OnEnable | SetSelected, SetThumbnailButton, OnOver, OnExit, OnPush, OnRelease, ButtonEnable, OnClick / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/AvatarViewer/Script/AvatarViewer.cs | Dependency / 70 | AvatarViewer |  |  / synced=0 / — |  | SetAvatarView, SetLoadingCover / 2 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/AvatarNow.cs | Dependency / 269 | AvatarNow |  | Manual / synced=1 / — | Start, Update | OnSelectorDecodeEnd, OnPushSyncButton, OnPushSelectLockButton, ChangeSyncValue, ApplySyncSharedIndex, OnThumbnaiDecodeEnd / 6 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/LoadingManager/LoadingManeger.cs | Dependency / 76 | LoadingManeger |  | NoVariableSync / synced=0 / — |  | TrySelectorDecodeStart, OnSelectorDecodeEnd, TryGetThumbnailStart, OnThumbnailDecodeEnd / 4 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/LoadingManager/LoadingManegerCallBack.cs | Dependency / 17 | LoadingManegerCallBack |  | NoVariableSync / synced=0 / — |  | OnSelectorDecodeEnd, OnThumbnaiDecodeEnd / 2 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/SelectorDecoder/SelectorDecoder.cs | Dependency / 303 | SelectorDecoder |  |  / synced=0 / — |  | GetSelectorInfo, OnStringLoadSuccess, OnStringLoadError, PreSplitString, JsonDecode, MakeEventBunnerPrepare, MakeOneEventBunner, DecodeComplete / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/SelectorDecoder/Type/AvatarInfo.cs | Dependency / 74 | AvatarInfo, AvatarInfoExt |  |  / synced=0 / — |  | New, ThumbnailUrlIndex, ThumbnailUrlInnerIndex, AvatarNameJP, BluePrintID, CircleNameJP, AvatarURL, Index / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/SelectorDecoder/Type/EventInfo.cs | Dependency / 84 | EventInfo, EventInfoInfoExt |  |  / synced=0 / — |  | New, EventName, EventTypeName, ActiveEvent, ValidEvent, BannerDataStart, BannerDataLength, AvatarInfos / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/SelectorDecoder/Type/SelectorInfo.cs | Dependency / 54 | SelectorInfo, SelectorInfoExt |  |  / synced=0 / — |  | New, EventInfos / 2 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/ThumbnailDecoder/ThumbnailDecoder.cs | Dependency / 374 | ThumbnailDecoder | UdonSharpBehaviour |  / synced=0 / — | Start | GetThumbnail, OnStringLoadSuccess, OnStringLoadError, PreSplitString, JsonDecode, MakeTexturesBytesPrepare, MakeOneTextureBytes, MakeThumbnailAndPushBuffer / 8 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/ThumbnailDecoder/Type/ThumbnailBuff.cs | Dependency / 31 | ThumbnailBuff, ThumbnailBuffExt |  |  / synced=0 / — |  | New, UrlIndex, ThumbnailBytes / 3 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/ThumbnailDecoder/Type/ThumbnailData.cs | Dependency / 39 | ThumbnailData, ThumbnailDataExt |  |  / synced=0 / — |  | New, StartIndex, DataLength / 3 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Core/ThumbnailDecoder/Type/ThumbnailInfo.cs | Dependency / 40 | ThumbnailInfo, ThumbnailInfoExt |  |  / synced=0 / — |  | New, ThumbnailData / 2 |
| Assets/N.Assets/N.Script/N.AvatarNow/Dependency/Decoder/Other/Sound/AudioControl.cs | Dependency / 34 | AudioControl |  |  / synced=0 / — |  | Open, Close, Select1, Select2, Select3 / 5 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NAllowButton.cs | Runtime / 78 | NAllowButton | NAvatarSelector |  / synced=0 / — | Start, OnEnable | OnOver, OnExit, OnPush, OnRelease, OnClick, ButtonEnable / 6 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NAudioControl.cs | Runtime / 36 | NAudioControl |  |  / synced=0 / — |  | Open, Close, Select1, Select2, Select3 / 5 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NAvatarSelector.cs | Runtime / 400 | NAvatarSelector | NAvatarNow, NAudioControl, NLoadingManeger |  / synced=0 / — |  | OnPushAllowButton, SelectThumnailButtons, OnPushEventButton, SelectIdLockUI, ViewUI, OnPushThumbnailButton, SelectThumbnail, InitAvatarSelector / 15 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NEventButton.cs | Runtime / 34 | NEventButton | NAvatarSelector |  / synced=0 / — |  | SetEventButton, SetCheckMark, OnPush / 3 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NShowSelectorUiButton.cs | Runtime / 23 | NShowSelectorUiButton |  |  / synced=0 / — |  | OnPush / 1 |
| Assets/N.Assets/N.Script/N.AvatarNow/UI/NThumbnailButton.cs | Runtime / 137 | NThumbnailButton | NAvatarSelector, NAudioControl |  / synced=0 / — | Start, OnEnable | SetSelected, SetThumbnailButton, OnOver, OnExit, OnPush, OnRelease, ButtonEnable, OnClick / 8 |

## N.BoothPoster

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.BoothPoster/NBoothPosterAssetBuilder.cs | Editor / 99 | NBoothPosterAssetBuilder |  |  / synced=0 / — |  | BuildFromMenu, EnsureProgramAssets / 2 |
| Assets/N.Assets/Editor/N.BoothPoster/NBoothPosterEditors.cs | Editor / 178 | NBoothPosterEditorBase, NBoothPosterEditor, NBoothItemContainerEditor, NGetBoothItemsRequestEditor, NBoothItemEditor, NBoothCategoryButtonEditor, NTagCenterWidthEditor, NTagRightXPositionEditor, NUrlWindowEditor, NServerErrorWindowEditor, NUntrustedUrlsWindowEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.BoothPoster/NBoothPosterInteractionBuilder.cs | Editor / 217 | NBoothPosterInteractionBuilder | NBoothCategoryButton |  / synced=0 / — |  | BuildCurrentScene / 1 |
| Assets/N.Assets/Editor/N.BoothPoster/NBoothPosterMigration.cs | Editor / 275 | NBoothPosterMigration | UdonSharpBehaviour[] |  / synced=0 / — |  | Preview, MigrateFirstInOpenScene, Migrate / 3 |
| Assets/N.Assets/N.Script/N.BoothPoster/NBoothCategoryButton.cs | Runtime / 47 | NBoothCategoryButton | NBoothPoster, NBoothCategoryButtonDirection | None / synced=0 / — | Start | Activate, Interact, ConfigureEditor / 3 |
| Assets/N.Assets/N.Script/N.BoothPoster/NBoothItem.cs | Runtime / 126 | NBoothItem | NUrlWindow | None / synced=0 / — | Start | UpdateItemInfo, SetAtlasTexture, SetEmptyItemInfo, ResetItem, SetLoading, OnPushButton, SetCategoryDisplay, SetUrlWindow / 10 |
| Assets/N.Assets/N.Script/N.BoothPoster/NBoothItemContainer.cs | Runtime / 207 | NBoothItemContainer | NBoothItem[], NGetBoothItemsRequest, NServerErrorWindow, NUntrustedUrlsWindow, NBoothContainerEntryType | None / synced=0 / — | Start | UpdateItems, SetRuntimeCategory, OnStringLoadSuccess, OnStringLoadError, ConfigureDependencies, RebuildItemReferences, ConfigureEntryTypeFromName, SetModelCategory / 9 |
| Assets/N.Assets/N.Script/N.BoothPoster/NBoothPoster.cs | Runtime / 166 | NBoothPoster | NBoothModelCategory, NBoothItemContainer[], NServerErrorWindow[], NUntrustedUrlsWindow[], NBoothCategoryButton[] | Manual / synced=1 / — | Start, Update, OnDeserialization | UpdateContainers, SelectPreviousCategory, SelectNextCategory, SelectCategory, OnDeserialization, RebuildReferencesAndApply, SetCategoryUi / 7 |
| Assets/N.Assets/N.Script/N.BoothPoster/NBoothPosterEnums.cs | Runtime / 74 | NBoothPosterEnums | NBoothModelCategory |  / synced=0 / — |  | GetJapanese, ParseCategory / 2 |
| Assets/N.Assets/N.Script/N.BoothPoster/NGetBoothItems.cs | Runtime / 75 | NGetBoothItems, NGetBoothItemsExt | NGetBoothItems, NGetBoothItemsEntry[], NGetBoothItemsImage |  / synced=0 / — |  | New, TryFromJson, Items, Image / 4 |
| Assets/N.Assets/N.Script/N.BoothPoster/NGetBoothItemsEntry.cs | Runtime / 50 | NGetBoothItemsEntry, NGetBoothItemsEntryExt | NGetBoothItemsEntry |  / synced=0 / — |  | New, TryFromJson, Title, Url, ShopName, SubCategory / 6 |
| Assets/N.Assets/N.Script/N.BoothPoster/NGetBoothItemsImage.cs | Runtime / 45 | NGetBoothItemsImage, NGetBoothItemsImageExt | NGetBoothItemsImage |  / synced=0 / — |  | New, TryFromJson, ImageBase64, Width, Height / 5 |
| Assets/N.Assets/N.Script/N.BoothPoster/NGetBoothItemsRequest.cs | Runtime / 86 | NGetBoothItemsRequest |  | None / synced=0 / — |  | SendRequest, SetCategoryIndex, OnSuccess, TryGetData, OnFailed, SetRequestUrl, SetCategoryRequestUrls / 7 |
| Assets/N.Assets/N.Script/N.BoothPoster/NServerErrorWindow.cs | Runtime / 24 | NServerErrorWindow |  | None / synced=0 / — |  | Open, Close / 2 |
| Assets/N.Assets/N.Script/N.BoothPoster/NTagCenterWidth.cs | Runtime / 28 | NTagCenterWidth |  | None / synced=0 / — | Start, Update |  / 0 |
| Assets/N.Assets/N.Script/N.BoothPoster/NTagRightXPosition.cs | Runtime / 20 | NTagRightXPosition |  | None / synced=0 / — | Update |  / 0 |
| Assets/N.Assets/N.Script/N.BoothPoster/NUntrustedUrlsWindow.cs | Runtime / 43 | NUntrustedUrlsWindow |  | None / synced=0 / — | Start | Open, Close, OnEnterInput / 3 |
| Assets/N.Assets/N.Script/N.BoothPoster/NUrlWindow.cs | Runtime / 36 | NUrlWindow |  | None / synced=0 / — |  | Open, Close, OnEnterInput / 3 |

## N.Border

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.Border/NBorderAssetBuilder.cs | Editor / 164 | NBorderAssetBuilder |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.Border/NBorderEditor.cs | Editor / 1165 | NBorderEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.Border/NBorderManagerEditor.cs | Editor / 339 | NBorderManagerEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.Border/NBorderShaderGUI.cs | Editor / 20 | NBorderShaderGUI |  |  / synced=0 / — |  | OnGUI / 1 |
| Assets/N.Assets/N.Script/N.Border/NBorder.cs | Runtime / 904 | NBorder | NBorderManager, UdonSharpBehaviour | Manual / synced=0 / — | Start, OnDeserialization | IsLocalPassable, IsMaintenanceMode, GetExternalOverride, InitializeBorder, OnContactEnter, OnContactExit, PeriodicRefresh, OnDeserialization / 28 |
| Assets/N.Assets/N.Script/N.Border/NBorderManager.cs | Runtime / 114 | NBorderManager | NBorder[], UdonSharpBehaviour[] | Manual / synced=0 / — | Start, OnDeserialization | InitializeManager, OnDeserialization, GetGlobalExternalOverride, IsValidGroup, HasConfiguredGroups, IsGroupEnabled, RefreshAllBorders, ApplySharedMaterialSettings / 13 |

## N.CalibrationSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.CalibrationSystem/Editor/NCalibrationSystemEditor.cs | Editor / 80 | NCalibrationSystemEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.CalibrationSystem/Runtime/NCalibrationSystem.cs | Runtime / 137 | NCalibrationSystem | UdonBehaviour | None / synced=0 / — | Start | Interact, Calibrate, ResetCalibration / 3 |

## N.CocktailLiquidSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.CocktailLiquidSystem/NCocktailLiquidShapeBaker.cs | Editor / 386 | NCocktailLiquidShapeBaker |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.CocktailLiquidSystem/NCocktailLiquidBridge.cs | Runtime / 151 | NCocktailLiquidBridge |  | None / synced=0 / — | Start, Update | BeginCocktail, ReceiveUnit, GetLiquidUnits, ResetLiquid / 4 |

## N.Console

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.Console/NConsoleAssetBuilder.cs | Editor / 70 | NConsoleAssetBuilder |  |  / synced=0 / — |  | CompileProgram / 1 |
| Assets/N.Assets/Editor/N.Console/NConsoleEditor.cs | Editor / 179 | NConsoleEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.Console/NConsole.cs | Runtime / 393 | NConsole | UdonSharpBehaviour, NUdonGameChips, UdonSharpBehaviour[] | None / synced=0 / — | Start | OnEndEdit, SubmitCommand, ExecuteCommand, ClearConsole, ShowHelp / 5 |

## N.DebugVisualization

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.DebugVisualization/NDebugVisualizationAssetBuilder.cs | Editor / 130 | NDebugVisualizationAssetBuilder |  |  / synced=0 / — |  | CreateOrUpdateAssets / 1 |
| Assets/N.Assets/Editor/N.DebugVisualization/NDebugVisualizationBakeUtility.cs | Editor / 691 | NDebugVisualizationBakeUtility, BuildData |  |  / synced=0 / — |  | Preview, RebuildWithConfirmation, RemoveWithConfirmation, Rebuild, EnsureMaterials / 5 |
| Assets/N.Assets/Editor/N.DebugVisualization/NDebugVisualizationEditorBase.cs | Editor / 47 | NDebugVisualizationEditorBase |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.DebugVisualization/NDebugVisualizationManagerEditor.cs | Editor / 129 | NDebugVisualizationManagerEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.DebugVisualization/NDebugVisualizationManager.cs | Runtime / 353 | NDebugVisualizationManager |  | None / synced=0 / — | Start, Update | ApplyVisibility, ApplyColors, ShowAllWorld, HideAll, ToggleMeshWireframes, ToggleUvOverlay, ToggleNormals, ToggleColliders / 19 |

## N.DoorSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.DoorSystem/NDoorPhysBoneSetupUtility.cs | Editor / 429 | NDoorPhysBoneSetupUtility, SetupContext | NDoorSystem |  / synced=0 / — |  | PreviewSelection, ApplySelection / 2 |
| Assets/N.Assets/Editor/N.DoorSystem/NDoorSystemEditor.cs | Editor / 564 | NDoorSystemEditor, NDoorCardKeyEditor, NDoorHandleInputEditor, NDoorPhysBoneHandleInputEditor, NDoorRelayEditorBase, NDoorAuthZoneEditor, NDoorTeleportInputEditor, NDoorModeSwitchEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorAuthZone.cs | Runtime / 55 | NDoorAuthZone | NDoorSystem | NoVariableSync / synced=0 / — | Start, Update | RefreshInteractionMode, Interact, OnPlayerTriggerEnter, OnConstraintReceiverEnter / 4 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorCardKey.cs | Runtime / 60 | NDoorCardKey | NDoorSystem | Continuous / synced=2 / — | Start, Update, OnDeserialization | OnPickup, OnDrop, OnDeserialization, AssignOwner, SetDisplayPose, IsLocallyHeld, ClearAssignment / 7 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorHandleInput.cs | Runtime / 37 | NDoorHandleInput | NDoorSystem | NoVariableSync / synced=0 / — | Update | Interact, OnPickup, OnDrop / 3 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorModeSwitch.cs | Runtime / 19 | NDoorModeSwitch | NDoorSystem | NoVariableSync / synced=0 / — |  | Interact / 1 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorPhysBoneHandleInput.cs | Runtime / 36 | NDoorPhysBoneHandleInput | NDoorSystem | NoVariableSync / synced=0 / — |  | OnPhysBoneGrabbed, OnPhysBoneReleased / 2 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorSystem.cs | Runtime / 1503 | NDoorSystem | NDynamicObjectManager, UdonBehaviour[], NDynamicObjectSnapPoint[], UdonBehaviour, NDynamicObjectSnapPoint, NDoorCardKey | Manual / synced=2 / — | Start, Update, FixedUpdate, OnDeserialization, OnOwnershipTransferred | OnDeserialization, OnOwnershipTransferred, IsLocked, IsRealMode, TryUseCardKey, SetLocked, InteractDoor, BeginHandleGrab / 32 |
| Assets/N.Assets/N.Script/N.DoorSystem/NDoorTeleportInput.cs | Runtime / 36 | NDoorTeleportInput | NDoorSystem | NoVariableSync / synced=0 / — | Start, Update | RefreshInteractionMode, Interact / 2 |

## N.DriftCorrection

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.DriftCorrection/Editor/NDriftCorrectionEditor.cs | Editor / 80 | NDriftCorrectionEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.DriftCorrection/Runtime/NDriftCorrection.cs | Runtime / 171 | NDriftCorrection | UdonBehaviour | None / synced=0 / — | Update | Interact, StartNeutralCalibration, ResetNeutralCalibration, GetHorizontal, GetVertical / 5 |

## N.DynamicObject

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectDependencyEditors.cs | Editor / 99 | NDynamicObjectSyncDependencyEditor, NDynamicObjectPickupDependencyEditor, NDynamicObjectRigidbodyDependencyEditor |  |  / synced=0 / — |  | OnInspectorGUI / 1 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectEditor.cs | Editor / 1144 | NDynamicObjectEditor | NDynamicObjectManager[], NDynamicObjectManager |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectEditorBase.cs | Editor / 89 | NDynamicObjectEditorBase |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectManagerEditor.cs | Editor / 215 | NDynamicObjectManagerEditor |  |  / synced=0 / PlayerData | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectMigrationUtility.cs | Editor / 445 | NDynamicObjectMigrationUtility | NDynamicObject[] |  / synced=0 / — |  | Add, PreviewSceneMigration, MigrateActiveScene, ApplyPreviewedSceneMigration, PreviewPrefabMigration, MigratePrefabsWithConfirmation, ApplyPreviewedPrefabMigration, Inspect / 10 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectPrefabBuilder.cs | Editor / 198 | NDynamicObjectPrefabBuilder |  |  / synced=0 / — |  | BuildSamplePrefabs, CompileUdonPrograms, BuildSamplePrefabsForValidation / 3 |
| Assets/N.Assets/Editor/N.DynamicObject/NDynamicObjectSnapPointEditor.cs | Editor / 198 | NDynamicObjectSnapPointEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/N.Script/N.DynamicObject/NDynamicObject.cs | Runtime / 1742 | NDynamicObject | NDynamicObjectManager, NCraftOperation, NDynamicObject[], NItemBonusMode, NStatusModifierTarget[], NStatusSystem, UdonSharpBehaviour, UdonSharpBehaviour[], NDynamicObject, NDynamicObjectSnapPoint | Manual / synced=22 / — | Start, OnEnable, OnDisable, Update, FixedUpdate, OnOwnershipTransferred, OnDeserialization | InitializeFromVendingMachine, GetDisplayName, GetDisplayCategoryName, GetDisplaySubcategoryName, MatchesItemName, HideInInventory, StoreInInventory, WithdrawFromInventory / 44 |
| Assets/N.Assets/N.Script/N.DynamicObject/NDynamicObjectManager.cs | Runtime / 532 | NDynamicObjectManager | NDynamicObject[], NDynamicObjectSnapPoint[], NDynamicObject, NDynamicObjectSnapPoint | None / synced=0 / PlayerData | Start, OnPlayerRestored | InitializeConfiguredReferences, RegisterConfiguredReferences, ApplyDefaultsToRegisteredObjects, RegisterObject, UnregisterObject, RegisterSnapPoint, UnregisterSnapPoint, TrySnap / 26 |
| Assets/N.Assets/N.Script/N.DynamicObject/NDynamicObjectPaymentTerminal.cs | Runtime / 44 | NDynamicObjectPaymentTerminal | NDynamicObjectManager, NUdonGameChips, UdonSharpBehaviour[] | None / synced=0 / — |  | TryPay / 1 |
| Assets/N.Assets/N.Script/N.DynamicObject/NDynamicObjectSnapPoint.cs | Runtime / 173 | NDynamicObjectSnapPoint | NDynamicObjectManager, UdonSharpBehaviour[] | Manual / synced=5 / — | Start, OnDisable, OnDeserialization | OnDeserialization, CanAccept, IsFreeFor, IsOccupiedBy, TryOccupy, ClearOccupancy, PosePosition, PoseRotation / 8 |

## N.DynamicYamaPlayer

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.DynamicYamaPlayer/NDynamicYamaPlayerManagerEditor.cs | Editor / 145 | NDynamicYamaPlayerManagerEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.DynamicYamaPlayer/NDynamicYamaPlayerPrefabBuilder.cs | Editor / 101 | NDynamicYamaPlayerPrefabBuilder |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.DynamicYamaPlayer/NDynamicYamaPlayerManager.cs | Runtime / 376 | NDynamicYamaPlayerManager | UdonSharpBehaviour | Manual / synced=1 / — | Start, OnDeserialization | RangeCheckLoop, OnDeserialization, RequestConfiguredPreset, ReleaseConfiguredPreset, RequestPreset, ReleasePreset, ReleaseAll, IsPresetActive / 8 |

## N.ElevatorSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.ElevatorSystem/NElevatorButtonEditor.cs | Editor / 505 | NElevatorButtonEditor | UdonSharpBehaviour |  / synced=0 / — | OnDisable |  / 0 |
| Assets/N.Assets/Editor/N.ElevatorSystem/NElevatorEditorBase.cs | Editor / 82 | NElevatorEditorBase |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.ElevatorSystem/NElevatorHotelSetup.cs | Editor / 608 | NElevatorHotelSetup | NElevatorButton |  / synced=0 / — |  | RepairSelectedHierarchy, ApplyPreparedSetup, Validate, SaveValidatedScene, RenderEntrancePreview, Inspect / 6 |
| Assets/N.Assets/Editor/N.ElevatorSystem/NElevatorPrefabBuilder.cs | Editor / 134 | NElevatorPrefabBuilder |  |  / synced=0 / — |  | BuildForValidation / 1 |
| Assets/N.Assets/Editor/N.ElevatorSystem/NElevatorSystemEditor.cs | Editor / 384 | NElevatorSystemEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.ElevatorSystem/NElevatorButton.cs | Runtime / 325 | NElevatorButton | NElevatorSystem, UdonSharpBehaviour | NoVariableSync / synced=0 / — | Start, Update | OnPlayerTriggerEnter, Interact, PressFromExternalEvent, ApplyDesktopTriggerState, HasRoomOwnerPermission / 5 |
| Assets/N.Assets/N.Script/N.ElevatorSystem/NElevatorSystem.cs | Runtime / 903 | NElevatorSystem | NDynamicObjectManager, NDynamicObject[], NElevatorButton[] | Manual / synced=8 / — | Start, Update, OnDeserialization, OnOwnershipTransferred | OnDeserialization, OnOwnershipTransferred, RequestFloor, RequestHallCall, RequestDestination, RequestOpenDoor, RequestCloseDoor, ToggleMaintenanceMode / 18 |

## N.FarmerSimulation

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.FarmerSimulation/Editor/NFarmerSimulationPlotEditor.cs | Editor / 140 | NFarmerCropTraitsEditor, NFarmerSimulationPlotEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.FarmerSimulation/Runtime/NFarmerCropTraits.cs | Runtime / 51 | NFarmerCropTraits |  | Manual / synced=7 / — |  | SetTraits, GetQualityName, GetTraitSummary / 3 |
| Assets/N.Assets/N.Script/N.FarmerSimulation/Runtime/NFarmerSimulationPlot.cs | Runtime / 252 | NFarmerSimulationPlot | NDynamicObject[] | Manual / synced=12 / — | Start, Update, OnDeserialization | Interact, PlantSeedByIndex, Water, ApplyFertilizer, Harvest, GetHarvestSummary, OnDeserialization / 7 |

## N.FlyingSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.FlyingSystem/NFlyingSystemEditor.cs | Editor / 276 | NFlyingSystemEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.FlyingSystem/NFlyingSystemPrefabBuilder.cs | Editor / 101 | NFlyingSystemPrefabBuilder |  |  / synced=0 / — |  | BuildForValidation / 1 |
| Assets/N.Assets/N.Script/N.FlyingSystem/NFlyingSystem.cs | Runtime / 400 | NFlyingSystem | NMovementSystem, NStatusSystem, UdonBehaviour | NoVariableSync / synced=0 / — | Start, Update, FixedUpdate, OnDisable | Interact, InputMoveHorizontal, InputMoveVertical, InputLookHorizontal, InputLookVertical, InputJump, EnableFlight, DisableFlight / 15 |

## N.GimmickTransformationSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/Editor/NGimmickTransformationAssetBuilder.cs | Editor / 115 | NGimmickTransformationAssetBuilder |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/Editor/NGimmickTransformationWindow.cs | Editor / 2212 | NGimmickTransformationWindow, MenuControlInfo, ActionInfo, ParticleInfo, WeaponInputInfo, AnimatorGraphNode, AnimatorGraphEdge, DesktopKeyInfo, PhysBoneActionInfo | NWeaponsManager, NWeaponType, NWorldWeaponController, UdonSharpBehaviour, NWorldAnimatorMenuButton |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/Editor/NWorldAnimatorControlEditors.cs | Editor / 260 | NWorldAnimatorParameterManagerEditor, NWorldAnimatorMenuButtonEditor, NWorldContactAnimatorBridgeEditor, NWorldWeaponControllerEditor, NWorldWeaponContactActionEditor, NWorldDamageReceiverEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/Editor/NWorldGimmickToggleEditor.cs | Editor / 40 | NWorldGimmickToggleEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldAnimatorMenuButton.cs | Runtime / 69 | NWorldAnimatorMenuButton | NWorldAnimatorParameterManager | NoVariableSync / synced=0 / — |  | Interact, PlayAction, ResetAction / 3 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldAnimatorParameterManager.cs | Runtime / 141 | NWorldAnimatorParameterManager |  | Manual / synced=3 / — | Start, OnDeserialization | ToggleBoolean, SelectInteger, SelectFloat, PlayPulse, ResetPulse, OnDeserialization / 6 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldContactAnimatorBridge.cs | Runtime / 86 | NWorldContactAnimatorBridge |  | None / synced=0 / — |  | OnContactEnter, OnContactExit, ResetContactPulse / 3 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldDamageReceiver.cs | Runtime / 42 | NWorldDamageReceiver |  | Manual / synced=2 / — | Start, OnDeserialization | ApplyDamage, OnDeserialization / 2 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldGimmickToggle.cs | Runtime / 82 | NWorldGimmickToggle |  | Manual / synced=1 / — | Start, OnDeserialization | Interact, OnDeserialization, TurnOn, TurnOff, Toggle / 5 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldWeaponContactAction.cs | Runtime / 38 | NWorldWeaponContactAction | NWorldWeaponController | None / synced=0 / — |  | OnContactEnter / 1 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldWeaponController.cs | Runtime / 350 | NWorldWeaponController | NWeaponsManager, NWeaponState, NWorldAnimatorMenuButton[] | Manual / synced=2 / — | Start, OnDeserialization, Update | OnPickup, OnDeserialization, OnPickupUseDown, InputUse, InputGrab, InputDrop, InputJump, InputMoveHorizontal / 18 |
| Assets/N.Assets/N.Script/N.GimmickTransformationSystem/NWorldWeaponPhysBoneAnimatorBridge.cs | Runtime / 53 | NWorldWeaponPhysBoneAnimatorBridge | NWorldWeaponController, NWorldAnimatorParameterManager | NoVariableSync / synced=0 / — |  | OnPhysBoneGrabbed, OnPhysBoneReleased, PlayGrabAction, ResetGrabAction / 4 |

## N.Inspector

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.Inspector/NInspectorEditorBase.cs | Editor / 147 | NInspectorEditorBase, NInspectorStyles |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.Inspector/NInspectorSceneCache.cs | Editor / 44 | NInspectorSceneCache |  |  / synced=0 / — |  | Invalidate / 1 |
| Assets/N.Assets/Editor/N.Inspector/NInspectorValidation.cs | Editor / 132 | NInspectorValidationTarget, NInspectorSessionValidationTarget, NInspectorValidationEditor, NInspectorValidation, Status, ContractResult |  |  / synced=0 / — |  | Property, Apply, WriteStatus, CompileRuntime, Validate / 5 |

## N.Inventory

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.Inventory/NInventoryEditorBase.cs | Editor / 82 | NInventoryEditorBase |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.Inventory/NInventoryInserterEditor.cs | Editor / 71 | NInventoryInserterEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.Inventory/NInventoryManagerEditor.cs | Editor / 169 | NInventoryManagerEditor |  |  / synced=0 / PlayerData |  |  / 0 |
| Assets/N.Assets/Editor/N.Inventory/NInventoryPrefabBuilder.cs | Editor / 183 | NInventoryPrefabBuilder |  |  / synced=0 / — |  | CreateSamplePrefab, CompileUdonPrograms / 2 |
| Assets/N.Assets/Editor/N.Inventory/NInventoryTestSceneSetup.cs | Editor / 407 | NInventoryTestSceneSetup, NInventoryTestSetupAssetPostprocessor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.Inventory/NInventoryWithdrawButtonEditor.cs | Editor / 50 | NInventoryWithdrawButtonEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.Inventory/NInventoryInserter.cs | Runtime / 76 | NInventoryInserter | NInventoryManager, NInventoryItemSize, NDynamicObject | None / synced=0 / — | Start | TryStoreItem, _OnDynamicObjectDrop / 2 |
| Assets/N.Assets/N.Script/N.Inventory/NInventoryManager.cs | Runtime / 902 | NInventoryManager | NDynamicObjectManager, NInventoryPersistenceMode, NDynamicObject[], UdonSharpBehaviour[], NDynamicObject | None / synced=0 / PlayerData | Start, Update, OnPlayerRestored | OnPlayerRestored, RegisterCatalog, RegisterCatalogItem, AddItem, RemoveItem, GetCraftableItemCount, GetCraftableItem, CraftItem / 35 |
| Assets/N.Assets/N.Script/N.Inventory/NInventoryStatusTestItem.cs | Runtime / 28 | NInventoryStatusTestItem | NStatusSystem | None / synced=0 / — |  | OnPickupUseDown / 1 |
| Assets/N.Assets/N.Script/N.Inventory/NInventoryWithdrawButton.cs | Runtime / 29 | NInventoryWithdrawButton | NInventoryManager | None / synced=0 / — |  | Interact, Withdraw / 2 |

## N.MainMenu

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.MainMenu/NIntegratedMenuPointer.cs | Runtime / 327 | NIntegratedMenuPointer | NMainMenuFollower[], UdonBehaviour[] | None / synced=0 / — | Start, PostLateUpdate | PostLateUpdate, InputUse / 2 |
| Assets/N.Assets/N.Script/N.MainMenu/NMainMenuFollower.cs | Runtime / 1676 | NMainMenuFollower | NMainMenuDesktopOpenMethod, NMainMenuVrOpenMethod, NMainMenuDominantHand, NMainMenuSummonStyle, UdonBehaviour[], UdonBehaviour, NMainMenuFollower | None / synced=0 / PlayerData | Start, PostLateUpdate, OnPlayerRestored | PointerInputReady, IsFollowModeLocked, SetPointerHover, PointerBeginGrab, PointerBeginResize, PointerEndManipulation, PointerCancelCapture, PointerBeginDock / 30 |

## N.MixedDrinksSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.MixedDrinksSystem/NMixedDrinksRecipeEditorWindow.cs | Editor / 272 | NMixedDrinksRecipeEditorWindow, IngredientRow | NMixedDrinksSystem |  / synced=0 / — |  | Open, RefreshDropdown / 2 |
| Assets/N.Assets/Editor/N.MixedDrinksSystem/NMixedDrinksSystemEditor.cs | Editor / 105 | NMixedDrinksSystemEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.MixedDrinksSystem/NMixedDrinksSystemPrefabBuilder.cs | Editor / 114 | NMixedDrinksSystemPrefabBuilder |  |  / synced=0 / — |  | GenerateManagedPrefab / 1 |
| Assets/N.Assets/N.Script/N.MixedDrinksSystem/Runtime/NMixedDrinksSystem.cs | Runtime / 34 | NMixedDrinksSystem |  | NoVariableSync / synced=0 / — |  | GetIngredientRoot, GetRecipeRoot, GetRecipeDropdown / 3 |

## N.MovementSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.MovementSystem/NMovementSystemEditor.cs | Editor / 82 | NMovementSystemEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.MovementSystem/NMovementSystemPrefabBuilder.cs | Editor / 57 | NMovementSystemPrefabBuilder |  |  / synced=0 / — |  | BuildForValidation / 1 |
| Assets/N.Assets/N.Script/N.MovementSystem/NMovementSystem.cs | Runtime / 423 | NMovementSystem | UdonBehaviour, NStatusSystem | NoVariableSync / synced=0 / — | Start, Update, LateUpdate | InputMoveHorizontal, InputMoveVertical, InputJump, OnAvatarEyeHeightChanged, OnAvatarChanged, BeginExternalMovementOverride, TryBeginExternalMovementOverride, EndExternalMovementOverride / 11 |

## N.PetSimulator

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/N.Script/N.PetSimulator/Editor/NPetSimulatorAgentEditor.cs | Editor / 89 | NPetSimulatorAgentEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.PetSimulator/Runtime/NPetSimulatorAgent.cs | Runtime / 136 | NPetSimulatorAgent |  | Manual / synced=4 / — | Start, Update, OnDeserialization | Interact, OnDeserialization / 2 |

## N.SecuritySystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.SecuritySystem/NSecurityObjectGuardEditor.cs | Editor / 187 | NSecurityObjectGuardEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.SecuritySystem/NSecuritySystemAssetBuilder.cs | Editor / 210 | NSecuritySystemAssetBuilder |  |  / synced=0 / — |  | BuildAllAssets, CompileUdonPrograms, BuildAllAssetsAutomation, ValidateCustomInspectors, BuildAllAssetsForValidation / 5 |
| Assets/N.Assets/Editor/N.SecuritySystem/NSecuritySystemEditor.cs | Editor / 182 | NSecuritySystemEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.SecuritySystem/NSecuritySystemEditors.cs | Editor / 155 | NSecurityEditorBase | UdonSharpBehaviour |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.SecuritySystem/NSecurityZoneEditor.cs | Editor / 131 | NSecurityZoneEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/N.Script/N.SecuritySystem/NSecurityObjectGuard.cs | Runtime / 461 | NSecurityObjectGuard | NSecuritySystem, NDynamicObject, NSecurityZone[] | None / synced=0 / — | Start | _InitializeGuard, _SecurityTick, _ValidateOwnershipRequest, _OnSecurityPickup, _OnSecurityDrop, _OnSecurityOwnershipTransferred, _OnSecurityDeserialization, _EndRecovery / 8 |
| Assets/N.Assets/N.Script/N.SecuritySystem/NSecuritySystem.cs | Runtime / 507 | NSecuritySystem | NSecurityZone[], NSecurityObjectGuard[], UdonSharpBehaviour, NSecurityZone | None / synced=0 / — | Start, Update, PostLateUpdate | PostLateUpdate, OnVRCCameraSettingsChanged, _ResolveReferences, _NotifyLocalPlayerEntered, _NotifyLocalPlayerExited, _IsLocalAuthorized, _IsPlayerAuthorized, _RefreshAuthorityAndVisibility / 12 |
| Assets/N.Assets/N.Script/N.SecuritySystem/NSecurityZone.cs | Runtime / 138 | NSecurityZone | NSecuritySystem | None / synced=0 / — | Start | OnPlayerTriggerEnter, OnPlayerTriggerExit, _ResolveReferences, _ContainsPoint, _RefreshLocalAuthorityAndVisibility, _ApplyLocalVisibility / 6 |

## N.StatusSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.StatusSystem/NStatusSystemEditor.cs | Editor / 488 | NStatusSystemEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.StatusSystem/NStatusSystemPrefabBuilder.cs | Editor / 55 | NStatusSystemPrefabBuilder |  |  / synced=0 / — |  | BuildForValidation / 1 |
| Assets/N.Assets/N.Script/N.StatusSystem/NStatusSystem.cs | Runtime / 1042 | NStatusSystem | NStatusModifierTarget[] | NoVariableSync / synced=0 / PlayerData | Start, Update, OnPlayerRestored | SetInventoryBonusTotals, ApplyPickupItemBonus, ApplyStatusEffect, GetCurrencyGainMultiplier, GetCurrencyCostMultiplier, GetSwimSpeedMultiplier, GetFlightSpeedMultiplier, GetSwimStaminaCostMultiplier / 42 |

## N.SwimSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.SwimSystem/NSwimSystemEditor.cs | Editor / 255 | NSwimSystemEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.SwimSystem/NSwimSystemPrefabBuilder.cs | Editor / 101 | NSwimSystemPrefabBuilder |  |  / synced=0 / — |  | BuildForValidation / 1 |
| Assets/N.Assets/N.Script/N.SwimSystem/NSwimSystem.cs | Runtime / 465 | NSwimSystem | NMovementSystem, NStatusSystem, UdonBehaviour | NoVariableSync / synced=0 / — | Start, Update, FixedUpdate, OnDisable | InputMoveHorizontal, InputMoveVertical, InputJump, EnableSwimSystem, DisableSwimSystem, ToggleSwimSystem, IsSwimming, IsUnderwater / 8 |

## N.TouchPanelUI

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.TouchPanelUI/NTouchPanelAssetBuilder.cs | Editor / 75 | NTouchPanelAssetBuilder |  |  / synced=0 / — |  | EnsureProgramAssets / 1 |
| Assets/N.Assets/Editor/N.TouchPanelUI/NTouchPanelButtonEditor.cs | Editor / 133 | NTouchPanelButtonEditor | NTouchPanelButton |  / synced=0 / — |  | Ensure / 1 |
| Assets/N.Assets/N.Script/N.TouchPanelUI/NTouchPanelButton.cs | Runtime / 152 | NTouchPanelButton | UdonBehaviour | None / synced=0 / — | Start, Update | Interact, OnContactEnter, TriggerAction, ConfigureEditor / 4 |

## N.UdonChipsExchangeSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.UdonChipsExchangeSystem/NUdonChipsExchangeEditors.cs | Editor / 318 | NUdonChipsExchangeEditorBase, NUdonChipsExchangeSystemEditor, NChipsExchangeButtonEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.UdonChipsExchangeSystem/NUdonChipsExchangePrefabBuilder.cs | Editor / 128 | NUdonChipsExchangePrefabBuilder |  |  / synced=0 / — |  | BuildAssets / 1 |
| Assets/N.Assets/N.Script/N.UdonChipsExchangeSystem/NChipsExchangeButton.cs | Runtime / 57 | NChipsExchangeButton | NUdonChipsExchangeSystem, NExchangeDirection | None / synced=0 / — |  | Interact, ExecuteExchange, SetModeSwitch, SetExchangeAmount / 4 |
| Assets/N.Assets/N.Script/N.UdonChipsExchangeSystem/NUdonChipsExchangeSystem.cs | Runtime / 371 | NUdonChipsExchangeSystem | UdonSharpBehaviour, NUdonGameChips, NStatusSystem, NExchangeRoundingMode, UdonSharpBehaviour[] | None / synced=0 / — | Start | ExchangeDefaultMoneyToGameChips, ExchangeRequestedMoneyToGameChips, ExchangeAllMoneyToGameChips, ExchangeDefaultGameChipsToMoney, ExchangeRequestedGameChipsToMoney, ExchangeAllGameChipsToMoney, TryExchangeMoneyToGameChips, TryExchangeGameChipsToMoney / 15 |

## N.UdonGameChips

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.UdonGameChips/NUdonGameChipsEditor.cs | Editor / 156 | NUdonGameChipsEditor |  |  / synced=0 / PlayerData | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.UdonGameChips/NUdonGameChipsPrefabBuilder.cs | Editor / 105 | NUdonGameChipsPrefabBuilder |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.UdonGameChips/NUdonGameChips.cs | Runtime / 223 | NUdonGameChips | UdonSharpBehaviour[], NStatusSystem | None / synced=0 / PlayerData | Start, OnPlayerRestored, Update | OnPlayerRestored, GetBankBalance, GetGameChips, CanWithdrawBank, CanSpendGameChips, CanAddGameChips, DepositBank, TryWithdrawBank / 16 |

## N.VehicleManager

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.VehicleManager/NVehicleManagerEditor.cs | Editor / 295 | NVehicleInspectorBase, NVehicleManagerEditor, NVehicleSystemEditor, NCarSystemEditor, NBoatSystemEditor, NVehiclePhysicsEditorBase, NTrainSystemEditor, NMotorcycleSystemEditor, NAircraftSystemEditor, NFighterSystemEditor, NHelicopterSystemEditor, NDroneSystemEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NAircraftSystem.cs | Runtime / 41 | NAircraftSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NBoatSystem.cs | Runtime / 55 | NBoatSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NCarSystem.cs | Runtime / 62 | NCarSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NDroneSystem.cs | Runtime / 41 | NDroneSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NFighterSystem.cs | Runtime / 43 | NFighterSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NHelicopterSystem.cs | Runtime / 38 | NHelicopterSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NMotorcycleSystem.cs | Runtime / 41 | NMotorcycleSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NTrainSystem.cs | Runtime / 42 | NTrainSystem | NVehicleSystem | NoVariableSync / synced=0 / — | Start, FixedUpdate |  / 0 |
| Assets/N.Assets/N.Script/N.VehicleManager/NVehicleManager.cs | Runtime / 91 | NVehicleManager | NMovementSystem, NSwimSystem, NFlyingSystem, NVehicleSystem | NoVariableSync / synced=0 / — | OnDisable | TryBeginVehicleControl, EndVehicleControl, IsVehicleControlActive / 3 |
| Assets/N.Assets/N.Script/N.VehicleManager/NVehicleSystem.cs | Runtime / 163 | NVehicleSystem | NVehicleManager |  / synced=0 / — | Start, Update, FixedUpdate, OnDisable | Interact, OnStationEntered, OnStationExited, ExitVehicle, ForceLeaveVehicle, GetSteeringInput, GetThrottleInput, GetBrakeInput / 9 |

## N.VirtualInput

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.VirtualInput/NVirtualInputAssetBuilder.cs | Editor / 175 | NVirtualInputAssetBuilder |  |  / synced=0 / — |  | CreateOrUpdateAssets / 1 |
| Assets/N.Assets/Editor/N.VirtualInput/NVirtualInputContactGateEditor.cs | Editor / 61 | NVirtualInputContactGateEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.VirtualInput/NVirtualInputEditorBase.cs | Editor / 49 | NVirtualInputEditorBase |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.VirtualInput/NVirtualInputManagerEditor.cs | Editor / 238 | NVirtualInputManagerEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.VirtualInput/NVirtualInputPhysBoneGateEditor.cs | Editor / 41 | NVirtualInputPhysBoneGateEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.VirtualInput/NVirtualInputContactGate.cs | Runtime / 33 | NVirtualInputContactGate | NVirtualInputManager | None / synced=0 / — |  | OnContactEnter, OnContactExit / 2 |
| Assets/N.Assets/N.Script/N.VirtualInput/NVirtualInputManager.cs | Runtime / 441 | NVirtualInputManager | UdonBehaviour | None / synced=0 / — | Start, Update | Interact, InputUse, InputGrab, OnInputMethodChanged, SetRightContactGateActive, SetRightContactGateInactive, SetLeftContactGateActive, SetLeftContactGateInactive / 16 |
| Assets/N.Assets/N.Script/N.VirtualInput/NVirtualInputPhysBoneGate.cs | Runtime / 33 | NVirtualInputPhysBoneGate | NVirtualInputManager | None / synced=0 / — |  | OnPhysBoneGrabbed, OnPhysBoneReleased / 2 |

## N.WaterRippleSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.WaterRippleSystem/NWaterBuoyantPickupEditor.cs | Editor / 69 | NWaterBuoyantPickupEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.WaterRippleSystem/NWaterRippleControllerEditor.cs | Editor / 1704 | NWaterRippleControllerEditor, NWaterRippleSampleSetupRequest |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/N.Script/N.WaterRippleSystem/NWaterBuoyantPickup.cs | Runtime / 95 | NWaterBuoyantPickup |  | None / synced=0 / — | Start, FixedUpdate, OnDisable |  / 0 |
| Assets/N.Assets/N.Script/N.WaterRippleSystem/NWaterRippleController.cs | Runtime / 827 | NWaterRippleController |  | None / synced=0 / — | Start, LateUpdate, OnDisable | ResetSimulation, EmitPreviewSplash / 2 |

## N.WeaponsManager

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.WeaponsManager/NWeaponsManagerEditor.cs | Editor / 43 | NWeaponsManagerEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.WeaponsManager/NWeaponStateEditor.cs | Editor / 49 | NWeaponStateEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/N.Script/N.WeaponsManager/NWeaponsManager.cs | Runtime / 47 | NWeaponsManager | NWeaponState[], UdonSharpBehaviour | Manual / synced=0 / — |  | RegisterWeapon, CanProcessWeapon, GetDamage, NotifyWeaponStateChanged / 4 |
| Assets/N.Assets/N.Script/N.WeaponsManager/NWeaponState.cs | Runtime / 132 | NWeaponState | NWeaponsManager, UdonSharpBehaviour, NWeaponType, NDynamicObject | Manual / synced=3 / — | Start, OnDeserialization | TryUse, Reload, OnDeserialization, OnPickup, OnDrop, OnPickupUseDown, SetSafety, SetColliderState / 11 |

## N.WelcomeSystem

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.WelcomeSystem/NWelcomeWindowSceneSetup.cs | Editor / 137 | NWelcomeWindowSceneSetup |  |  / synced=0 / — |  | RepairAuthorityKeyPickup, Apply, RepairDoorLocker701Outer / 3 |
| Assets/N.Assets/N.Script/N.WelcomeSystem/NWelcomeBoardIdentityBridge.cs | Runtime / 65 | NWelcomeBoardIdentityBridge | UdonSharpBehaviour | NoVariableSync / synced=0 / — |  | OnPlayerTriggerEnter, OnPlayerTriggerExit, IsLocalInside, PrepareIdentityCard / 4 |

## N.WIMExtensions

| ファイル | 区分 / 行数 | クラス | 参照型 | 同期 / 保存 | callbacks | API抜粋 / 件数 |
|---|---|---|---|---|---|---|
| Assets/N.Assets/Editor/N.WIMExtensions/NIntegratedMenuExperienceBuilder.cs | Editor / 449 | NIntegratedMenuExperienceBuilder |  |  / synced=0 / — |  | Apply, RepairEquipmentSelectionAndFollow, Refine / 3 |
| Assets/N.Assets/Editor/N.WIMExtensions/NIntegratedMenuOptimizer.cs | Editor / 687 | NIntegratedMenuOptimizer, Piece, Hit, NIntegratedMenuPointerEditor |  |  / synced=0 / — |  | Prepare, InspectApi, ApplyWithConfirmation, ApplyAuthorized, RefineFrames, ReferenceArt, Validate, Preview / 8 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMCatalogPageInspector.cs | Editor / 240 | NWIMCatalogPageInspector |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMExtensionsEditor.cs | Editor / 151 | NWIMInspectorUI, NWIMChatModuleEditor, NWIMWeatherModuleEditor |  |  / synced=0 / — | OnEnable | Header, Label / 2 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMExtensionsPrefabBuilder.cs | Editor / 620 | NWIMExtensionsPrefabBuilder | UdonBehaviour |  / synced=0 / — |  | BuildAll, BuildWeatherOnly, InstallIntoOpenScene, InstallModulesOnly, RemoveUnintendedBuilderRoots, ClearConsole, UpgradeWeatherIntegration / 7 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMInventoryAutoSetup.cs | Editor / 530 | NWIMInventoryAutoSetup | NDynamicObject[], UdonSharpBehaviour[] |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMMenuEditors.cs | Editor / 190 | NWIMMenuEditorBase, NWIMInventoryModuleEditor, NWIMMenuShellEditor |  |  / synced=0 / — | OnEnable |  / 0 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMMenuPageEditors.cs | Editor / 59 | NWIMShopPageEditor, NWIMMapPageEditor, NWIMSettingsPageEditor, NWIMEquipmentPageEditor, NWIMCraftPageEditor |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMMenuPrefabBuilder.cs | Editor / 1883 | NWIMMenuPrefabBuilder | NWIMMenuShell, NWIMShopPage, NWIMMapPage, NWIMSettingsPage, NWIMEquipmentPage |  / synced=0 / — |  | Build, RepairMainMenuInteractionControls, EnableTestShopProducts, InstallEquipmentCraftAndSlotExpansionTests, InstallIndependentMainMenu, InstallIntoWim, ConnectExistingIntoWim, AddSpecialPagesToExistingPrefab / 10 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMMenuReferenceBinder.cs | Editor / 791 | NWIMMenuReferenceBinder | UdonBehaviour |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMMenuValidation.cs | Editor / 145 | NWIMMenuValidation |  |  / synced=0 / PlayerData |  | Run, Validate / 2 |
| Assets/N.Assets/Editor/N.WIMExtensions/NWIMTMPSubMeshHierarchyCleaner.cs | Editor / 61 | NWIMTMPSubMeshHierarchyCleaner |  |  / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMChatModule.cs | Runtime / 32 | NWIMChatModule | UdonBehaviour | None / synced=0 / — |  | SendMessageToChat, OnModuleCalled / 2 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMCraftPage.cs | Runtime / 43 | NWIMCraftPage | NWIMMenuShell, NDynamicObject[] | None / synced=0 / — |  | SelectAll, SelectAssembly, SelectSynthesis, SelectAlchemy, SelectDisassembly, SelectRepair, SelectForge, SelectCooking / 9 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMEquipmentPage.cs | Runtime / 45 | NWIMEquipmentPage | NStatusSystem, NInventoryManager | None / synced=0 / — | Update |  / 0 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMInventoryModule.cs | Runtime / 794 | NWIMInventoryModule | NInventoryManager, NUdonGameChips, NUdonChipsExchangeSystem, NStatusSystem, NWIMMenuShell, NInventorySortMode, UdonBehaviour[], NDynamicObject | None / synced=0 / PlayerData | OnEnable, Start, OnPlayerRestored | OnNInventoryChanged, RefreshView, PreviousPage, NextPage, ShowOwnedItems, ShowAllItems, ShowCategory00, ShowCategory01 / 49 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMMapPage.cs | Runtime / 24 | NWIMMapPage | TeleportModule, TeleportTarget[] | None / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMMenuShell.cs | Runtime / 2313 | NWIMMenuShell | NWIMMenuShell[], UdonBehaviour[], NWIMInventoryModule, NUdonChipsExchangeSystem, NSwimSystem, NFlyingSystem, UdonBehaviour, NWIMShopPage, NWIMMapPage, NWIMSettingsPage, NWIMEquipmentPage, NWIMCraftPage, NWIMMenuShell, NDynamicObject | None / synced=0 / PlayerData | Start, OnEnable, OnDisable, Update, OnPlayerRestored | FitDesign, OnModuleCalled, SelectCurrentEntry, ShowMain, ShowChat, ShowInventory, ShowEquipment, ShowSettings / 116 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMSettingsPage.cs | Runtime / 35 | NWIMSettingsPage |  | None / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMShopPage.cs | Runtime / 41 | NWIMShopPage | NDynamicObject[] | None / synced=0 / — |  |  / 0 |
| Assets/N.Assets/N.Script/N.WIMExtensions/NWIMWeatherModule.cs | Runtime / 132 | NWIMWeatherModule | WeatherSystem | None / synced=0 / — | Start | OnModuleCalled, WeatherUpdated, RebuildUI, GetWeatherIcon / 4 |

## 同名クラス候補

同名はnamespace・条件コンパイル・asmdefを確認する前に重複不具合と断定しない。
