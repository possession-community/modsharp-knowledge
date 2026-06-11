# Sharp.Shared.GameEntities

Project: Sharp.Shared
Types: 24 (0 generated)

### interface IBaseAnimGraph : Sharp.Shared.GameEntities.IBaseModelEntity

- FullName: `Sharp.Shared.GameEntities.IBaseAnimGraph`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseAnimGraph.cs:26
- Generated: false
- Attributes: `[NetClass("CBaseAnimGraph")]`

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseAnimGraph.Force` [L:36]
  - Modifiers: public, abstract
  - Summary: m_vecForce
- `bool Sharp.Shared.GameEntities.IBaseAnimGraph.AnimGraphUpdateEnabled` [L:31]
  - Modifiers: public, abstract
  - Summary: m_bAnimGraphUpdateEnabled
- `int Sharp.Shared.GameEntities.IBaseAnimGraph.ForceBone` [L:41]
  - Modifiers: public, abstract
  - Summary: m_nForceBone


### interface IBaseButton : Sharp.Shared.GameEntities.IBaseToggle

- FullName: `Sharp.Shared.GameEntities.IBaseButton`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseButton.cs:25
- Generated: false
- Attributes: `[NetClass("CBaseButton")]`

#### Properties
- `bool Sharp.Shared.GameEntities.IBaseButton.Disabled` [L:35]
  - Modifiers: public, abstract
  - Summary: m_bDisabled
- `bool Sharp.Shared.GameEntities.IBaseButton.Locked` [L:30]
  - Modifiers: public, abstract
  - Summary: m_bLocked
- `int Sharp.Shared.GameEntities.IBaseButton.State` [L:40]
  - Modifiers: public, abstract
  - Summary: m_nState


### interface IBaseCombatCharacter : Sharp.Shared.GameEntities.IBaseAnimGraph

- FullName: `Sharp.Shared.GameEntities.IBaseCombatCharacter`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseCombatCharacter.cs:25
- Generated: false
- Attributes: `[NetClass("CBaseCombatCharacter")]`

#### Properties
- `bool Sharp.Shared.GameEntities.IBaseCombatCharacter.ApplyStressDamage` [L:35]
  - Modifiers: public, abstract
  - Summary: m_bApplyStressDamage
- `float Sharp.Shared.GameEntities.IBaseCombatCharacter.ImpactEnergyScale` [L:30]
  - Modifiers: public, abstract
  - Summary: m_impactEnergyScale


### interface IBaseDoor : Sharp.Shared.GameEntities.IBaseToggle

- FullName: `Sharp.Shared.GameEntities.IBaseDoor`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseDoor.cs:26
- Generated: false
- Attributes: `[NetClass("CBaseDoor")]`

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseDoor.MoveDirParentSpace` [L:51]
  - Modifiers: public, abstract
  - Summary: m_vecMoveDirParentSpace
- `bool Sharp.Shared.GameEntities.IBaseDoor.ForceClosed` [L:41]
  - Modifiers: public, abstract
  - Summary: m_bForceClosed
- `bool Sharp.Shared.GameEntities.IBaseDoor.IsUsable` [L:46]
  - Modifiers: public, abstract
  - Summary: m_bIsUsable
- `bool Sharp.Shared.GameEntities.IBaseDoor.Locked` [L:31]
  - Modifiers: public, abstract
  - Summary: m_bLocked
- `float Sharp.Shared.GameEntities.IBaseDoor.BlockDamage` [L:36]
  - Modifiers: public, abstract
  - Summary: m_flBlockDamage


### interface IBaseEntity : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.GameEntities.IBaseEntity`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseEntity.cs:36
- Generated: false
- Attributes: `[NetClass("CBaseEntity")]`

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEntities.IBaseEntity.Team` [L:75]
  - Modifiers: public, abstract, readonly
  - Summary: Team
- `Sharp.Shared.Enums.EntityEffects Sharp.Shared.GameEntities.IBaseEntity.Effects` [L:149]
  - Modifiers: public, abstract
  - Summary: m_fEffects
- `Sharp.Shared.Enums.EntityFlags Sharp.Shared.GameEntities.IBaseEntity.Flags` [L:154]
  - Modifiers: public, abstract
  - Summary: m_fFlags
- `Sharp.Shared.Enums.LifeState Sharp.Shared.GameEntities.IBaseEntity.LifeState` [L:70]
  - Modifiers: public, abstract, readonly
  - Summary: Lifestate
- `Sharp.Shared.Enums.MoveCollideType Sharp.Shared.GameEntities.IBaseEntity.MoveCollide` [L:80]
  - Modifiers: public, abstract, readonly
  - Summary: MoveCollide
- `Sharp.Shared.Enums.MoveType Sharp.Shared.GameEntities.IBaseEntity.ActualMoveType` [L:90]
  - Modifiers: public, abstract, readonly
  - Summary: ActualMoveType
- `Sharp.Shared.Enums.MoveType Sharp.Shared.GameEntities.IBaseEntity.MoveType` [L:85]
  - Modifiers: public, abstract, readonly
  - Summary: MoveType
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBaseEntity.EffectEntity` [L:184]
  - Modifiers: public, abstract, readonly
  - Summary: m_hEffectEntity
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBaseEntity.GroundEntity` [L:174]
  - Modifiers: public, abstract, readonly
  - Summary: m_hGroundEntity
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBaseEntity.OwnerEntity` [L:144]
  - Modifiers: public, abstract, readonly
  - Summary: m_hOwnerEntity
- `Sharp.Shared.GameEntities.IBaseFilter? Sharp.Shared.GameEntities.IBaseEntity.DamageFilterEntity` [L:194]
  - Modifiers: public, abstract, readonly
  - Summary: Get the damage filter entity applied to this entity
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBaseEntity.EffectEntityHandle` [L:179]
  - Modifiers: public, abstract
  - Summary: m_hEffectEntity
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBaseEntity.GroundEntityHandle` [L:169]
  - Modifiers: public, abstract, readonly
  - Summary: m_hGroundEntity Handle
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBaseEntity.Handle` [L:41]
  - Modifiers: public, abstract, readonly
  - Summary: Gets the raw handle stored on the entity
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBaseEntity.RefHandle` [L:50]
  - Modifiers: public, abstract, readonly
  - Summary: Gets the true, usable handle for this entity.
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseFilter> Sharp.Shared.GameEntities.IBaseEntity.DamageFilterEntityHandle` [L:189]
  - Modifiers: public, abstract
  - Summary: Get the damage filter entity handle applied to this entity
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.BaseVelocity` [L:224]
  - Modifiers: public, abstract
  - Summary: Base velocity Setting this will apply extra velocity to the final speed
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.GameEntities.IBaseEntity.Index` [L:104]
  - Modifiers: public, abstract, readonly
  - Summary: Return the index of this entity
- `bool Sharp.Shared.GameEntities.IBaseEntity.AllowTakesDamage` [L:139]
  - Modifiers: public, abstract
  - Summary: Is this entity allowed to take damage
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsAlive` [L:65]
  - Modifiers: public, abstract, readonly
  - Summary: Is this entity alive
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsPlayerController` [L:567]
  - Modifiers: public, abstract, readonly
  - Summary: Check if the entity is CCSPlayerController
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsPlayerPawn` [L:572]
  - Modifiers: public, abstract, readonly
  - Summary: Check if the entity is CBasePlayerPawn
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsValidEntity` [L:199]
  - Modifiers: public, abstract, readonly
  - Summary: Check if this entity is valid
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsWeapon` [L:562]
  - Modifiers: public, abstract, readonly
  - Summary: Check if the entity is BaseWeapon
- `float Sharp.Shared.GameEntities.IBaseEntity.CreateTime` [L:234]
  - Modifiers: public, abstract, readonly
  - Summary: m_flCreateTime
- `float Sharp.Shared.GameEntities.IBaseEntity.GravityScale` [L:239]
  - Modifiers: public, abstract
  - Summary: m_flGravityScale
- `float Sharp.Shared.GameEntities.IBaseEntity.Speed` [L:164]
  - Modifiers: public, abstract
  - Summary: m_flSpeed
- `int Sharp.Shared.GameEntities.IBaseEntity.EFlags` [L:159]
  - Modifiers: public, abstract
  - Summary: m_iEFlags
- `int Sharp.Shared.GameEntities.IBaseEntity.Health` [L:55]
  - Modifiers: public, abstract
  - Summary: Health
- `int Sharp.Shared.GameEntities.IBaseEntity.MaxHealth` [L:60]
  - Modifiers: public, abstract
  - Summary: Max health
- `int Sharp.Shared.GameEntities.IBaseEntity.NextThinkTick` [L:229]
  - Modifiers: public, abstract
  - Summary: m_nNextThinkTick
- `string Sharp.Shared.GameEntities.IBaseEntity.Classname` [L:111]
  - Modifiers: public, abstract, readonly
  - Summary: 读取Classname
- `string Sharp.Shared.GameEntities.IBaseEntity.GlobalName` [L:130]
  - Modifiers: public, abstract
  - Summary: m_iGlobalname
- `string Sharp.Shared.GameEntities.IBaseEntity.HammerId` [L:125]
  - Modifiers: public, abstract, readonly
  - Summary: Get the HammerId of this entity
- `string Sharp.Shared.GameEntities.IBaseEntity.Name` [L:120]
  - Modifiers: public, abstract, readonly
  - Summary: Get the targetname of this entity
- `string Sharp.Shared.GameEntities.IBaseEntity.PrivateVScripts` [L:244]
  - Modifiers: public, abstract, readonly
  - Summary: m_iszPrivateVScripts
- `uint Sharp.Shared.GameEntities.IBaseEntity.SpawnFlags` [L:95]
  - Modifiers: public, abstract
  - Summary: Spawn Flags
- `uint Sharp.Shared.GameEntities.IBaseEntity.SubclassID` [L:249]
  - Modifiers: public, abstract, readonly
  - Summary: m_nSubclassID

#### Methods
- `Sharp.Shared.CStrike.ISchemaList<Sharp.Shared.Types.ResponseContext> Sharp.Shared.GameEntities.IBaseEntity.GetResponseContexts()` [L:603]
  - Modifiers: public, abstract
  - Summary: m_ResponseContexts
- `Sharp.Shared.GameEntities.IBaseGrenadeProjectile? Sharp.Shared.GameEntities.IBaseEntity.AsBaseGrenadeProjectile()` [L:578]
  - Modifiers: public, abstract
  - Summary: Cast to BaseGrenade It will return null if the entity is not a grenade
- `Sharp.Shared.GameEntities.IBasePlayerPawn? Sharp.Shared.GameEntities.IBaseEntity.AsBasePlayerPawn([bool safeCheck = true])` [L:533]
  - Modifiers: public, abstract
  - Summary: Cast to
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameEntities.IBaseEntity.AsBaseWeapon([bool safeCheck = true])` [L:557]
  - Modifiers: public, abstract
  - Summary: Cast to BaseWeapon It will return null if the entity is not Weapon
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEntities.IBaseEntity.AsPlayerController([bool safeCheck = true])` [L:550]
  - Modifiers: public, abstract
  - Summary: Cast to PlayerController It will return null if the entity is not PlayerController
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEntities.IBaseEntity.AsPlayerPawn([bool safeCheck = true])` [L:543]
  - Modifiers: public, abstract
  - Summary: Cast to
- `Sharp.Shared.GameObjects.IBodyComponent Sharp.Shared.GameEntities.IBaseEntity.GetBodyComponent()` [L:598]
  - Modifiers: public, abstract
  - Summary: m_CBodyComponent
- `Sharp.Shared.GameObjects.ICollisionProperty? Sharp.Shared.GameEntities.IBaseEntity.GetCollisionProperty()` [L:204]
  - Modifiers: public, abstract
  - Summary: CollisionProperty
- `Sharp.Shared.Types.SoundOpEventGuid Sharp.Shared.GameEntities.IBaseEntity.EmitSound(string sound, [float? volume = null], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:514]
  - Modifiers: public, abstract
  - Summary: Play a sound on this entity
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.GetAbsAngles()` [L:481]
  - Modifiers: public, abstract
  - Summary: Get the absolute angle in world space
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.GetAbsOrigin()` [L:491]
  - Modifiers: public, abstract
  - Summary: Get the entity absolute origin in world space
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.GetAbsVelocity()` [L:460]
  - Modifiers: public, abstract
  - Summary: SGet the absolute velocity in world space, EFL_DIRTY_ABSVELOCITY
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.GetCenter()` [L:501]
  - Modifiers: public, abstract
  - Summary: Get the center position of this entity in world space
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.GetLocalVelocity()` [L:471]
  - Modifiers: public, abstract
  - Summary: Get the relative velocity in world space, networked
- `T Sharp.Shared.GameEntities.IBaseEntity.As<T>() where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:583]
  - Modifiers: public, abstract
  - Summary: Cast entity to other types
- `bool Sharp.Shared.GameEntities.IBaseEntity.AcceptInput(string input, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller, float value, [int outputId = 0])` [L:317]
  - Modifiers: public, abstract
  - Summary: Fires an entity input.
- `bool Sharp.Shared.GameEntities.IBaseEntity.AcceptInput(string input, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller, int value, [int outputId = 0])` [L:303]
  - Modifiers: public, abstract
  - Summary: Fires an entity input.
- `bool Sharp.Shared.GameEntities.IBaseEntity.AcceptInput(string input, [Sharp.Shared.GameEntities.IBaseEntity? activator = null], [Sharp.Shared.GameEntities.IBaseEntity? caller = null], [string? value = null], [int outputId = 0])` [L:289]
  - Modifiers: public, abstract
  - Summary: Fires an entity input.
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsMarkedForDeletion()` [L:262]
  - Modifiers: public, abstract
  - Summary: Check if this entity is maked for deletion
- `bool Sharp.Shared.GameEntities.IBaseEntity.IsValid()` [L:256]
  - Modifiers: public, abstract
  - Summary: Check if this entity is valid
- `long Sharp.Shared.GameEntities.IBaseEntity.DispatchTraceAttack(Sharp.Shared.Types.TakeDamageInfo* info, [bool bypassHook = false])` [L:403]
  - Modifiers: public, abstract
  - Summary: Applies damage to this entity using trace attack logic (Unsafe).
- `long Sharp.Shared.GameEntities.IBaseEntity.DispatchTraceAttack(in Sharp.Shared.Types.TakeDamageInfo info, [bool bypassHook = false])` [L:386]
  - Modifiers: public, abstract
  - Summary: Applies damage to this entity using trace attack logic.
- `void Sharp.Shared.GameEntities.IBaseEntity.AddIOEvent(float delay, string input, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller, float value, [int outputId = 0])` [L:364]
  - Modifiers: public, abstract
  - Summary: Add an IO event to this entity
- `void Sharp.Shared.GameEntities.IBaseEntity.AddIOEvent(float delay, string input, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller, int value, [int outputId = 0])` [L:348]
  - Modifiers: public, abstract
  - Summary: Add an IO event to this entity
- `void Sharp.Shared.GameEntities.IBaseEntity.AddIOEvent(float delay, string input, [Sharp.Shared.GameEntities.IBaseEntity? activator = null], [Sharp.Shared.GameEntities.IBaseEntity? caller = null], [string? value = null], [int outputId = 0])` [L:332]
  - Modifiers: public, abstract
  - Summary: Add an IO event to this entity
- `void Sharp.Shared.GameEntities.IBaseEntity.ApplyAbsVelocityImpulse(Sharp.Shared.Types.Vector velocity)` [L:454]
  - Modifiers: public, abstract
  - Summary: Apply an absolute velocity to this entity. CurrentAbsVelocity + velocity = NewVelocity
- `void Sharp.Shared.GameEntities.IBaseEntity.ChangeTeam(Sharp.Shared.Enums.CStrikeTeam team)` [L:279]
  - Modifiers: public, abstract
  - Summary: Change entity's team
- `void Sharp.Shared.GameEntities.IBaseEntity.CollisionRulesChanged()` [L:506]
  - Modifiers: public, abstract
  - Summary: Update collision rules
- `void Sharp.Shared.GameEntities.IBaseEntity.DispatchSpawn([System.Collections.Generic.IReadOnlyDictionary<string, Sharp.Shared.Types.KeyValuesVariantValueItem>? keyValues = null])` [L:591]
  - Modifiers: public, abstract
  - Summary: Spawn entity with entity field values
- `void Sharp.Shared.GameEntities.IBaseEntity.Kill()` [L:267]
  - Modifiers: public, abstract
  - Summary: Mark this entity for deletion and delete
- `void Sharp.Shared.GameEntities.IBaseEntity.SetAbsAngles(Sharp.Shared.Types.Vector angles)` [L:486]
  - Modifiers: public, abstract
  - Summary: Set the absolute angle in world space, EFL_DIRTY_ABSTRANSFORM
- `void Sharp.Shared.GameEntities.IBaseEntity.SetAbsOrigin(Sharp.Shared.Types.Vector origin)` [L:496]
  - Modifiers: public, abstract
  - Summary: Set the entity absolute origin in world space. EFL_DIRTY_ABSTRANSFORM
- `void Sharp.Shared.GameEntities.IBaseEntity.SetAbsVelocity(Sharp.Shared.Types.Vector velocity)` [L:465]
  - Modifiers: public, abstract
  - Summary: Set the absolute velocity in world space, EFL_DIRTY_ABSVELOCITY
- `void Sharp.Shared.GameEntities.IBaseEntity.SetClassname(string classname)` [L:273]
  - Modifiers: public, abstract
  - Summary: Update ClassnameDoing this will impact entity clean up on round end
- `void Sharp.Shared.GameEntities.IBaseEntity.SetCollisionGroup(Sharp.Shared.Enums.CollisionGroupType type)` [L:524]
  - Modifiers: public, abstract
  - Summary: Set an entitiy's collision group
- `void Sharp.Shared.GameEntities.IBaseEntity.SetGravityScale(float scale)` [L:449]
  - Modifiers: public, abstract
  - Summary: Set GravityScale
- `void Sharp.Shared.GameEntities.IBaseEntity.SetGroundEntity(Sharp.Shared.GameEntities.IBaseEntity? ground, Sharp.Shared.GameEntities.IBaseEntity? unknown)` [L:425]
  - Modifiers: public, abstract
  - Summary: Set GroundEntity
- `void Sharp.Shared.GameEntities.IBaseEntity.SetLocalVelocity(Sharp.Shared.Types.Vector velocity)` [L:476]
  - Modifiers: public, abstract
  - Summary: Set the relative velocity in world space, networked
- `void Sharp.Shared.GameEntities.IBaseEntity.SetModel(string model)` [L:414]
  - Modifiers: public, abstract
  - Summary: Set entity model, Only works on ModelEntity
- `void Sharp.Shared.GameEntities.IBaseEntity.SetMoveType(Sharp.Shared.Enums.MoveType type)` [L:444]
  - Modifiers: public, abstract
  - Summary: Set movetype
- `void Sharp.Shared.GameEntities.IBaseEntity.SetName(string name)` [L:408]
  - Modifiers: public, abstract
  - Summary: Set entity targetname
- `void Sharp.Shared.GameEntities.IBaseEntity.SetOwner(Sharp.Shared.GameEntities.IBaseEntity? owner)` [L:420]
  - Modifiers: public, abstract
  - Summary: Set entity owner
- `void Sharp.Shared.GameEntities.IBaseEntity.SetSolid(Sharp.Shared.Enums.SolidType solid)` [L:431]
  - Modifiers: public, abstract
  - Summary: Set solid type, only works on ModelEntity
- `void Sharp.Shared.GameEntities.IBaseEntity.StopSound(string sound)` [L:519]
  - Modifiers: public, abstract
  - Summary: Stop the sound from playing on this entity
- `void Sharp.Shared.GameEntities.IBaseEntity.Teleport([Sharp.Shared.Types.Vector? position = null], [Sharp.Shared.Types.Vector? angles = null], [Sharp.Shared.Types.Vector? velocity = null])` [L:439]
  - Modifiers: public, abstract
  - Summary: Teleport

#### Obsolete Members
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.AbsVelocity` [L:218] — Use GetAbsVelocity/GetAbsVelocity, will be removed in 2.2
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseEntity.Velocity` [L:211] — Use GetLocalVelocity/GetLocalVelocity, will be removed in 2.2


### interface IBaseFilter : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IBaseFilter`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseFilter.cs:25
- Generated: false
- Attributes: `[NetClass("CBaseFilter")]`

#### Properties
- `bool Sharp.Shared.GameEntities.IBaseFilter.Negated` [L:30]
  - Modifiers: public, abstract
  - Summary: m_bNegated


### interface IBaseGrenadeProjectile : Sharp.Shared.GameEntities.IBaseAnimGraph

- FullName: `Sharp.Shared.GameEntities.IBaseGrenadeProjectile`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseGrenadeProjectile.cs:26
- Generated: false
- Attributes: `[NetClass("CBaseCSGrenadeProjectile")]`

#### Properties
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEntities.IBaseGrenadeProjectile.ThrowerEntity` [L:66]
  - Modifiers: public, abstract, readonly
  - Summary: m_hThrower
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IPlayerPawn> Sharp.Shared.GameEntities.IBaseGrenadeProjectile.ThrowerEntityHandle` [L:61]
  - Modifiers: public, abstract
  - Summary: m_hThrower
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseGrenadeProjectile.InitialPosition` [L:71]
  - Modifiers: public, abstract, readonly
  - Summary: m_vInitialPosition
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseGrenadeProjectile.InitialVelocity` [L:76]
  - Modifiers: public, abstract, readonly
  - Summary: m_vInitialVelocity
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseGrenadeProjectile.LastHitSurfaceNormal` [L:86]
  - Modifiers: public, abstract, readonly
  - Summary: m_vecLastHitSurfaceNormal
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseGrenadeProjectile.OriginalSpawnLocation` [L:81]
  - Modifiers: public, abstract, readonly
  - Summary: m_vecOriginalSpawnLocation
- `bool Sharp.Shared.GameEntities.IBaseGrenadeProjectile.HasEverHitEnemy` [L:102]
  - Modifiers: public, abstract
  - Summary: m_bHasEverHitEnemy
- `bool Sharp.Shared.GameEntities.IBaseGrenadeProjectile.IsSmokeGrenade` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: m_bIsSmokeGrenade
- `float Sharp.Shared.GameEntities.IBaseGrenadeProjectile.Damage` [L:51]
  - Modifiers: public, abstract
  - Summary: m_flDamage
- `float Sharp.Shared.GameEntities.IBaseGrenadeProjectile.DamageRadius` [L:46]
  - Modifiers: public, abstract
  - Summary: m_DmgRadius
- `float Sharp.Shared.GameEntities.IBaseGrenadeProjectile.DetonateTime` [L:56]
  - Modifiers: public, abstract
  - Summary: m_flDetonateTime
- `float Sharp.Shared.GameEntities.IBaseGrenadeProjectile.SpawnTime` [L:36]
  - Modifiers: public, abstract
  - Summary: m_flSpawnTime
- `int Sharp.Shared.GameEntities.IBaseGrenadeProjectile.Bounces` [L:91]
  - Modifiers: public, abstract
  - Summary: m_nBounces
- `int Sharp.Shared.GameEntities.IBaseGrenadeProjectile.TicksAtZeroVelocity` [L:96]
  - Modifiers: public, abstract
  - Summary: m_nTicksAtZeroVelocity
- `ushort Sharp.Shared.GameEntities.IBaseGrenadeProjectile.ItemDefinitionIndex` [L:41]
  - Modifiers: public, abstract
  - Summary: m_nItemIndex


### interface IBaseModelEntity : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IBaseModelEntity`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseModelEntity.cs:28
- Generated: false
- Attributes: `[NetClass("CBaseModelEntity")]`

#### Properties
- `Sharp.Shared.Enums.RenderFx Sharp.Shared.GameEntities.IBaseModelEntity.RenderFx` [L:43]
  - Modifiers: public, abstract
  - Summary: m_nRenderFX
- `Sharp.Shared.Enums.RenderMode Sharp.Shared.GameEntities.IBaseModelEntity.RenderMode` [L:38]
  - Modifiers: public, abstract
  - Summary: m_nRenderMode
- `Sharp.Shared.Types.Color32 Sharp.Shared.GameEntities.IBaseModelEntity.RenderColor` [L:48]
  - Modifiers: public, abstract
  - Summary: m_clrColor
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseModelEntity.ViewOffset` [L:78]
  - Modifiers: public, abstract, readonly
  - Summary: m_vecViewOffset
- `bool Sharp.Shared.GameEntities.IBaseModelEntity.AllowFadeInView` [L:53]
  - Modifiers: public, abstract
  - Summary: m_bAllowFadeInView
- `float Sharp.Shared.GameEntities.IBaseModelEntity.DissolveStartTime` [L:33]
  - Modifiers: public, abstract
  - Summary: m_flDissolveStartTime
- `float Sharp.Shared.GameEntities.IBaseModelEntity.FadeMaxDistance` [L:63]
  - Modifiers: public, abstract
  - Summary: m_fadeMaxDist
- `float Sharp.Shared.GameEntities.IBaseModelEntity.FadeMinDistance` [L:58]
  - Modifiers: public, abstract
  - Summary: m_fadeMinDist
- `float Sharp.Shared.GameEntities.IBaseModelEntity.FadeScale` [L:68]
  - Modifiers: public, abstract
  - Summary: m_flFadeScale
- `float Sharp.Shared.GameEntities.IBaseModelEntity.ShadowStrength` [L:73]
  - Modifiers: public, abstract
  - Summary: m_flShadowStrength

#### Methods
- `Sharp.Shared.GameObjects.IGlowProperty Sharp.Shared.GameEntities.IBaseModelEntity.GetGlowProperty()` [L:124]
  - Modifiers: public, abstract
  - Summary: GlowProperty
- `int Sharp.Shared.GameEntities.IBaseModelEntity.LookupAttachment(string attachment)` [L:94]
  - Modifiers: public, abstract
  - Summary: Get the given attachment's index
- `int Sharp.Shared.GameEntities.IBaseModelEntity.LookupBone(string bone)` [L:105]
  - Modifiers: public, abstract
  - Summary: Get the index of the bone
- `void Sharp.Shared.GameEntities.IBaseModelEntity.GetAttachment(int attachment, out Sharp.Shared.Types.Vector origin, out Sharp.Shared.Types.Vector angles)` [L:99]
  - Modifiers: public, abstract
  - Summary: Get the given attachment's origin and angles
- `void Sharp.Shared.GameEntities.IBaseModelEntity.GetBoneTransform(int bone, out Sharp.Shared.Types.Matrix3x4 matrix)` [L:109]
  - Modifiers: public, abstract
- `void Sharp.Shared.GameEntities.IBaseModelEntity.SetBodyGroupByName(string name, int value)` [L:83]
  - Modifiers: public, abstract
  - Summary: Sets a BodyGroup by name.
- `void Sharp.Shared.GameEntities.IBaseModelEntity.SetCollisionBounds(Sharp.Shared.Types.Vector mins, Sharp.Shared.Types.Vector maxs)` [L:119]
  - Modifiers: public, abstract
  - Summary: Set collision bounding box
- `void Sharp.Shared.GameEntities.IBaseModelEntity.SetMaterialGroupMask(ulong mask)` [L:88]
  - Modifiers: public, abstract
  - Summary: Set the mesh group mask of this entity.
- `void Sharp.Shared.GameEntities.IBaseModelEntity.SetModelScale(float scale)` [L:114]
  - Modifiers: public, abstract
  - Summary: Set model scale, will not work if the model has BoneMerge flag


### interface IBaseParticle : Sharp.Shared.GameEntities.IBaseModelEntity

- FullName: `Sharp.Shared.GameEntities.IBaseParticle`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseParticle.cs:27
- Generated: false
- Attributes: `[NetClass("CParticleSystem")]`

#### Properties
- `Sharp.Shared.Types.Color32 Sharp.Shared.GameEntities.IBaseParticle.TintColor` [L:97]
  - Modifiers: public, abstract
  - Summary: m_clrTint
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseParticle.DataControlPointValue` [L:87]
  - Modifiers: public, abstract
  - Summary: m_vecDataCPValue
- `bool Sharp.Shared.GameEntities.IBaseParticle.Active` [L:37]
  - Modifiers: public, abstract
  - Summary: m_bActive
- `bool Sharp.Shared.GameEntities.IBaseParticle.Frozen` [L:42]
  - Modifiers: public, abstract
  - Summary: m_bFrozen
- `bool Sharp.Shared.GameEntities.IBaseParticle.NoFreeze` [L:67]
  - Modifiers: public, abstract
  - Summary: m_bNoFreeze
- `bool Sharp.Shared.GameEntities.IBaseParticle.NoRamp` [L:72]
  - Modifiers: public, abstract
  - Summary: m_bNoRamp
- `bool Sharp.Shared.GameEntities.IBaseParticle.StartActive` [L:77]
  - Modifiers: public, abstract
  - Summary: m_bStartActive
- `float Sharp.Shared.GameEntities.IBaseParticle.FreezeTransitionDuration` [L:47]
  - Modifiers: public, abstract
  - Summary: m_flFreezeTransitionDuration
- `float Sharp.Shared.GameEntities.IBaseParticle.PreSimTime` [L:62]
  - Modifiers: public, abstract
  - Summary: m_flPreSimTime
- `float Sharp.Shared.GameEntities.IBaseParticle.StartTime` [L:57]
  - Modifiers: public, abstract
  - Summary: m_flStartTime
- `int Sharp.Shared.GameEntities.IBaseParticle.DataControlPoint` [L:82]
  - Modifiers: public, abstract
  - Summary: m_nDataCP
- `int Sharp.Shared.GameEntities.IBaseParticle.StopType` [L:52]
  - Modifiers: public, abstract
  - Summary: m_nStopType
- `int Sharp.Shared.GameEntities.IBaseParticle.TintControlPoint` [L:92]
  - Modifiers: public, abstract
  - Summary: m_nTintCP
- `string Sharp.Shared.GameEntities.IBaseParticle.SnapshotFileName` [L:32]
  - Modifiers: public, abstract
  - Summary: m_szSnapshotFileName

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity>> Sharp.Shared.GameEntities.IBaseParticle.GetControlPointEntities()` [L:112]
  - Modifiers: public, abstract
  - Summary: m_hControlPointEnts
- `Sharp.Shared.CStrike.ISchemaArray<Sharp.Shared.Types.Vector> Sharp.Shared.GameEntities.IBaseParticle.GetServerControlPoints()` [L:102]
  - Modifiers: public, abstract
  - Summary: m_vServerControlPoints
- `Sharp.Shared.CStrike.ISchemaArray<byte> Sharp.Shared.GameEntities.IBaseParticle.GetServerControlPointAssignments()` [L:107]
  - Modifiers: public, abstract
  - Summary: m_iServerControlPointAssignments


### interface IBasePlayerPawn : Sharp.Shared.GameEntities.IBaseCombatCharacter

- FullName: `Sharp.Shared.GameEntities.IBasePlayerPawn`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBasePlayerPawn.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayerPawnBase")]`

#### Properties
- `Sharp.Shared.Enums.PlayerState Sharp.Shared.GameEntities.IBasePlayerPawn.State` [L:134]
  - Modifiers: public, abstract
  - Summary: PlayerState
- `bool Sharp.Shared.GameEntities.IBasePlayerPawn.Respawning` [L:139]
  - Modifiers: public, abstract, readonly
  - Summary: m_bRespawning
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.DeathTime` [L:124]
  - Modifiers: public, abstract
  - Summary: m_flDeathTime
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.FlashDuration` [L:154]
  - Modifiers: public, abstract
  - Summary: How long does the flashbang effect last
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.FlashMaxAlpha` [L:149]
  - Modifiers: public, abstract
  - Summary: Alpha for flashbang effect
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.NextRadarUpdateTime` [L:159]
  - Modifiers: public, abstract
  - Summary: m_fNextRadarUpdateTime
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.NextSuicideTime` [L:129]
  - Modifiers: public, abstract
  - Summary: m_fNextSuicideTime
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.ProgressBarStartTime` [L:164]
  - Modifiers: public, abstract
  - Summary: m_flProgressBarStartTime
- `float Sharp.Shared.GameEntities.IBasePlayerPawn.TimeLastHurt` [L:119]
  - Modifiers: public, abstract
  - Summary: m_fTimeLastHurt
- `int Sharp.Shared.GameEntities.IBasePlayerPawn.NumSpawns` [L:144]
  - Modifiers: public, abstract, readonly
  - Summary: m_iNumSpawns
- `int Sharp.Shared.GameEntities.IBasePlayerPawn.ProgressBarDuration` [L:169]
  - Modifiers: public, abstract
  - Summary: m_iProgressBarDuration
- `uint Sharp.Shared.GameEntities.IBasePlayerPawn.HideHud` [L:114]
  - Modifiers: public, abstract
  - Summary: m_iHideHUD

#### Methods
- `Sharp.Shared.GameEntities.IObserverPawn? Sharp.Shared.GameEntities.IBasePlayerPawn.AsObserver()` [L:62]
  - Modifiers: public, abstract
  - Summary: Cast to CCSObserverPawn
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEntities.IBasePlayerPawn.GetController()` [L:67]
  - Modifiers: public, abstract
  - Summary: Gets the Controller corresponding to the current PlayerPawn
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEntities.IBasePlayerPawn.GetOriginalController()` [L:72]
  - Modifiers: public, abstract
  - Summary: m_hOriginalController
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEntities.IBasePlayerPawn.AsPlayer()` [L:57]
  - Modifiers: public, abstract
  - Summary: Cast to CCSPlayerPawn
- `Sharp.Shared.GameObjects.ICameraService? Sharp.Shared.GameEntities.IBasePlayerPawn.GetCameraService()` [L:99]
  - Modifiers: public, abstract
  - Summary: CameraService
- `Sharp.Shared.GameObjects.IMovementService? Sharp.Shared.GameEntities.IBasePlayerPawn.GetMovementService()` [L:104]
  - Modifiers: public, abstract
  - Summary: MoveService
- `Sharp.Shared.GameObjects.IUseService? Sharp.Shared.GameEntities.IBasePlayerPawn.GetUseService()` [L:109]
  - Modifiers: public, abstract
  - Summary: UseService
- `Sharp.Shared.Types.SoundOpEventGuid Sharp.Shared.GameEntities.IBasePlayerPawn.EmitSoundClient(string sound, [float? volume = null])` [L:89]
  - Modifiers: public, abstract
  - Summary: Play a soundevent to this player, other player won't hear it
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBasePlayerPawn.GetEyeAngles()` [L:77]
  - Modifiers: public, abstract
  - Summary: Eye angles
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBasePlayerPawn.GetEyePosition()` [L:82]
  - Modifiers: public, abstract
  - Summary: Eye position
- `bool Sharp.Shared.GameEntities.IBasePlayerPawn.IsPlayer([bool nativeCall = false])` [L:51]
  - Modifiers: public, abstract
  - Summary: Check if entity is CCSPlayerPawn or CCSObserverPawn
- `void Sharp.Shared.GameEntities.IBasePlayerPawn.Print(Sharp.Shared.Enums.HudPrintChannel channel, string message, [string? param1 = null], [string? param2 = null], [string? param3 = null], [string? param4 = null])` [L:33]
  - Modifiers: public, abstract
  - Summary: Print message to this player
- `void Sharp.Shared.GameEntities.IBasePlayerPawn.PrintCenterHtml(string message, [int duration = 1])` [L:46]
  - Modifiers: public, abstract
  - Summary: Print a hud message with limited html format support to this player.
- `void Sharp.Shared.GameEntities.IBasePlayerPawn.TransientChangeTeam(Sharp.Shared.Enums.CStrikeTeam team)` [L:94]
  - Modifiers: public, abstract
  - Summary: Change m_iTeamNum without sending update state to the client


### interface IBaseTeam : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IBaseTeam`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseTeam.cs:25
- Generated: false
- Attributes: `[NetClass("CCSTeam")]`

#### Properties
- `float Sharp.Shared.GameEntities.IBaseTeam.NextResourceTime` [L:55]
  - Modifiers: public, abstract
  - Summary: m_flNextResourceTime
- `int Sharp.Shared.GameEntities.IBaseTeam.LastUpdateSentAt` [L:50]
  - Modifiers: public, abstract
  - Summary: m_iLastUpdateSentAt
- `int Sharp.Shared.GameEntities.IBaseTeam.Score` [L:30]
  - Modifiers: public, abstract
  - Summary: Score
- `int Sharp.Shared.GameEntities.IBaseTeam.ScoreFirstHalf` [L:35]
  - Modifiers: public, abstract
  - Summary: Score of FirstHalf
- `int Sharp.Shared.GameEntities.IBaseTeam.ScoreOvertime` [L:45]
  - Modifiers: public, abstract
  - Summary: Score of Overtime
- `int Sharp.Shared.GameEntities.IBaseTeam.ScoreSecondHalf` [L:40]
  - Modifiers: public, abstract
  - Summary: Score of SecondHalf


### interface IBaseToggle : Sharp.Shared.GameEntities.IBaseModelEntity

- FullName: `Sharp.Shared.GameEntities.IBaseToggle`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseToggle.cs:27
- Generated: false
- Attributes: `[NetClass("CBaseToggle")]`

#### Properties
- `Sharp.Shared.Enums.ToggleState Sharp.Shared.GameEntities.IBaseToggle.ToggleState` [L:62]
  - Modifiers: public, abstract
  - Summary: m_toggle_state
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBaseToggle.ActivatorEntity` [L:52]
  - Modifiers: public, abstract, readonly
  - Summary: m_hActivator
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBaseToggle.ActivatorEntityHandle` [L:57]
  - Modifiers: public, abstract, readonly
  - Summary: m_hActivator
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseToggle.Position1` [L:42]
  - Modifiers: public, abstract
  - Summary: m_vecPosition1
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IBaseToggle.Position2` [L:47]
  - Modifiers: public, abstract
  - Summary: m_vecPosition2
- `float Sharp.Shared.GameEntities.IBaseToggle.MoveDistance` [L:37]
  - Modifiers: public, abstract
  - Summary: m_flMoveDistance
- `float Sharp.Shared.GameEntities.IBaseToggle.Wait` [L:32]
  - Modifiers: public, abstract
  - Summary: m_flWait


### interface IBaseTrigger : Sharp.Shared.GameEntities.IBaseToggle

- FullName: `Sharp.Shared.GameEntities.IBaseTrigger`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseTrigger.cs:27
- Generated: false
- Attributes: `[NetClass("CBaseTrigger")]`

#### Properties
- `Sharp.Shared.GameEntities.IBaseFilter? Sharp.Shared.GameEntities.IBaseTrigger.FilterEntity` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: m_hFilter
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseFilter> Sharp.Shared.GameEntities.IBaseTrigger.FilterEntityHandle` [L:42]
  - Modifiers: public, abstract
  - Summary: m_hFilter
- `bool Sharp.Shared.GameEntities.IBaseTrigger.Disabled` [L:32]
  - Modifiers: public, abstract
  - Summary: m_bDisabled

#### Methods
- `Sharp.Shared.CStrike.ISchemaList<Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity>> Sharp.Shared.GameEntities.IBaseTrigger.GetTouchingEntities()` [L:47]
  - Modifiers: public, abstract
  - Summary: m_hTouchingEntities


### interface IBaseWeapon : Sharp.Shared.GameEntities.IEconEntity

- FullName: `Sharp.Shared.GameEntities.IBaseWeapon`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBaseWeapon.cs:29
- Generated: false
- Attributes: `[NetClass("CCSWeaponBase")]`

#### Properties
- `Sharp.Shared.Enums.CStrikeWeaponMode Sharp.Shared.GameEntities.IBaseWeapon.WeaponMode` [L:121]
  - Modifiers: public, abstract
  - Summary: m_weaponMode
- `Sharp.Shared.Enums.GearSlot Sharp.Shared.GameEntities.IBaseWeapon.Slot` [L:101]
  - Modifiers: public, abstract, readonly
  - Summary: Weapon slot (From VData)
- `Sharp.Shared.Enums.WeaponGameplayAnimState Sharp.Shared.GameEntities.IBaseWeapon.WeaponGameplayAnimState` [L:111]
  - Modifiers: public, abstract
  - Summary: m_iWeaponGameplayAnimState
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEntities.IBaseWeapon.PrevOwnerEntity` [L:106]
  - Modifiers: public, abstract, readonly
  - Summary: m_hPrevOwner
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IPlayerPawn> Sharp.Shared.GameEntities.IBaseWeapon.PrevOwnerEntityHandle` [L:126]
  - Modifiers: public, abstract
  - Summary: m_hPrevOwner
- `bool Sharp.Shared.GameEntities.IBaseWeapon.CanBePickedUp` [L:141]
  - Modifiers: public, abstract
  - Summary: m_bCanBePickedUp
- `bool Sharp.Shared.GameEntities.IBaseWeapon.InReload` [L:161]
  - Modifiers: public, abstract
  - Summary: m_bInReload
- `bool Sharp.Shared.GameEntities.IBaseWeapon.IsKnife` [L:34]
  - Modifiers: public, abstract, readonly
  - Summary: Check if it is knife
- `bool Sharp.Shared.GameEntities.IBaseWeapon.SilencerOn` [L:166]
  - Modifiers: public, abstract
  - Summary: m_bSilencerOn
- `float Sharp.Shared.GameEntities.IBaseWeapon.AccuracyPenalty` [L:146]
  - Modifiers: public, abstract
  - Summary: m_fAccuracyPenalty
- `float Sharp.Shared.GameEntities.IBaseWeapon.LastAccuracyUpdateTime` [L:151]
  - Modifiers: public, abstract
  - Summary: m_flLastAccuracyUpdateTime
- `float Sharp.Shared.GameEntities.IBaseWeapon.LastShotTime` [L:176]
  - Modifiers: public, abstract
  - Summary: m_fLastShotTime
- `float Sharp.Shared.GameEntities.IBaseWeapon.NextOwnerTouchTime` [L:131]
  - Modifiers: public, abstract
  - Summary: m_nextOwnerTouchTime
- `float Sharp.Shared.GameEntities.IBaseWeapon.NextPrevOwnerTouchTime` [L:136]
  - Modifiers: public, abstract
  - Summary: m_nextPrevOwnerTouchTime
- `float Sharp.Shared.GameEntities.IBaseWeapon.RecoilIndex` [L:156]
  - Modifiers: public, abstract
  - Summary: m_flRecoilIndex
- `float Sharp.Shared.GameEntities.IBaseWeapon.TimeSilencerSwitchComplete` [L:171]
  - Modifiers: public, abstract
  - Summary: m_flTimeSilencerSwitchComplete
- `float Sharp.Shared.GameEntities.IBaseWeapon.WeaponGameplayAnimStateTimestamp` [L:116]
  - Modifiers: public, abstract
  - Summary: m_flWeaponGameplayAnimStateTimestamp
- `int Sharp.Shared.GameEntities.IBaseWeapon.Clip` [L:80]
  - Modifiers: public, abstract
  - Summary: Weapon clip, -1 means it does not use Clip1, -2 when it is not a weapon If exceeds  limit, will be reset to  when firing
- `int Sharp.Shared.GameEntities.IBaseWeapon.MaxClip` [L:91]
  - Modifiers: public, abstract, readonly
  - Summary: Maximum bullets in magazine (from VData)
- `int Sharp.Shared.GameEntities.IBaseWeapon.NextPrimaryAttackTick` [L:69]
  - Modifiers: public, abstract
  - Summary: m_nNextPrimaryAttackTick
- `int Sharp.Shared.GameEntities.IBaseWeapon.NextSecondaryAttackTick` [L:74]
  - Modifiers: public, abstract
  - Summary: m_nNextSecondaryAttackTick
- `int Sharp.Shared.GameEntities.IBaseWeapon.PrimaryReserveAmmoMax` [L:96]
  - Modifiers: public, abstract, readonly
  - Summary: Max primary reserve ammo (From VData)
- `int Sharp.Shared.GameEntities.IBaseWeapon.ReserveAmmo` [L:86]
  - Modifiers: public, abstract
  - Summary: Weapon reserve ammunition. Returns -1 if ReserveAmmo1 is not used, -2 if not a gun If exceeds ReserveAmmo limit, will be reset to  when firing
- `ushort Sharp.Shared.GameEntities.IBaseWeapon.ItemDefinitionIndex` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: m_iItemDefinitionIndex

#### Methods
- `Sharp.Shared.GameObjects.IEconItemDefinition Sharp.Shared.GameEntities.IBaseWeapon.GetItemDefinition()` [L:59]
  - Modifiers: public, abstract
  - Summary: ItemDefinition
- `Sharp.Shared.GameObjects.IWeaponData Sharp.Shared.GameEntities.IBaseWeapon.GetWeaponData()` [L:64]
  - Modifiers: public, abstract
  - Summary: WeaponVData
- `string Sharp.Shared.GameEntities.IBaseWeapon.GetItemDefinitionName()` [L:53]
  - Modifiers: public, abstract
  - Summary: ItemDefinitionName
- `string Sharp.Shared.GameEntities.IBaseWeapon.GetWeaponClassname()` [L:47]
  - Modifiers: public, abstract
  - Summary: weapon classname
- `void Sharp.Shared.GameEntities.IBaseWeapon.Deploy()` [L:186]
  - Modifiers: public, abstract
  - Summary: Deploy
- `void Sharp.Shared.GameEntities.IBaseWeapon.Holster()` [L:181]
  - Modifiers: public, abstract
  - Summary: Holster


### interface IBreakableProp : Sharp.Shared.GameEntities.IBaseAnimGraph

- FullName: `Sharp.Shared.GameEntities.IBreakableProp`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IBreakableProp.cs:26
- Generated: false
- Attributes: `[NetClass("CBreakableProp")]`

#### Properties
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBreakableProp.BreakerEntity` [L:36]
  - Modifiers: public, abstract, readonly
  - Summary: m_hBreaker
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.GameEntities.IBreakableProp.LastAttackerEntity` [L:46]
  - Modifiers: public, abstract, readonly
  - Summary: m_hLastAttacker
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBreakableProp.BreakerEntityHandle` [L:41]
  - Modifiers: public, abstract, readonly
  - Summary: m_hBreaker
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IBreakableProp.LastAttackerEntityHandle` [L:51]
  - Modifiers: public, abstract, readonly
  - Summary: m_hLastAttacker
- `float Sharp.Shared.GameEntities.IBreakableProp.ExplodeDamage` [L:56]
  - Modifiers: public, abstract
  - Summary: m_explodeDamage
- `float Sharp.Shared.GameEntities.IBreakableProp.ExplodeRadius` [L:61]
  - Modifiers: public, abstract
  - Summary: m_explodeRadius
- `float Sharp.Shared.GameEntities.IBreakableProp.ExplosionDelay` [L:66]
  - Modifiers: public, abstract
  - Summary: m_explosionDelay
- `int Sharp.Shared.GameEntities.IBreakableProp.MinHealthDamage` [L:31]
  - Modifiers: public, abstract
  - Summary: m_iMinHealthDmg


### interface IEconEntity : Sharp.Shared.GameEntities.IBaseAnimGraph

- FullName: `Sharp.Shared.GameEntities.IEconEntity`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IEconEntity.cs:26
- Generated: false
- Attributes: `[NetClass("CEconEntity")]`

#### Properties
- `Sharp.Shared.GameObjects.IAttributeContainer Sharp.Shared.GameEntities.IEconEntity.AttributeContainer` [L:32]
  - Modifiers: public, abstract, readonly
  - Summary: Econ property You should retrieve this each time you use it rather than cached or stored for reuse


### interface IEntityFlame : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IEntityFlame`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IEntityFlame.cs:26
- Generated: false
- Attributes: `[NetClass("CEntityFlame")]`

#### Properties
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IEntityFlame.AttackerEntity` [L:36]
  - Modifiers: public, abstract
  - Summary: m_hAttacker
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.GameEntities.IEntityFlame.EntityAttached` [L:31]
  - Modifiers: public, abstract
  - Summary: m_hEntAttached
- `float Sharp.Shared.GameEntities.IEntityFlame.LifeTime` [L:41]
  - Modifiers: public, abstract
  - Summary: m_flLifetime
- `float Sharp.Shared.GameEntities.IEntityFlame.Size` [L:46]
  - Modifiers: public, abstract
  - Summary: m_flSize
- `int Sharp.Shared.GameEntities.IEntityFlame.CustomDamageType` [L:51]
  - Modifiers: public, abstract
  - Summary: m_iCustomDamageType


### interface IMathCounter : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IMathCounter`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IMathCounter.cs:25
- Generated: false
- Attributes: `[NetClass("CMathCounter")]`

#### Properties
- `bool Sharp.Shared.GameEntities.IMathCounter.Disabled` [L:33]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameEntities.IMathCounter.MaxValue` [L:29]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameEntities.IMathCounter.MinValue` [L:27]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameEntities.IMathCounter.Value` [L:31]
  - Modifiers: public, abstract


### interface IObserverPawn : Sharp.Shared.GameEntities.IBasePlayerPawn

- FullName: `Sharp.Shared.GameEntities.IObserverPawn`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IObserverPawn.cs:26
- Generated: false
- Attributes: `[NetClass("CCSObserverPawn")]`

#### Methods
- `Sharp.Shared.GameObjects.IObserverService? Sharp.Shared.GameEntities.IObserverPawn.GetObserverService()` [L:31]
  - Modifiers: public, abstract
  - Summary: ObserverService instance


### interface IParticleGlow : Sharp.Shared.GameEntities.IBaseParticle

- FullName: `Sharp.Shared.GameEntities.IParticleGlow`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IParticleGlow.cs:26
- Generated: false
- Attributes: `[NetClass("CEnvParticleGlow")]`

#### Properties
- `Sharp.Shared.Types.Color32 Sharp.Shared.GameEntities.IParticleGlow.ColorTint` [L:46]
  - Modifiers: public, abstract
  - Summary: m_ColorTint
- `float Sharp.Shared.GameEntities.IParticleGlow.AlphaScale` [L:31]
  - Modifiers: public, abstract
  - Summary: m_flAlphaScale
- `float Sharp.Shared.GameEntities.IParticleGlow.RadiusScale` [L:36]
  - Modifiers: public, abstract
  - Summary: m_flRadiusScale
- `float Sharp.Shared.GameEntities.IParticleGlow.SelfIllumScale` [L:41]
  - Modifiers: public, abstract
  - Summary: m_flSelfIllumScale


### interface IPlayerController : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IPlayerController`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IPlayerController.cs:31
- Generated: false
- Attributes: `[NetClass("CCSPlayerController")]`

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEntities.IPlayerController.PendingTeamNum` [L:236]
  - Modifiers: public, abstract
  - Summary: m_iPendingTeamNum
- `Sharp.Shared.Enums.CompetitiveRankType Sharp.Shared.GameEntities.IPlayerController.CompetitiveRankType` [L:196]
  - Modifiers: public, abstract
  - Summary: m_iCompetitiveRankType
- `Sharp.Shared.Enums.PlayerConnectedState Sharp.Shared.GameEntities.IPlayerController.ConnectedState` [L:211]
  - Modifiers: public, abstract, readonly
  - Summary: Connection state
- `Sharp.Shared.Units.PlayerSlot Sharp.Shared.GameEntities.IPlayerController.PlayerSlot` [L:132]
  - Modifiers: public, abstract, readonly
  - Summary: PlayerSlot
- `Sharp.Shared.Units.SteamID Sharp.Shared.GameEntities.IPlayerController.SteamId` [L:127]
  - Modifiers: public, abstract, readonly
  - Summary: Returns a SteamID64 (7656119xxxxxxxxxx)
- `bool Sharp.Shared.GameEntities.IPlayerController.ControllingBot` [L:241]
  - Modifiers: public, abstract
  - Summary: m_bControllingBot
- `bool Sharp.Shared.GameEntities.IPlayerController.HasCommunicationAbuseMute` [L:231]
  - Modifiers: public, abstract
  - Summary: m_bHasCommunicationAbuseMute
- `bool Sharp.Shared.GameEntities.IPlayerController.IsFakeClient` [L:166]
  - Modifiers: public, virtual, readonly
  - Summary: Is this controller for FakeClient(Bots)
- `bool Sharp.Shared.GameEntities.IPlayerController.IsHltv` [L:161]
  - Modifiers: public, abstract, readonly
  - Summary: Is controller in HLTV
- `bool Sharp.Shared.GameEntities.IPlayerController.RemoveAllItemsOnNextRoundReset` [L:221]
  - Modifiers: public, abstract
  - Summary: m_bRemoveAllItemsOnNextRoundReset
- `bool Sharp.Shared.GameEntities.IPlayerController.SwitchTeamsOnNextRoundReset` [L:216]
  - Modifiers: public, abstract
  - Summary: Will the player switch team when a new round starts
- `float Sharp.Shared.GameEntities.IPlayerController.LaggedMovement` [L:186]
  - Modifiers: public, abstract
  - Summary: m_flLaggedMovementValue in source1
- `int Sharp.Shared.GameEntities.IPlayerController.CompetitiveRanking` [L:191]
  - Modifiers: public, abstract
  - Summary: m_iCompetitiveRanking
- `int Sharp.Shared.GameEntities.IPlayerController.CompetitiveWins` [L:201]
  - Modifiers: public, abstract
  - Summary: m_iCompetitiveWins
- `int Sharp.Shared.GameEntities.IPlayerController.DesiredObserverMode` [L:226]
  - Modifiers: public, abstract
  - Summary: Desired observer mode
- `int Sharp.Shared.GameEntities.IPlayerController.MvpCount` [L:176]
  - Modifiers: public, abstract
  - Summary: MVP on scoreboard
- `int Sharp.Shared.GameEntities.IPlayerController.RoundsWon` [L:246]
  - Modifiers: public, abstract
  - Summary: m_iRoundsWon
- `int Sharp.Shared.GameEntities.IPlayerController.Score` [L:171]
  - Modifiers: public, abstract
  - Summary: Score on scoreboard
- `int Sharp.Shared.GameEntities.IPlayerController.UpdaterCount` [L:181]
  - Modifiers: public, abstract
  - Summary: Scoreboard update count
- `string Sharp.Shared.GameEntities.IPlayerController.ClanTag` [L:137]
  - Modifiers: public, abstract, readonly
  - Summary: Clantag
- `string Sharp.Shared.GameEntities.IPlayerController.PlayerName` [L:142]
  - Modifiers: public, abstract
  - Summary: PlayerName, setting the value does not call StateChanged
- `uint Sharp.Shared.GameEntities.IPlayerController.DesiredFOV` [L:206]
  - Modifiers: public, abstract
  - Summary: m_iDesiredFOV

#### Methods
- `Sharp.Shared.GameEntities.IBasePlayerPawn? Sharp.Shared.GameEntities.IPlayerController.GetPawn()` [L:39]
  - Modifiers: public, abstract
  - Summary: Gets the PlayerPawn for this Controller
- `Sharp.Shared.GameEntities.IObserverPawn? Sharp.Shared.GameEntities.IPlayerController.GetObserverPawn()` [L:55]
  - Modifiers: public, abstract
  - Summary: Gets the ObserverPawn for this Controller
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEntities.IPlayerController.GetPlayerPawn()` [L:47]
  - Modifiers: public, abstract
  - Summary: Gets the PlayerPawn for this Controller
- `Sharp.Shared.GameObjects.IControllerActionTrackingService? Sharp.Shared.GameEntities.IPlayerController.GetActionTrackingService()` [L:266]
  - Modifiers: public, abstract
  - Summary: ActionTrackingService
- `Sharp.Shared.GameObjects.IDamageService? Sharp.Shared.GameEntities.IPlayerController.GetDamageService()` [L:251]
  - Modifiers: public, abstract
  - Summary: DamageService
- `Sharp.Shared.GameObjects.IEconItemView? Sharp.Shared.GameEntities.IPlayerController.GetItemInLoadoutFromInventory(Sharp.Shared.Enums.CStrikeTeam team, int slot)` [L:278]
  - Modifiers: public, abstract
  - Summary: Gets the equipped inventory item from loadout
- `Sharp.Shared.GameObjects.IInGameMoneyService? Sharp.Shared.GameEntities.IPlayerController.GetInGameMoneyService()` [L:256]
  - Modifiers: public, abstract
  - Summary: MoneyService
- `Sharp.Shared.GameObjects.IInventoryService? Sharp.Shared.GameEntities.IPlayerController.GetInventoryService()` [L:261]
  - Modifiers: public, abstract
  - Summary: InventoryService
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.GameEntities.IPlayerController.GetGameClient()` [L:67]
  - Modifiers: public, abstract
  - Summary: Gets the Returns null if the player is not in-game, even if the entity exists
- `Sharp.Shared.Types.SoundOpEventGuid Sharp.Shared.GameEntities.IPlayerController.EmitSoundClient(string sound, [float? volume = null])` [L:273]
  - Modifiers: public, abstract
  - Summary: Play a soundevent only for this player
- `bool Sharp.Shared.GameEntities.IPlayerController.IsConnected()` [L:115]
  - Modifiers: public, virtual
  - Summary: Is the player connected
- `bool Sharp.Shared.GameEntities.IPlayerController.IsDisconnecting()` [L:121]
  - Modifiers: public, virtual
  - Summary: Is the player disconnecting
- `void Sharp.Shared.GameEntities.IPlayerController.CheckPawn()` [L:105]
  - Modifiers: public, abstract
  - Summary: Check awn
- `void Sharp.Shared.GameEntities.IPlayerController.Print(Sharp.Shared.Enums.HudPrintChannel channel, string message, [string? param1 = null], [string? param2 = null], [string? param3 = null], [string? param4 = null])` [L:72]
  - Modifiers: public, abstract
  - Summary: Print message to this player
- `void Sharp.Shared.GameEntities.IPlayerController.PrintCenterHtml(string message, [int duration = 1])` [L:85]
  - Modifiers: public, abstract
  - Summary: Print a hud message with limited html format support to this player.
- `void Sharp.Shared.GameEntities.IPlayerController.Respawn()` [L:95]
  - Modifiers: public, abstract
  - Summary: Respawn player
- `void Sharp.Shared.GameEntities.IPlayerController.SetClanTag(string tag)` [L:100]
  - Modifiers: public, abstract
  - Summary: Set clantag
- `void Sharp.Shared.GameEntities.IPlayerController.SetPawn(Sharp.Shared.GameEntities.IBasePlayerPawn pawn, bool unknown1, bool unknown2, bool unknown3, bool unknown4)` [L:110]
  - Modifiers: public, abstract
  - Summary: Set PlayerPawn
- `void Sharp.Shared.GameEntities.IPlayerController.SetPlayerPawn(Sharp.Shared.GameEntities.IPlayerPawn pawn)` [L:61]
  - Modifiers: public, abstract
  - Summary: Sets the PlayerPawn You should know what you're doing before calling this
- `void Sharp.Shared.GameEntities.IPlayerController.SwitchTeam(Sharp.Shared.Enums.CStrikeTeam team)` [L:90]
  - Modifiers: public, abstract
  - Summary: Change team without slaying

#### Obsolete Members
- `bool Sharp.Shared.GameEntities.IPlayerController.IsPawnAlive` [L:149] — Use GetPawn().IsAlive, will be removed in 2.2
- `uint Sharp.Shared.GameEntities.IPlayerController.PawnHealth` [L:156] — Use GetPawn().Health, will be removed in 2.2


### interface IPlayerPawn : Sharp.Shared.GameEntities.IBasePlayerPawn

- FullName: `Sharp.Shared.GameEntities.IPlayerPawn`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IPlayerPawn.cs:28
- Generated: false
- Attributes: `[NetClass("CCSPlayerPawn")]`

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.GameEntities.IPlayerPawn.TotalBulletForce` [L:245]
  - Modifiers: public, abstract
  - Summary: m_vecTotalBulletForce
- `bool Sharp.Shared.GameEntities.IPlayerPawn.InBombZone` [L:225]
  - Modifiers: public, abstract, readonly
  - Summary: m_bInBombZone
- `bool Sharp.Shared.GameEntities.IPlayerPawn.InBuyZone` [L:215]
  - Modifiers: public, abstract, readonly
  - Summary: m_bInBuyZone
- `bool Sharp.Shared.GameEntities.IPlayerPawn.InHostageRescueZone` [L:220]
  - Modifiers: public, abstract, readonly
  - Summary: m_bInHostageRescueZone
- `bool Sharp.Shared.GameEntities.IPlayerPawn.IsBuyMenuOpen` [L:230]
  - Modifiers: public, abstract, readonly
  - Summary: m_bIsBuyMenuOpen
- `bool Sharp.Shared.GameEntities.IPlayerPawn.LeftHanded` [L:235]
  - Modifiers: public, abstract, readonly
  - Summary: m_bLeftHanded
- `bool Sharp.Shared.GameEntities.IPlayerPawn.WaitForNoAttack` [L:255]
  - Modifiers: public, abstract
  - Summary: m_bWaitForNoAttack
- `float Sharp.Shared.GameEntities.IPlayerPawn.FlinchStack` [L:210]
  - Modifiers: public, abstract
  - Summary: m_flFlinchStack
- `float Sharp.Shared.GameEntities.IPlayerPawn.HealthShotBoostExpirationTime` [L:195]
  - Modifiers: public, abstract
  - Summary: m_flHealthShotBoostExpirationTime
- `float Sharp.Shared.GameEntities.IPlayerPawn.MolotovDamageTime` [L:190]
  - Modifiers: public, abstract
  - Summary: m_fMolotovDamageTime
- `float Sharp.Shared.GameEntities.IPlayerPawn.SwitchedHandednessTime` [L:240]
  - Modifiers: public, abstract
  - Summary: m_fSwitchedHandednessTime
- `float Sharp.Shared.GameEntities.IPlayerPawn.VelocityModifier` [L:200]
  - Modifiers: public, abstract
  - Summary: m_flVelocityModifier
- `int Sharp.Shared.GameEntities.IPlayerPawn.ArmorValue` [L:185]
  - Modifiers: public, abstract
  - Summary: Armor value
- `int Sharp.Shared.GameEntities.IPlayerPawn.DeathFlags` [L:250]
  - Modifiers: public, abstract
  - Summary: m_iDeathFlags
- `int Sharp.Shared.GameEntities.IPlayerPawn.ShotsFired` [L:205]
  - Modifiers: public, abstract
  - Summary: m_iShotsFired

#### Methods
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameEntities.IPlayerPawn.GetActiveWeapon()` [L:55]
  - Modifiers: public, abstract
  - Summary: Gets the currently held weapon
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameEntities.IPlayerPawn.GetWeaponBySlot(Sharp.Shared.Enums.GearSlot slot, [int position = -1])` [L:60]
  - Modifiers: public, abstract
  - Summary: Gets weapon from inventory by slot
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameEntities.IPlayerPawn.GiveNamedItem(Sharp.Shared.Enums.EconItemId item)` [L:49]
  - Modifiers: public, abstract
  - Summary: Give weapon to player
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.GameEntities.IPlayerPawn.GiveNamedItem(string weapon)` [L:44]
  - Modifiers: public, abstract
  - Summary: Give weapon to player
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEntities.IPlayerPawn.GetControllerAuto()` [L:39]
  - Modifiers: public, abstract
  - Summary: Automatically gets Controller if alive, otherwise OriginalController
- `Sharp.Shared.GameObjects.IAimPunchService? Sharp.Shared.GameEntities.IPlayerPawn.GetAimPunchService()` [L:175]
  - Modifiers: public, abstract
  - Summary: AimPunchService
- `Sharp.Shared.GameObjects.IBulletService? Sharp.Shared.GameEntities.IPlayerPawn.GetBulletService()` [L:145]
  - Modifiers: public, abstract
  - Summary: BulletService
- `Sharp.Shared.GameObjects.IBuyService? Sharp.Shared.GameEntities.IPlayerPawn.GetBuyService()` [L:155]
  - Modifiers: public, abstract
  - Summary: BuyService
- `Sharp.Shared.GameObjects.IDamageReactService? Sharp.Shared.GameEntities.IPlayerPawn.GetDamageReactService()` [L:170]
  - Modifiers: public, abstract
  - Summary: DamageReactService
- `Sharp.Shared.GameObjects.IEconItemView Sharp.Shared.GameEntities.IPlayerPawn.GetEconGloves()` [L:180]
  - Modifiers: public, abstract
  - Summary: Glove Econ
- `Sharp.Shared.GameObjects.IHostageService? Sharp.Shared.GameEntities.IPlayerPawn.GetHostageService()` [L:150]
  - Modifiers: public, abstract
  - Summary: HostageService
- `Sharp.Shared.GameObjects.IItemService? Sharp.Shared.GameEntities.IPlayerPawn.GetItemService()` [L:115]
  - Modifiers: public, abstract
  - Summary: ItemService
- `Sharp.Shared.GameObjects.IPingService? Sharp.Shared.GameEntities.IPlayerPawn.GetPingService()` [L:135]
  - Modifiers: public, abstract
  - Summary: PingServices
- `Sharp.Shared.GameObjects.IPlayerActionTrackingService? Sharp.Shared.GameEntities.IPlayerPawn.GetActionTrackingService()` [L:160]
  - Modifiers: public, abstract
  - Summary: ActionTrackingService
- `Sharp.Shared.GameObjects.IPlayerMovementService? Sharp.Shared.GameEntities.IPlayerPawn.GetPlayerMovementService()` [L:125]
  - Modifiers: public, abstract
  - Summary: PlayerMoveService
- `Sharp.Shared.GameObjects.IPlayerUseService? Sharp.Shared.GameEntities.IPlayerPawn.GetPlayerUseService()` [L:130]
  - Modifiers: public, abstract
  - Summary: PlayerUseService
- `Sharp.Shared.GameObjects.IRadioService? Sharp.Shared.GameEntities.IPlayerPawn.GetRadioService()` [L:165]
  - Modifiers: public, abstract
  - Summary: RadioService
- `Sharp.Shared.GameObjects.IWaterService? Sharp.Shared.GameEntities.IPlayerPawn.GetWaterService()` [L:140]
  - Modifiers: public, abstract
  - Summary: WaterService
- `Sharp.Shared.GameObjects.IWeaponService? Sharp.Shared.GameEntities.IPlayerPawn.GetWeaponService()` [L:120]
  - Modifiers: public, abstract
  - Summary: WeaponService
- `bool Sharp.Shared.GameEntities.IPlayerPawn.DetachWeapon(Sharp.Shared.GameEntities.IBaseWeapon item)` [L:90]
  - Modifiers: public, abstract
  - Summary: Detach weapon from player
- `bool Sharp.Shared.GameEntities.IPlayerPawn.SelectItem(Sharp.Shared.GameEntities.IBaseWeapon item)` [L:85]
  - Modifiers: public, abstract
  - Summary: Switch to weapon/item
- `void Sharp.Shared.GameEntities.IPlayerPawn.DropWeapon(Sharp.Shared.GameEntities.IBaseWeapon item)` [L:80]
  - Modifiers: public, abstract
  - Summary: Force drop weapon
- `void Sharp.Shared.GameEntities.IPlayerPawn.GiveGloves(Sharp.Shared.Enums.EconGlovesId id, int prefab, float wear, int seed)` [L:105]
  - Modifiers: public, abstract
  - Summary: Give gloves to player
- `void Sharp.Shared.GameEntities.IPlayerPawn.GiveGloves(int itemDefIndex, int prefab, float wear, int seed)` [L:100]
  - Modifiers: public, abstract
  - Summary: Give gloves to player
- `void Sharp.Shared.GameEntities.IPlayerPawn.RemoveAllItems([bool removeSuit = false])` [L:75]
  - Modifiers: public, abstract
  - Summary: Remove all items
- `void Sharp.Shared.GameEntities.IPlayerPawn.RemovePlayerItem(Sharp.Shared.GameEntities.IBaseWeapon item)` [L:69]
  - Modifiers: public, abstract
  - Summary: Remove weapon and destroy it immediately
- `void Sharp.Shared.GameEntities.IPlayerPawn.Slay([bool explode = false])` [L:33]
  - Modifiers: public, abstract
  - Summary: Slay
- `void Sharp.Shared.GameEntities.IPlayerPawn.SwitchWeapon(Sharp.Shared.GameEntities.IBaseWeapon? weapon)` [L:95]
  - Modifiers: public, abstract
  - Summary: Force switch weapon or go empty-handed (bypasses all checks/conditions)
- `void Sharp.Shared.GameEntities.IPlayerPawn.TransientChangeVelocityModifier(float velocityModifier)` [L:110]
  - Modifiers: public, abstract
  - Summary: Change VelocityModifier without calling StateChanged, player won't receive new value


### interface IVoteController : Sharp.Shared.GameEntities.IBaseEntity

- FullName: `Sharp.Shared.GameEntities.IVoteController`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IVoteController.cs:26
- Generated: false
- Attributes: `[NetClass("CVoteController")]`

#### Properties
- `bool Sharp.Shared.GameEntities.IVoteController.IsYesNoVote` [L:46]
  - Modifiers: public, abstract
  - Summary: m_bIsYesNoVote
- `int Sharp.Shared.GameEntities.IVoteController.OnlyTeamToVote` [L:31]
  - Modifiers: public, abstract
  - Summary: m_iOnlyTeamToVote
- `int Sharp.Shared.GameEntities.IVoteController.PotentialVotes` [L:41]
  - Modifiers: public, abstract
  - Summary: m_nPotentialVotes

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<int> Sharp.Shared.GameEntities.IVoteController.GetVoteOptionCount()` [L:36]
  - Modifiers: public, abstract
  - Summary: m_nVoteOptionCount
- `Sharp.Shared.CStrike.ISchemaArray<int> Sharp.Shared.GameEntities.IVoteController.GetVotesCast()` [L:51]
  - Modifiers: public, abstract
  - Summary: m_nVotesCast


### interface IWorldText : Sharp.Shared.GameEntities.IBaseModelEntity

- FullName: `Sharp.Shared.GameEntities.IWorldText`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEntities/IWorldText.cs:26
- Generated: false
- Attributes: `[NetClass("CPointWorldText")]`

#### Properties
- `Sharp.Shared.Types.Color32 Sharp.Shared.GameEntities.IWorldText.Color` [L:31]
  - Modifiers: public, abstract
  - Summary: m_Color
- `bool Sharp.Shared.GameEntities.IWorldText.DrawBackground` [L:56]
  - Modifiers: public, abstract
  - Summary: m_bDrawBackground
- `bool Sharp.Shared.GameEntities.IWorldText.Enabled` [L:46]
  - Modifiers: public, abstract
  - Summary: m_bEnabled
- `bool Sharp.Shared.GameEntities.IWorldText.FullBright` [L:51]
  - Modifiers: public, abstract
  - Summary: m_bFullbright
- `float Sharp.Shared.GameEntities.IWorldText.BackgroundBorderHeight` [L:71]
  - Modifiers: public, abstract
  - Summary: m_flBackgroundBorderHeight
- `float Sharp.Shared.GameEntities.IWorldText.BackgroundBorderWidth` [L:66]
  - Modifiers: public, abstract
  - Summary: m_flBackgroundBorderWidth
- `float Sharp.Shared.GameEntities.IWorldText.BackgroundWorldToUV` [L:76]
  - Modifiers: public, abstract
  - Summary: m_flBackgroundWorldToUV
- `float Sharp.Shared.GameEntities.IWorldText.FontSize` [L:41]
  - Modifiers: public, abstract
  - Summary: m_flFontSize
- `string Sharp.Shared.GameEntities.IWorldText.BackgroundMaterialName` [L:61]
  - Modifiers: public, abstract
  - Summary: m_BackgroundMaterialName
- `string Sharp.Shared.GameEntities.IWorldText.Message` [L:36]
  - Modifiers: public, abstract
  - Summary: m_messageText


