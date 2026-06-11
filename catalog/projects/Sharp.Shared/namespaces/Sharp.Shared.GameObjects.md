# Sharp.Shared.GameObjects

Project: Sharp.Shared
Types: 42 (0 generated)

### interface IAdditionalMatchStats : Sharp.Shared.GameObjects.IAdditionalPerRoundStats

- FullName: `Sharp.Shared.GameObjects.IAdditionalMatchStats`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IControllerActionTrackingService.cs:128
- Generated: false
- Attributes: `[NetClass("CSAdditionalMatchStats_t")]`

#### Properties
- `float Sharp.Shared.GameObjects.IAdditionalMatchStats.TeamDamage` [L:152]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.MaxNumRoundsSurvivedStreak` [L:132]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumClutchKills` [L:142]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumFirstKills` [L:140]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumPistolKills` [L:144]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumRoundsSurvivedStreak` [L:130]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumRoundsSurvivedTotal` [L:134]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumSniperKills` [L:146]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumSuicides` [L:148]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.NumTeamKills` [L:150]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.RoundsWonWithoutPurchase` [L:136]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalMatchStats.RoundsWonWithoutPurchaseTotal` [L:138]
  - Modifiers: public, abstract


### interface IAdditionalPerRoundStats : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IAdditionalPerRoundStats`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IControllerActionTrackingService.cs:102
- Generated: false
- Attributes: `[NetClass("CSAdditionalPerRoundStats_t")]`

#### Properties
- `bool Sharp.Shared.GameObjects.IAdditionalPerRoundStats.BombPlantedAndAlive` [L:118]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameObjects.IAdditionalPerRoundStats.FreshStartThisRound` [L:116]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameObjects.IAdditionalPerRoundStats.BlastDamageInflicted` [L:112]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameObjects.IAdditionalPerRoundStats.BurnDamageInflicted` [L:110]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.BombCarrierkills` [L:108]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.DefuseStarts` [L:120]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.Dinks` [L:114]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.HostagePickUps` [L:122]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.KillsWhileBlind` [L:106]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.NumChickensKilled` [L:104]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAdditionalPerRoundStats.NumTeammatesFlashed` [L:124]
  - Modifiers: public, abstract


### interface IAimPunchService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IAimPunchService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IAimPunchService.cs:26
- Generated: false
- Attributes: `[NetClass("CCSPlayer_AimPunchServices")]`

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IAimPunchService.PredictableBaseAngle` [L:31]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IAimPunchService.PredictableBaseAngleVel` [L:32]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IAimPunchService.UnpredictableBaseAngle` [L:36]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameObjects.IAimPunchService.PredictableBaseTickInterpAmount` [L:29]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAimPunchService.PredictableBaseTick` [L:28]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IAimPunchService.UnpredictableBaseTick` [L:34]
  - Modifiers: public, abstract


### interface IAttributeContainer : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IAttributeContainer`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IEconItem.cs:26
- Generated: false
- Attributes: `[NetClass("CAttributeContainer")]`

#### Properties
- `Sharp.Shared.GameObjects.IEconItemView Sharp.Shared.GameObjects.IAttributeContainer.Item` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: Econ item view


### interface IBodyComponent : Sharp.Shared.CStrike.IEntityComponent

- FullName: `Sharp.Shared.GameObjects.IBodyComponent`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBodyComponent.cs:28
- Generated: false
- Attributes: `[NetClass("CBodyComponent")]`

#### Properties
- `Sharp.Shared.GameObjects.IBodyComponentSkeletonInstance Sharp.Shared.GameObjects.IBodyComponent.AsBodyComponentSkeletonInstance` [L:35]
  - Modifiers: public, abstract, readonly
  - Summary: Cast to  without validating

#### Methods
- `Sharp.Shared.GameObjects.IGameSceneNode? Sharp.Shared.GameObjects.IBodyComponent.GetSceneNode()` [L:30]
  - Modifiers: public, abstract


### interface IBodyComponentSkeletonInstance : Sharp.Shared.GameObjects.IBodyComponent

- FullName: `Sharp.Shared.GameObjects.IBodyComponentSkeletonInstance`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBodyComponent.cs:39
- Generated: false
- Attributes: `[NetClass("CBodyComponentSkeletonInstance")]`

#### Methods
- `Sharp.Shared.GameObjects.ISkeletonInstance? Sharp.Shared.GameObjects.IBodyComponentSkeletonInstance.GetSkeletonInstance()` [L:41]
  - Modifiers: public, abstract


### interface IBulletService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IBulletService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBulletService.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayer_BulletServices")]`
- Summary: BulletServices is CCSPlayerPawn only

#### Properties
- `int Sharp.Shared.GameObjects.IBulletService.TotalHitsOnServer` [L:33]
  - Modifiers: public, abstract
  - Summary: m_totalHitsOnServer


### interface IBuyService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IBuyService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBuyService.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayer_BuyServices")]`
- Summary: BuyService is CCSPlayerPawn only


### interface ICameraService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.ICameraService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/ICameraService.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayerBase_CameraServices")]`

#### Properties
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameObjects.ICameraService.ViewEntity` [L:38]
  - Modifiers: public, abstract
  - Summary: CPlayer_CameraServices::m_hViewEntity
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.ICameraService.ViewEntityHandle` [L:33]
  - Modifiers: public, abstract
  - Summary: CPlayer_CameraServices::m_hViewEntity
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.ICameraService.ZoomOwnerHandle` [L:63]
  - Modifiers: public, abstract
  - Summary: CCSPlayerBase_CameraServices::m_hZoomOwner
- `float Sharp.Shared.GameObjects.ICameraService.FieldOfViewRate` [L:58]
  - Modifiers: public, abstract
  - Summary: CCSPlayerBase_CameraServices::m_flFOVRate
- `float Sharp.Shared.GameObjects.ICameraService.FieldOfViewTime` [L:53]
  - Modifiers: public, abstract
  - Summary: CCSPlayerBase_CameraServices::m_flFOVTime
- `uint Sharp.Shared.GameObjects.ICameraService.FieldOfView` [L:43]
  - Modifiers: public, abstract
  - Summary: CCSPlayerBase_CameraServices::m_iFOV
- `uint Sharp.Shared.GameObjects.ICameraService.FieldOfViewStart` [L:48]
  - Modifiers: public, abstract
  - Summary: CCSPlayerBase_CameraServices::m_iFOVStart

#### Methods
- `Sharp.Shared.CStrike.ISchemaList<Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity>> Sharp.Shared.GameObjects.ICameraService.GetPostProcessingVolumes()` [L:68]
  - Modifiers: public, abstract
  - Summary: CPlayer_CameraServices::m_PostProcessingVolumes


### interface ICollisionProperty : Sharp.Shared.CStrike.IEntityObject

- FullName: `Sharp.Shared.GameObjects.ICollisionProperty`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/ICollisionProperty.cs:28
- Generated: false
- Attributes: `[NetClass("CCollisionProperty")]`

#### Properties
- `Sharp.Shared.Enums.CollisionGroupType Sharp.Shared.GameObjects.ICollisionProperty.CollisionGroup` [L:48]
  - Modifiers: public, abstract
  - Summary: Collision group
- `Sharp.Shared.Enums.SolidType Sharp.Shared.GameObjects.ICollisionProperty.SolidType` [L:33]
  - Modifiers: public, abstract
  - Summary: Solid type, typically related to collision
- `Sharp.Shared.Enums.SurroundingBoundsType Sharp.Shared.GameObjects.ICollisionProperty.SurroundType` [L:73]
  - Modifiers: public, abstract
  - Summary: m_nSurroundType
- `Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute Sharp.Shared.GameObjects.ICollisionProperty.CollisionAttribute` [L:53]
  - Modifiers: public, abstract, readonly
  - Summary: VPhysics collision attribute
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.ICollisionProperty.Maxs` [L:63]
  - Modifiers: public, abstract
  - Summary: Bounding Box Maxs
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.ICollisionProperty.Mins` [L:58]
  - Modifiers: public, abstract
  - Summary: Bounding Box Mins
- `byte Sharp.Shared.GameObjects.ICollisionProperty.EnablePhysics` [L:38]
  - Modifiers: public, abstract
  - Summary: VPhysics type to enable
- `byte Sharp.Shared.GameObjects.ICollisionProperty.SolidFlags` [L:43]
  - Modifiers: public, abstract
  - Summary: Solid Flags
- `float Sharp.Shared.GameObjects.ICollisionProperty.BoundingRadius` [L:68]
  - Modifiers: public, abstract
  - Summary: Bounding capsule/sphere radius


### interface IControllerActionTrackingService : Sharp.Shared.GameObjects.IPlayerControllerComponent

- FullName: `Sharp.Shared.GameObjects.IControllerActionTrackingService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IControllerActionTrackingService.cs:156
- Generated: false
- Attributes: `[NetClass("CCSPlayerController_ActionTrackingServices")]`

#### Properties
- `float Sharp.Shared.GameObjects.IControllerActionTrackingService.TotalRoundDamageDealt` [L:171]
  - Modifiers: public, abstract
  - Summary: Total damage dealt in current round
- `int Sharp.Shared.GameObjects.IControllerActionTrackingService.NumRoundKills` [L:161]
  - Modifiers: public, abstract
  - Summary: Number of kills in current round
- `int Sharp.Shared.GameObjects.IControllerActionTrackingService.NumRoundKillsHeadshots` [L:166]
  - Modifiers: public, abstract
  - Summary: Number of headshot kills in current round

#### Methods
- `Sharp.Shared.GameObjects.IAdditionalMatchStats Sharp.Shared.GameObjects.IControllerActionTrackingService.GetAdditionalMatchStats()` [L:181]
  - Modifiers: public, abstract
  - Summary: Get additional match stats
- `Sharp.Shared.GameObjects.IMatchStats Sharp.Shared.GameObjects.IControllerActionTrackingService.GetMatchStats()` [L:176]
  - Modifiers: public, abstract
  - Summary: Gets the MatchStats instance


### interface IDamageReactService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IDamageReactService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IDamageReactService.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayer_DamageReactServices")]`
- Summary: DamageReactServices is CCSPlayerPawn only


### interface IDamageRecord : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.GameObjects.IDamageRecord`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IDamageService.cs:38
- Generated: false
- Attributes: `[NetClass("CDamageRecord")]`

#### Properties
- `Sharp.Shared.GameObjects.KillTypes Sharp.Shared.GameObjects.IDamageRecord.KillType` [L:73]
  - Modifiers: public, abstract, readonly
  - Summary: Kill type
- `Sharp.Shared.Units.SteamID Sharp.Shared.GameObjects.IDamageRecord.DamagerXuid` [L:43]
  - Modifiers: public, abstract, readonly
  - Summary: Killer SteamId
- `Sharp.Shared.Units.SteamID Sharp.Shared.GameObjects.IDamageRecord.RecipientXuid` [L:48]
  - Modifiers: public, abstract, readonly
  - Summary: Victim SteamId
- `float Sharp.Shared.GameObjects.IDamageRecord.ActualHealthRemoved` [L:63]
  - Modifiers: public, abstract, readonly
  - Summary: Actual health removed
- `float Sharp.Shared.GameObjects.IDamageRecord.BulletsDamage` [L:53]
  - Modifiers: public, abstract, readonly
  - Summary: Bullet damage
- `float Sharp.Shared.GameObjects.IDamageRecord.Damage` [L:58]
  - Modifiers: public, abstract, readonly
  - Summary: Total damage
- `int Sharp.Shared.GameObjects.IDamageRecord.NumHits` [L:68]
  - Modifiers: public, abstract, readonly
  - Summary: Number of hits


### interface IDamageService : Sharp.Shared.GameObjects.IPlayerControllerComponent

- FullName: `Sharp.Shared.GameObjects.IDamageService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IDamageService.cs:77
- Generated: false
- Attributes: `[NetClass("CCSPlayerController_DamageServices")]`

#### Methods
- `Sharp.Shared.CStrike.ISchemaEmbeddedList<Sharp.Shared.GameObjects.IDamageRecord> Sharp.Shared.GameObjects.IDamageService.GetDamageList()` [L:82]
  - Modifiers: public, abstract
  - Summary: Gets the damage statistics list


### interface IEconItemDefinition : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.GameObjects.IEconItemDefinition`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IEconItemDefinition.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Enums.EconItemType Sharp.Shared.GameObjects.IEconItemDefinition.ItemType` [L:37]
  - Modifiers: public, abstract, readonly
- `byte Sharp.Shared.GameObjects.IEconItemDefinition.Quality` [L:29]
  - Modifiers: public, abstract, readonly
- `byte Sharp.Shared.GameObjects.IEconItemDefinition.Rarity` [L:28]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.GameObjects.IEconItemDefinition.DefaultLoadoutSlot` [L:38]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.BaseDisplayModel` [L:32]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.DefinitionName` [L:35]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.ItemBaseName` [L:30]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.ItemClassName` [L:34]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.ItemTypeName` [L:31]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IEconItemDefinition.WorldDisplayModel` [L:33]
  - Modifiers: public, abstract, readonly
- `uint Sharp.Shared.GameObjects.IEconItemDefinition.StickerSlots` [L:36]
  - Modifiers: public, abstract, readonly
- `ushort Sharp.Shared.GameObjects.IEconItemDefinition.Index` [L:27]
  - Modifiers: public, abstract, readonly


### interface IEconItemView : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IEconItemView`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IEconItem.cs:35
- Generated: false
- Attributes: `[NetClass("CEconItemView")]`

#### Properties
- `bool Sharp.Shared.GameObjects.IEconItemView.Initialized` [L:74]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.GameObjects.IEconItemView.Quality` [L:45]
  - Modifiers: public, abstract, readonly
  - Summary: Item quality
- `string Sharp.Shared.GameObjects.IEconItemView.CustomName` [L:72]
  - Modifiers: public, abstract
- `uint Sharp.Shared.GameObjects.IEconItemView.AccountId` [L:70]
  - Modifiers: public, abstract, readonly
  - Summary: Owner AccountId
- `uint Sharp.Shared.GameObjects.IEconItemView.ItemIdHigh` [L:60]
  - Modifiers: public, abstract, readonly
  - Summary: Item ID (high bits)
- `uint Sharp.Shared.GameObjects.IEconItemView.ItemIdLow` [L:65]
  - Modifiers: public, abstract, readonly
  - Summary: Item ID (low bits)
- `uint Sharp.Shared.GameObjects.IEconItemView.Level` [L:50]
  - Modifiers: public, abstract, readonly
  - Summary: Item level
- `ulong Sharp.Shared.GameObjects.IEconItemView.ItemId` [L:55]
  - Modifiers: public, abstract, readonly
  - Summary: Item ID (corresponds to ID in Steam inventory)
- `ushort Sharp.Shared.GameObjects.IEconItemView.ItemDefinitionIndex` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: ItemDefIndex

#### Methods
- `void Sharp.Shared.GameObjects.IEconItemView.SetAccountIdLocal(uint value)` [L:82]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetCustomNameLocal(string value)` [L:86]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetCustomNameOverrideLocal(string value)` [L:88]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetInitializedLocal(bool value)` [L:90]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetItemDefinitionIndexLocal(ushort value)` [L:76]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetItemIdHighLocal(uint value)` [L:80]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetItemIdLowLocal(uint value)` [L:78]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IEconItemView.SetQualityLocal(int value)` [L:84]
  - Modifiers: public, abstract


### interface IGameSceneNode : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IGameSceneNode`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBodyComponent.cs:45
- Generated: false
- Attributes: `[NetClass("CGameSceneNode")]`

#### Properties
- `Sharp.Shared.GameObjects.ISkeletonInstance? Sharp.Shared.GameObjects.IGameSceneNode.AsSkeletonInstance` [L:63]
  - Modifiers: public, abstract, readonly
  - Summary: Cast to
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IGameSceneNode.AbsOrigin` [L:55]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IGameSceneNode.AbsRotation` [L:56]
  - Modifiers: public, abstract, readonly
- `float Sharp.Shared.GameObjects.IGameSceneNode.AbsScale` [L:58]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameObjects.IGameSceneNode.Scale` [L:57]
  - Modifiers: public, abstract

#### Methods
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameObjects.IGameSceneNode.GetOwner()` [L:53]
  - Modifiers: public, abstract
- `Sharp.Shared.GameObjects.IGameSceneNode? Sharp.Shared.GameObjects.IGameSceneNode.GetChild()` [L:49]
  - Modifiers: public, abstract
- `Sharp.Shared.GameObjects.IGameSceneNode? Sharp.Shared.GameObjects.IGameSceneNode.GetNextSibling()` [L:51]
  - Modifiers: public, abstract
- `Sharp.Shared.GameObjects.IGameSceneNode? Sharp.Shared.GameObjects.IGameSceneNode.GetParent()` [L:47]
  - Modifiers: public, abstract


### interface IGlowProperty : Sharp.Shared.CStrike.IEntityObject

- FullName: `Sharp.Shared.GameObjects.IGlowProperty`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IGlowProperty.cs:27
- Generated: false
- Attributes: `[NetClass("CGlowProperty")]`

#### Properties
- `Sharp.Shared.Types.Color32 Sharp.Shared.GameObjects.IGlowProperty.GlowColorOverride` [L:82]
  - Modifiers: public, abstract
  - Summary: m_glowColorOverride
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IGlowProperty.GlowColor` [L:77]
  - Modifiers: public, abstract
  - Summary: m_fGlowColor
- `bool Sharp.Shared.GameObjects.IGlowProperty.EligibleForScreenHighlight` [L:42]
  - Modifiers: public, abstract
  - Summary: m_bEligibleForScreenHighlight
- `bool Sharp.Shared.GameObjects.IGlowProperty.Flashing` [L:62]
  - Modifiers: public, abstract
  - Summary: m_bFlashing
- `bool Sharp.Shared.GameObjects.IGlowProperty.Glowing` [L:57]
  - Modifiers: public, abstract
  - Summary: Glowing
- `float Sharp.Shared.GameObjects.IGlowProperty.GlowStartTime` [L:52]
  - Modifiers: public, abstract
  - Summary: m_flGlowStartTime
- `float Sharp.Shared.GameObjects.IGlowProperty.GlowTime` [L:47]
  - Modifiers: public, abstract
  - Summary: m_flGlowTime
- `int Sharp.Shared.GameObjects.IGlowProperty.GlowRangeMax` [L:67]
  - Modifiers: public, abstract
  - Summary: m_nGlowRange
- `int Sharp.Shared.GameObjects.IGlowProperty.GlowRangeMin` [L:72]
  - Modifiers: public, abstract
  - Summary: m_nGlowRangeMin
- `int Sharp.Shared.GameObjects.IGlowProperty.GlowTeam` [L:37]
  - Modifiers: public, abstract
  - Summary: m_iGlowTeam
- `int Sharp.Shared.GameObjects.IGlowProperty.GlowType` [L:32]
  - Modifiers: public, abstract
  - Summary: m_iGlowType


### interface IHostageService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IHostageService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IHostageService.cs:30
- Generated: false
- Attributes: `[NetClass("CCSPlayer_HostageServices")]`
- Summary: HostageServices is CCSPlayerPawn only

#### Properties
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.IHostageService.CarriedHostageHandle` [L:35]
  - Modifiers: public, abstract
  - Summary: m_hCarriedHostage
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.IHostageService.CarriedHostagePropHandle` [L:40]
  - Modifiers: public, abstract
  - Summary: m_hCarriedHostageProp


### interface IInGameMoneyService : Sharp.Shared.GameObjects.IPlayerControllerComponent

- FullName: `Sharp.Shared.GameObjects.IInGameMoneyService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IInGameMoneyService.cs:25
- Generated: false
- Attributes: `[NetClass("CCSPlayerController_InGameMoneyServices")]`

#### Properties
- `int Sharp.Shared.GameObjects.IInGameMoneyService.Account` [L:30]
  - Modifiers: public, abstract
  - Summary: The amount of money


### interface IInventoryService : Sharp.Shared.GameObjects.IPlayerControllerComponent

- FullName: `Sharp.Shared.GameObjects.IInventoryService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IInventoryService.cs:25
- Generated: false
- Attributes: `[NetClass("CCSPlayerController_InventoryServices")]`

#### Properties
- `int Sharp.Shared.GameObjects.IInventoryService.PersonaDataPublicLevel` [L:40]
  - Modifiers: public, abstract
  - Summary: m_nPersonaDataPublicLevel
- `int Sharp.Shared.GameObjects.IInventoryService.PersonaDataXpTrailLevel` [L:35]
  - Modifiers: public, abstract
  - Summary: m_nPersonaDataXpTrailLevel
- `ushort Sharp.Shared.GameObjects.IInventoryService.MusicId` [L:30]
  - Modifiers: public, abstract
  - Summary: m_unMusicID


### interface IItemService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IItemService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IItemService.cs:30
- Generated: false
- Attributes: `[NetClass("CCSPlayer_ItemServices")]`
- Summary: ItemServices is only for CCSPlayerPawn

#### Properties
- `bool Sharp.Shared.GameObjects.IItemService.HasDefuser` [L:35]
  - Modifiers: public, abstract
  - Summary: Does the player have a defuser
- `bool Sharp.Shared.GameObjects.IItemService.HasHelmet` [L:40]
  - Modifiers: public, abstract
  - Summary: Does the player have a helmet

#### Methods
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameObjects.IItemService.GiveNamedItem(Sharp.Shared.Enums.EconItemId id)` [L:44]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameObjects.IItemService.GiveNamedItem(string classname)` [L:42]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameObjects.IItemService.RemoveAllItems(bool removeSuit)` [L:46]
  - Modifiers: public, abstract


### interface IMatchStats : Sharp.Shared.GameObjects.IPerRoundStats

- FullName: `Sharp.Shared.GameObjects.IMatchStats`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IControllerActionTrackingService.cs:56
- Generated: false
- Attributes: `[NetClass("CSMatchStats_t")]`

#### Properties
- `float Sharp.Shared.GameObjects.IMatchStats.HealthPointsDealtTotal` [L:82]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameObjects.IMatchStats.HealthPointsRemovedTotal` [L:80]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.Enemy2Ks` [L:64]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.Enemy3Ks` [L:62]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.Enemy4Ks` [L:60]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.Enemy5Ks` [L:58]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.EnemyKnifeKills` [L:66]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.EnemyTaserKills` [L:68]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.EntryCount` [L:96]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.EntryWins` [L:98]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.FlashCount` [L:76]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.FlashSuccesses` [L:78]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.R1V1Count` [L:88]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.R1V1Wins` [L:90]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.R1V2Count` [L:92]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.R1V2Wins` [L:94]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.ShotsFiredTotal` [L:84]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.ShotsOnTargetTotal` [L:86]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.UtilityCount` [L:70]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.UtilityEnemies` [L:74]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IMatchStats.UtilitySuccesses` [L:72]
  - Modifiers: public, abstract


### interface IModelState : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.GameObjects.IModelState`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBodyComponent.cs:77
- Generated: false
- Attributes: `[NetClass("CModelState")]`

#### Properties
- `string Sharp.Shared.GameObjects.IModelState.ModelName` [L:79]
  - Modifiers: public, abstract, readonly
- `ulong Sharp.Shared.GameObjects.IModelState.MeshGroupMask` [L:81]
  - Modifiers: public, abstract, readonly


### interface IMovementService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IMovementService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IMovementService.cs:26
- Generated: false
- Attributes: `[NetClass("CPlayer_MovementServices")]`

#### Properties
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.GameObjects.IMovementService.KeyButtons` [L:36]
  - Modifiers: public, abstract
  - Summary: Pressed keyboard buttons
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.GameObjects.IMovementService.KeyChangedButtons` [L:41]
  - Modifiers: public, abstract
  - Summary: Changed keyboard buttons
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.GameObjects.IMovementService.ScrollButtons` [L:46]
  - Modifiers: public, abstract
  - Summary: Buttons that are done by scrolling
- `float Sharp.Shared.GameObjects.IMovementService.MaxSpeed` [L:31]
  - Modifiers: public, abstract
  - Summary: MaxSpeed in MoveData

#### Methods
- `Sharp.Shared.GameObjects.IPlayerMovementService? Sharp.Shared.GameObjects.IMovementService.AsPlayerMovementService([bool reinterpret = false])` [L:55]
  - Modifiers: public, abstract
  - Summary: Cast to CCSPlayer_MovementServices
- `void Sharp.Shared.GameObjects.IMovementService.TransientChangeMaxSpeed(float speed)` [L:60]
  - Modifiers: public, abstract
  - Summary: Temporarily change MaxSpeed without sending network update


### interface IObserverService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IObserverService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IObserverService.cs:31
- Generated: false
- Attributes: `[NetClass("CCSObserver_ObserverServices")]`
- Summary: ObserverServices is CCSObserver only

#### Properties
- `Sharp.Shared.Enums.ObserverMode Sharp.Shared.GameObjects.IObserverService.ObserverLastMode` [L:35]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.ObserverMode Sharp.Shared.GameObjects.IObserverService.ObserverMode` [L:39]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.IObserverService.ObserverTarget` [L:37]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameObjects.IObserverService.ForcedObserverMode` [L:33]
  - Modifiers: public, abstract


### interface IPaintKit : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.GameObjects.IPaintKit`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IPaintKit.cs:24
- Generated: false

#### Properties
- `bool Sharp.Shared.GameObjects.IPaintKit.IsLegacyModel` [L:32]
  - Modifiers: public, abstract, readonly
- `bool Sharp.Shared.GameObjects.IPaintKit.IsUseNormalModel` [L:31]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IPaintKit.DescriptionString` [L:28]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IPaintKit.DescriptionTag` [L:29]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameObjects.IPaintKit.Name` [L:27]
  - Modifiers: public, abstract, readonly
- `uint Sharp.Shared.GameObjects.IPaintKit.Id` [L:26]
  - Modifiers: public, abstract, readonly
- `uint Sharp.Shared.GameObjects.IPaintKit.Rarity` [L:30]
  - Modifiers: public, abstract, readonly


### interface IPerRoundStats : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IPerRoundStats`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IControllerActionTrackingService.cs:26
- Generated: false
- Attributes: `[NetClass("CSPerRoundStats_t")]`

#### Properties
- `int Sharp.Shared.GameObjects.IPerRoundStats.Assists` [L:32]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.CashEarned` [L:48]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.Damage` [L:34]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.Deaths` [L:30]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.EnemiesFlashed` [L:52]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.EquipmentValue` [L:36]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.HeadShotKills` [L:44]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.KillReward` [L:40]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.Kills` [L:28]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.LiveTime` [L:42]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.MoneySaved` [L:38]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.Objective` [L:46]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameObjects.IPerRoundStats.UtilityDamage` [L:50]
  - Modifiers: public, abstract


### interface IPingService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IPingService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IPingService.cs:31
- Generated: false
- Attributes: `[NetClass("CCSPlayer_PingServices")]`
- Summary: PingServices is CCSPlayerPawn only

#### Properties
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.IPingService.PlayerPingHandle` [L:41]
  - Modifiers: public, abstract
  - Summary: m_hPlayerPing

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<int> Sharp.Shared.GameObjects.IPingService.GetPlayerPingTokens()` [L:36]
  - Modifiers: public, abstract
  - Summary: m_flPlayerPingTokens


### interface IPlayerActionTrackingService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IPlayerActionTrackingService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IPlayerActionTrackingService.cs:30
- Generated: false
- Attributes: `[NetClass("CCSPlayer_ActionTrackingServices")]`
- Summary: ActionTrackingServices is CCSPlayerPawn only

#### Properties
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Shared.GameObjects.IPlayerActionTrackingService.LastWeaponBeforeC4AutoSwitchHandle` [L:35]
  - Modifiers: public, abstract
  - Summary: m_hLastWeaponBeforeC4AutoSwitch
- `bool Sharp.Shared.GameObjects.IPlayerActionTrackingService.IsRescuing` [L:40]
  - Modifiers: public, abstract
  - Summary: m_bIsRescuing


### interface IPlayerControllerComponent : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IPlayerControllerComponent`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IPlayerControllerComponent.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameObjects.IPlayerControllerComponent.GetPlayer()` [L:30]
  - Modifiers: public, abstract
  - Summary: Get player controller


### interface IPlayerMovementService : Sharp.Shared.GameObjects.IMovementService

- FullName: `Sharp.Shared.GameObjects.IPlayerMovementService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IMovementService.cs:64
- Generated: false
- Attributes: `[NetClass("CCSPlayer_MovementServices")]`

#### Properties
- `bool Sharp.Shared.GameObjects.IPlayerMovementService.DuckOverride` [L:89]
  - Modifiers: public, abstract
  - Summary: Force duck/crouch
- `bool Sharp.Shared.GameObjects.IPlayerMovementService.OldJumpPressed` [L:74]
  - Modifiers: public, abstract
  - Summary: Jump button held down
- `float Sharp.Shared.GameObjects.IPlayerMovementService.DuckSpeed` [L:69]
  - Modifiers: public, abstract
  - Summary: Duck speed, the lower it is the longer it takes to fully duck
- `float Sharp.Shared.GameObjects.IPlayerMovementService.JumpPressedTime` [L:79]
  - Modifiers: public, abstract
  - Summary: When does the player press their jump button
- `float Sharp.Shared.GameObjects.IPlayerMovementService.Stamina` [L:84]
  - Modifiers: public, abstract
  - Summary: Stamina value

#### Methods
- `void Sharp.Shared.GameObjects.IPlayerMovementService.TransientChangeStamina(float stamina)` [L:94]
  - Modifiers: public, abstract
  - Summary: Temporarily change stamina without sending network update


### interface IPlayerPawnComponent : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IPlayerPawnComponent`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IPlayerPawnComponent.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.GameEntities.IBasePlayerPawn? Sharp.Shared.GameObjects.IPlayerPawnComponent.GetPlayer()` [L:30]
  - Modifiers: public, abstract
  - Summary: Get player pawn


### interface IPlayerUseService : Sharp.Shared.GameObjects.IUseService

- FullName: `Sharp.Shared.GameObjects.IPlayerUseService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IUseService.cs:40
- Generated: false
- Attributes: `[NetClass("CCSPlayer_UseServices")]`

#### Properties
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameObjects.IPlayerUseService.LastKnownUseEntityHandle` [L:45]
  - Modifiers: public, abstract
  - Summary: m_hLastKnownUseEntity
- `float Sharp.Shared.GameObjects.IPlayerUseService.LastUseTimeStamp` [L:50]
  - Modifiers: public, abstract
  - Summary: LastUseTimeStamp
- `float Sharp.Shared.GameObjects.IPlayerUseService.TimeLastUsedWindow` [L:55]
  - Modifiers: public, abstract
  - Summary: m_flTimeLastUsedWindow


### interface IRadioService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IRadioService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IRadioService.cs:29
- Generated: false
- Attributes: `[NetClass("CCSPlayer_RadioServices")]`
- Summary: RadioService is CCSPlayerPawn only

#### Properties
- `bool Sharp.Shared.GameObjects.IRadioService.IgnoreRadio` [L:49]
  - Modifiers: public, abstract
  - Summary: m_bIgnoreRadio
- `float Sharp.Shared.GameObjects.IRadioService.C4PlantTalkTimer` [L:44]
  - Modifiers: public, abstract
  - Summary: m_flC4PlantTalkTimer
- `float Sharp.Shared.GameObjects.IRadioService.DefusingTalkTimer` [L:39]
  - Modifiers: public, abstract
  - Summary: m_flDefusingTalkTimer
- `float Sharp.Shared.GameObjects.IRadioService.GotHostageTalkTimer` [L:34]
  - Modifiers: public, abstract
  - Summary: m_flGotHostageTalkTimer

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<float> Sharp.Shared.GameObjects.IRadioService.GetRadioTokenSlots()` [L:54]
  - Modifiers: public, abstract
  - Summary: m_flRadioTokenSlots


### interface ISkeletonInstance : Sharp.Shared.GameObjects.IGameSceneNode

- FullName: `Sharp.Shared.GameObjects.ISkeletonInstance`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IBodyComponent.cs:67
- Generated: false
- Attributes: `[NetClass("CSkeletonInstance")]`

#### Properties
- `bool Sharp.Shared.GameObjects.ISkeletonInstance.DisableSolidCollisionsForHierarchy` [L:71]
  - Modifiers: public, abstract
- `uint Sharp.Shared.GameObjects.ISkeletonInstance.MaterialGroup` [L:73]
  - Modifiers: public, abstract

#### Methods
- `Sharp.Shared.GameObjects.IModelState Sharp.Shared.GameObjects.ISkeletonInstance.GetModelState()` [L:69]
  - Modifiers: public, abstract


### interface IUseService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IUseService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IUseService.cs:27
- Generated: false
- Attributes: `[NetClass("CPlayer_UseServices")]`

#### Methods
- `Sharp.Shared.GameObjects.IPlayerUseService? Sharp.Shared.GameObjects.IUseService.AsPlayerUseService([bool reinterpret = false])` [L:36]
  - Modifiers: public, abstract
  - Summary: Cast to CCSPlayer_UseServices


### interface IVPhysicsCollisionAttribute : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/ICollisionProperty.cs:76
- Generated: false

#### Properties
- `Sharp.Shared.Enums.CollisionGroupType Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.CollisionGroup` [L:81]
  - Modifiers: public, abstract
  - Summary: Collision group
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.InteractsAs` [L:87]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.InteractsExclude` [L:89]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.InteractsWith` [L:88]
  - Modifiers: public, abstract
- `uint Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.EntityId` [L:83]
  - Modifiers: public, abstract
- `uint Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.OwnerId` [L:84]
  - Modifiers: public, abstract
- `ushort Sharp.Shared.GameObjects.IVPhysicsCollisionAttribute.HierarchyId` [L:85]
  - Modifiers: public, abstract


### interface IWaterService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IWaterService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IWaterService.cs:29
- Generated: false
- Attributes: `[NetClass("CCSPlayer_WaterServices")]`
- Summary: WaterService is CCSPlayerPawn only

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.GameObjects.IWaterService.WaterJumpVel` [L:54]
  - Modifiers: public, abstract
  - Summary: m_vecWaterJumpVel
- `float Sharp.Shared.GameObjects.IWaterService.AirFinishedTime` [L:44]
  - Modifiers: public, abstract
  - Summary: m_AirFinishedTime
- `float Sharp.Shared.GameObjects.IWaterService.NextDrownDamageTime` [L:34]
  - Modifiers: public, abstract
  - Summary: m_NextDrownDamageTime
- `float Sharp.Shared.GameObjects.IWaterService.SwimSoundTime` [L:59]
  - Modifiers: public, abstract
  - Summary: m_flSwimSoundTime
- `float Sharp.Shared.GameObjects.IWaterService.WaterJumpTime` [L:49]
  - Modifiers: public, abstract
  - Summary: m_flWaterJumpTime
- `int Sharp.Shared.GameObjects.IWaterService.DrownDmgRate` [L:39]
  - Modifiers: public, abstract
  - Summary: m_nDrownDmgRate


### interface IWeaponData : Sharp.Shared.CStrike.IEntitySubclassVData

- FullName: `Sharp.Shared.GameObjects.IWeaponData`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IWeaponData.cs:27
- Generated: false
- Attributes: `[NetClass("CCSWeaponBaseVData")]`

#### Properties
- `Sharp.Shared.Enums.CStrikeWeaponCategory Sharp.Shared.GameObjects.IWeaponData.WeaponCategory` [L:42]
  - Modifiers: public, abstract, readonly
  - Summary: Weapon category
- `Sharp.Shared.Enums.CStrikeWeaponType Sharp.Shared.GameObjects.IWeaponData.WeaponType` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: Weapon type
- `Sharp.Shared.Enums.GearSlot Sharp.Shared.GameObjects.IWeaponData.GearSlot` [L:47]
  - Modifiers: public, abstract, readonly
  - Summary: Equipment slot
- `bool Sharp.Shared.GameObjects.IWeaponData.IsFullAuto` [L:67]
  - Modifiers: public, abstract, readonly
  - Summary: Whether weapon is fully automatic
- `bool Sharp.Shared.GameObjects.IWeaponData.IsMeleeWeapon` [L:62]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this is a melee weapon
- `float Sharp.Shared.GameObjects.IWeaponData.ArmorRatio` [L:107]
  - Modifiers: public, abstract
  - Summary: Armor penetration ratio
- `float Sharp.Shared.GameObjects.IWeaponData.CycleTime` [L:77]
  - Modifiers: public, abstract
  - Summary: How long does it take to perform a primary attack
- `float Sharp.Shared.GameObjects.IWeaponData.CycleTimeAlt` [L:82]
  - Modifiers: public, abstract
  - Summary: How long does it take to perform a secondary attack
- `float Sharp.Shared.GameObjects.IWeaponData.HeadshotMultiplier` [L:102]
  - Modifiers: public, abstract
  - Summary: Headshot damage multiplier
- `float Sharp.Shared.GameObjects.IWeaponData.MaxSpeed` [L:87]
  - Modifiers: public, abstract
  - Summary: Max walk speed when holding it
- `float Sharp.Shared.GameObjects.IWeaponData.MaxSpeedAlt` [L:92]
  - Modifiers: public, abstract
  - Summary: Max alt walk speed when holding it, for example awp with scope on
- `float Sharp.Shared.GameObjects.IWeaponData.Range` [L:112]
  - Modifiers: public, abstract
  - Summary: Weapon range
- `float Sharp.Shared.GameObjects.IWeaponData.RangeModifier` [L:117]
  - Modifiers: public, abstract
  - Summary: Distance damage falloff modifier
- `int Sharp.Shared.GameObjects.IWeaponData.Damage` [L:97]
  - Modifiers: public, abstract
  - Summary: Damage
- `int Sharp.Shared.GameObjects.IWeaponData.MaxClip` [L:32]
  - Modifiers: public, abstract
  - Summary: Maximum bullets in magazine
- `int Sharp.Shared.GameObjects.IWeaponData.NumBullets` [L:72]
  - Modifiers: public, abstract
  - Summary: Number of projectiles per shot
- `int Sharp.Shared.GameObjects.IWeaponData.Price` [L:52]
  - Modifiers: public, abstract
  - Summary: Purchase price
- `int Sharp.Shared.GameObjects.IWeaponData.PrimaryReserveAmmoMax` [L:57]
  - Modifiers: public, abstract
  - Summary: Maximum reserve ammunition


### interface IWeaponService : Sharp.Shared.GameObjects.IPlayerPawnComponent

- FullName: `Sharp.Shared.GameObjects.IWeaponService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IWeaponService.cs:31
- Generated: false
- Attributes: `[NetClass("CCSPlayer_WeaponServices")]`
- Summary: WeaponServices is only for CCSPlayerPawn

#### Properties
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameObjects.IWeaponService.ActiveWeapon` [L:75]
  - Modifiers: public, abstract, readonly
  - Summary: ActiveWeapon
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameObjects.IWeaponService.LastWeapon` [L:85]
  - Modifiers: public, abstract, readonly
  - Summary: Last used Weapon
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Shared.GameObjects.IWeaponService.ActiveWeaponHandle` [L:80]
  - Modifiers: public, abstract
  - Summary: m_hActiveWeapon
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Shared.GameObjects.IWeaponService.LastWeaponHandle` [L:90]
  - Modifiers: public, abstract
  - Summary: m_hLastWeapon
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Shared.GameObjects.IWeaponService.SavedWeaponHandle` [L:43]
  - Modifiers: public, abstract
  - Summary: m_hSavedWeapon
- `bool Sharp.Shared.GameObjects.IWeaponService.DisableAutoDeploy` [L:58]
  - Modifiers: public, abstract
  - Summary: m_bDisableAutoDeploy
- `bool Sharp.Shared.GameObjects.IWeaponService.IsPickingUpGroundWeapon` [L:63]
  - Modifiers: public, abstract
  - Summary: m_bIsPickingUpGroundWeapon
- `bool Sharp.Shared.GameObjects.IWeaponService.IsPickingUpItemWithUse` [L:48]
  - Modifiers: public, abstract
  - Summary: m_bIsPickingUpItemWithUse
- `bool Sharp.Shared.GameObjects.IWeaponService.PickedUpWeapon` [L:53]
  - Modifiers: public, abstract
  - Summary: m_bPickedUpWeapon
- `bool Sharp.Shared.GameObjects.IWeaponService.PreventWeaponPickup` [L:100]
  - Modifiers: public, abstract
  - Summary: m_bPreventWeaponPickup
- `float Sharp.Shared.GameObjects.IWeaponService.NextAttack` [L:38]
  - Modifiers: public, abstract
  - Summary: m_flNextAttack

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<ushort> Sharp.Shared.GameObjects.IWeaponService.GetAmmo()` [L:95]
  - Modifiers: public, abstract
  - Summary: m_iAmmo[32]
- `Sharp.Shared.CStrike.ISchemaList<Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseWeapon>> Sharp.Shared.GameObjects.IWeaponService.GetMyWeapons()` [L:70]
  - Modifiers: public, abstract
  - Summary: m_hMyWeapons


### enum KillTypes : System.Enum

- FullName: `Sharp.Shared.GameObjects.KillTypes`
- Kind: enum
- Modifiers: public
- Source: Sharp.Shared/GameObjects/IDamageService.cs:26
- Generated: false

Inheritance: object → System.ValueType → System.Enum → **KillTypes**

#### Enum Members
- `Sharp.Shared.GameObjects.KillTypes.Blast = 3` [L:31]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.Burn = 4` [L:32]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.Default = 1` [L:29]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.Headshot = 2` [L:30]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.None = 0` [L:28]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.Shock = 6` [L:34]
  - Modifiers: public, static, const
- `Sharp.Shared.GameObjects.KillTypes.Slash = 5` [L:33]
  - Modifiers: public, static, const


