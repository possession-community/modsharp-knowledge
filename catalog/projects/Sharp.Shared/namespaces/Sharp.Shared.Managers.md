# Sharp.Shared.Managers

Project: Sharp.Shared
Types: 20 (0 generated)

### interface IClientManager

- FullName: `Sharp.Shared.Managers.IClientManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/ClientManager.cs:30
- Generated: false

#### Methods
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Managers.IClientManager.GetGameClient(Sharp.Shared.Units.PlayerSlot slot)` [L:69]
  - Modifiers: public, abstract
  - Summary: Find an  by Slot
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Managers.IClientManager.GetGameClient(Sharp.Shared.Units.SteamID steamId)` [L:79]
  - Modifiers: public, abstract
  - Summary: Find an  by SteamId
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Managers.IClientManager.GetGameClient(Sharp.Shared.Units.UserID userId)` [L:74]
  - Modifiers: public, abstract
  - Summary: Find an  by UserId
- `System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Shared.Managers.IClientManager.GetGameClients([bool inGame = false])` [L:84]
  - Modifiers: public, abstract
  - Summary: Get connected s
- `System.Collections.Generic.List<Sharp.Shared.Objects.IGameClient> Sharp.Shared.Managers.IClientManager.GetGameClientList([bool inGame = false])` [L:89]
  - Modifiers: public, abstract
  - Summary: Get connected s
- `int Sharp.Shared.Managers.IClientManager.GetClientCount([bool inGame = false])` [L:94]
  - Modifiers: public, abstract
  - Summary: Get the number of s in the client pool
- `int Sharp.Shared.Managers.IClientManager.QueryConVar(Sharp.Shared.Objects.IGameClient client, string name, System.Action<Sharp.Shared.Objects.IGameClient, Sharp.Shared.Enums.QueryConVarValueStatus, string, string> callback)` [L:124]
  - Modifiers: public, abstract
  - Summary: Query the value of a given cvar from the client
- `void Sharp.Shared.Managers.IClientManager.InstallClientListener(Sharp.Shared.Listeners.IClientListener listener)` [L:37]
  - Modifiers: public, abstract
  - Summary: Add  to listen for events
- `void Sharp.Shared.Managers.IClientManager.InstallCommandCallback(string command, Sharp.Shared.Managers.IClientManager.DelegateClientCommand callback)` [L:48]
  - Modifiers: public, abstract
  - Summary: Listen for StringCommand (Virtual Command) sent by
- `void Sharp.Shared.Managers.IClientManager.InstallCommandListener(string command, Sharp.Shared.Managers.IClientManager.DelegateClientCommand callback)` [L:59]
  - Modifiers: public, abstract
  - Summary: Listen for ConCommand sent by
- `void Sharp.Shared.Managers.IClientManager.KickClient(Sharp.Shared.Objects.IGameClient client, string internalReason, [Sharp.Shared.Enums.NetworkDisconnectionReason msgId = Sharp.Shared.Enums.NetworkDisconnectionReason.Invalid])` [L:104]
  - Modifiers: public, abstract
  - Summary: Immediately kick a player from the game
- `void Sharp.Shared.Managers.IClientManager.PrintCenterHtmlToAll(string message, [int duration = 1])` [L:129]
  - Modifiers: public, abstract
  - Summary: Send center HTML message to all players
- `void Sharp.Shared.Managers.IClientManager.PrintCenterHtmlToClients(System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> clients, string message, [int duration = 1])` [L:134]
  - Modifiers: public, abstract
  - Summary: Send center HTML message to multiple players
- `void Sharp.Shared.Managers.IClientManager.RemoveClientListener(Sharp.Shared.Listeners.IClientListener listener)` [L:42]
  - Modifiers: public, abstract
  - Summary: Remove
- `void Sharp.Shared.Managers.IClientManager.RemoveCommandCallback(string command, Sharp.Shared.Managers.IClientManager.DelegateClientCommand callback)` [L:54]
  - Modifiers: public, abstract
  - Summary: Remove listener for StringCommand (Virtual Command) sent by
- `void Sharp.Shared.Managers.IClientManager.RemoveCommandListener(string command, Sharp.Shared.Managers.IClientManager.DelegateClientCommand callback)` [L:64]
  - Modifiers: public, abstract
  - Summary: Remove listener for ConCommand sent by

#### Obsolete Members
- `Sharp.Shared.Objects.IAdmin Sharp.Shared.Managers.IClientManager.CreateAdmin(Sharp.Shared.Units.SteamID identity, string name, [byte immunity = 0])` [L:158] — Migrated to AdminManager. Will be removed at 2.2
- `Sharp.Shared.Objects.IAdmin? Sharp.Shared.Managers.IClientManager.FindAdmin(Sharp.Shared.Units.SteamID identity)` [L:146] — Migrated to AdminManager. Will be removed at 2.2
- `Sharp.Shared.Objects.IAdmin? Sharp.Shared.Managers.IClientManager.FindAdmin(string name)` [L:152] — Migrated to AdminManager. Will be removed at 2.2
- `System.Collections.Generic.IReadOnlyCollection<Sharp.Shared.Objects.IAdmin> Sharp.Shared.Managers.IClientManager.GetAdmins()` [L:171] — Migrated to AdminManager. Will be removed at 2.2
- `void Sharp.Shared.Managers.IClientManager.DeleteAdmin(Sharp.Shared.Objects.IAdmin admin)` [L:164] — Migrated to AdminManager. Will be removed at 2.2
- `void Sharp.Shared.Managers.IClientManager.ReloadAdmins()` [L:140] — Migrated to AdminManager. Will be removed at 2.2


### delegate DelegateClientCommand : System.MulticastDelegate

- FullName: `Sharp.Shared.Managers.IClientManager.DelegateClientCommand`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Shared/Managers/ClientManager.cs:32
- Generated: false
- Invoke: `virtual Sharp.Shared.Enums.ECommandAction Sharp.Shared.Managers.IClientManager.DelegateClientCommand.Invoke(Sharp.Shared.Objects.IGameClient client, Sharp.Shared.Types.StringCommand command)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateClientCommand**


### interface IConVarManager

- FullName: `Sharp.Shared.Managers.IConVarManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/ConVarManager.cs:27
- Generated: false

#### Methods
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, bool defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:53]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, float defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:130]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, float defaultValue, float min, float max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:135]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, int defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:89]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, int defaultValue, int min, int max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:82]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, long defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:113]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, long defaultValue, long min, long max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:106]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, short defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:65]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, short defaultValue, short min, short max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:58]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, string defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:142]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, uint defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:101]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, uint defaultValue, uint min, uint max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:94]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, ulong defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:125]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, ulong defaultValue, ulong min, ulong max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:118]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, ushort defaultValue, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:77]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.CreateConVar(string name, ushort defaultValue, ushort min, ushort max, [string? helpString = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:70]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IConVar? Sharp.Shared.Managers.IConVarManager.FindConVar(string name, [bool useIterator = false])` [L:40]
  - Modifiers: public, abstract
  - Summary: Search for an existing ConVar
- `bool Sharp.Shared.Managers.IConVarManager.ReleaseCommand(string name)` [L:172]
  - Modifiers: public, abstract
  - Summary: Must be called during unload, otherwise leak occurs
- `void Sharp.Shared.Managers.IConVarManager.CreateConsoleCommand(string name, System.Func<Sharp.Shared.Objects.IGameClient?, Sharp.Shared.Types.StringCommand, Sharp.Shared.Enums.ECommandAction> fn, [string? description = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:156]
  - Modifiers: public, abstract
  - Summary: Create a console command that can be used by both client and server. If you want to create
- `void Sharp.Shared.Managers.IConVarManager.CreateServerCommand(string name, System.Func<Sharp.Shared.Types.StringCommand, Sharp.Shared.Enums.ECommandAction> fn, [string? description = null], [Sharp.Shared.Enums.ConVarFlags? flags = null])` [L:164]
  - Modifiers: public, abstract
  - Summary: Create a server only command
- `void Sharp.Shared.Managers.IConVarManager.InstallChangeHook(Sharp.Shared.Objects.IConVar conVar, Sharp.Shared.Managers.IConVarManager.DelegateConVarChange callback)` [L:46]
  - Modifiers: public, abstract
  - Summary: Listen for changes to a ConVar value Modifying values within the Callback will immediately cause StackOverflow
- `void Sharp.Shared.Managers.IConVarManager.RemoveChangeHook(Sharp.Shared.Objects.IConVar conVar, Sharp.Shared.Managers.IConVarManager.DelegateConVarChange callback)` [L:51]
  - Modifiers: public, abstract
  - Summary: Remove ConVar listener


### delegate DelegateConVarChange : System.MulticastDelegate

- FullName: `Sharp.Shared.Managers.IConVarManager.DelegateConVarChange`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Shared/Managers/ConVarManager.cs:33
- Generated: false
- Summary: Callback called when ConVar value changes Modifying values within the Callback will cause StackOverflow
- Invoke: `virtual void Sharp.Shared.Managers.IConVarManager.DelegateConVarChange.Invoke(Sharp.Shared.Objects.IConVar conVar)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateConVarChange**


### interface IEconItemManager

- FullName: `Sharp.Shared.Managers.IEconItemManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/EconItemManager.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.GameObjects.IEconItemDefinition? Sharp.Shared.Managers.IEconItemManager.GetEconItemDefinitionByIndex(Sharp.Shared.Enums.EconItemId index)` [L:46]
  - Modifiers: public, abstract
  - Summary: Get EconItemDefinition by index
- `Sharp.Shared.GameObjects.IEconItemDefinition? Sharp.Shared.Managers.IEconItemManager.GetEconItemDefinitionByIndex(ushort index)` [L:41]
  - Modifiers: public, abstract
  - Summary: Get EconItemDefinition by index
- `Sharp.Shared.GameObjects.IEconItemDefinition? Sharp.Shared.Managers.IEconItemManager.GetEconItemDefinitionByName(string name)` [L:51]
  - Modifiers: public, abstract
  - Summary: Get EconItemDefinition by name
- `System.Collections.Frozen.FrozenDictionary<uint, Sharp.Shared.GameObjects.IPaintKit> Sharp.Shared.Managers.IEconItemManager.GetPaintKits()` [L:36]
  - Modifiers: public, abstract
  - Summary: Get dictionary of all PaintKits
- `System.Collections.Frozen.FrozenDictionary<ushort, Sharp.Shared.GameObjects.IEconItemDefinition> Sharp.Shared.Managers.IEconItemManager.GetEconItems()` [L:31]
  - Modifiers: public, abstract
  - Summary: Get dictionary of all EconItems


### interface IEntityManager

- FullName: `Sharp.Shared.Managers.IEntityManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/EntityManager.cs:30
- Generated: false

#### Methods
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.CreateEntityByName(string classname)` [L:156]
  - Modifiers: public, abstract
  - Summary: Create an entity instance without spawning it. You must call
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.FindEntityByClassname(Sharp.Shared.GameEntities.IBaseEntity? start, string classname)` [L:86]
  - Modifiers: public, abstract
  - Summary: Find entity by Classname.
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.FindEntityByIndex(Sharp.Shared.Units.EntityIndex index)` [L:50]
  - Modifiers: public, abstract
  - Summary: Find entity by Index
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.FindEntityByName(Sharp.Shared.GameEntities.IBaseEntity? start, string name)` [L:111]
  - Modifiers: public, abstract
  - Summary: Find entity by Targetname.
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.FindEntityInSphere(Sharp.Shared.GameEntities.IBaseEntity? start, Sharp.Shared.Types.Vector center, float radius)` [L:119]
  - Modifiers: public, abstract
  - Summary: Find entity by center coordinates
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Managers.IEntityManager.SpawnEntitySync(string classname, System.Collections.Generic.IReadOnlyDictionary<string, Sharp.Shared.Types.KeyValuesVariantValueItem> keyValues)` [L:134]
  - Modifiers: public, abstract
  - Summary: Create and spawn entity (full pipeline: create + precache + dispatch spawn).
- `Sharp.Shared.GameEntities.IBasePlayerPawn? Sharp.Shared.Managers.IEntityManager.FindPlayerPawnBySlot(Sharp.Shared.Units.PlayerSlot slot)` [L:186]
  - Modifiers: public, abstract
  - Summary: Find PlayerPawn by PlayerSlot
- `Sharp.Shared.GameEntities.IBaseTeam? Sharp.Shared.Managers.IEntityManager.GetGlobalCStrikeTeam(Sharp.Shared.Enums.CStrikeTeam team)` [L:226]
  - Modifiers: public, abstract
  - Summary: Get CCSTeam
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.Managers.IEntityManager.FindPlayerControllerBySlot(Sharp.Shared.Units.PlayerSlot slot)` [L:191]
  - Modifiers: public, abstract
  - Summary: Find PlayerController by PlayerSlot
- `Sharp.Shared.Types.Tier.CUtlSymbolLarge Sharp.Shared.Managers.IEntityManager.AllocPooledString(string content)` [L:169]
  - Modifiers: public, abstract
  - Summary: Create persistent CString in game
- `System.Collections.Generic.IEnumerable<Sharp.Shared.GameEntities.IPlayerController> Sharp.Shared.Managers.IEntityManager.GetPlayerControllers([bool inGame = true])` [L:197]
  - Modifiers: public, abstract
  - Summary: Find all existing PlayerControllers
- `System.Collections.Generic.List<Sharp.Shared.GameEntities.IPlayerController> Sharp.Shared.Managers.IEntityManager.FindPlayerControllers([bool inGame = true])` [L:203]
  - Modifiers: public, abstract
  - Summary: List all existing PlayerControllers
- `T Sharp.Shared.Managers.IEntityManager.MakeEntityFromPointer<T>(nint entity) where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:61]
  - Modifiers: public, abstract
  - Summary: Build entity from pointer
- `T? Sharp.Shared.Managers.IEntityManager.CreateEntityByName<T>(string classname) where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:164]
  - Modifiers: public, abstract
  - Summary: Generic version of .
- `T? Sharp.Shared.Managers.IEntityManager.FindEntityByHandle<T>(Sharp.Shared.Types.CEntityHandle<T> eHandle) where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:45]
  - Modifiers: public, abstract
  - Summary: Find entity by EHandle
- `T? Sharp.Shared.Managers.IEntityManager.FindEntityByIndex<T>(Sharp.Shared.Units.EntityIndex index) where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:66]
  - Modifiers: public, abstract
  - Summary: Find entity by Index
- `T? Sharp.Shared.Managers.IEntityManager.SpawnEntitySync<T>(string classname, System.Collections.Generic.IReadOnlyDictionary<string, Sharp.Shared.Types.KeyValuesVariantValueItem> keyValues) where T : class, Sharp.Shared.GameEntities.IBaseEntity` [L:144]
  - Modifiers: public, abstract
  - Summary: Generic version of .
- `bool Sharp.Shared.Managers.IEntityManager.UpdateEconItemAttributes(Sharp.Shared.GameEntities.IBaseEntity entity, uint accountId, string nameTag, int paint, int pattern, float wear, int nSticker1, float flSticker1, int nSticker2, float flSticker2, int nSticker3, float flSticker3, int nSticker4, float flSticker4)` [L:208]
  - Modifiers: public, abstract
  - Summary: Update Econ entity attributes
- `void Sharp.Shared.Managers.IEntityManager.HookEntityInput(string classname, string input)` [L:179]
  - Modifiers: public, abstract
  - Summary: Listen for entity Input
- `void Sharp.Shared.Managers.IEntityManager.HookEntityOutput(string classname, string output)` [L:174]
  - Modifiers: public, abstract
  - Summary: Listen for entity Output
- `void Sharp.Shared.Managers.IEntityManager.InstallEntityListener(Sharp.Shared.Listeners.IEntityListener listener)` [L:35]
  - Modifiers: public, abstract
  - Summary: Add  to listen for events
- `void Sharp.Shared.Managers.IEntityManager.RemoveEntityListener(Sharp.Shared.Listeners.IEntityListener listener)` [L:40]
  - Modifiers: public, abstract
  - Summary: Remove


### interface IEventManager

- FullName: `Sharp.Shared.Managers.IEventManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/EventManager.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.Objects.IGameEvent? Sharp.Shared.Managers.IEventManager.CreateEvent(string name, bool force)` [L:41]
  - Modifiers: public, abstract
  - Summary: Create Game Event
- `T? Sharp.Shared.Managers.IEventManager.CloneEvent<T>(T @event) where T : class, Sharp.Shared.Objects.IGameEvent` [L:52]
  - Modifiers: public, abstract
  - Summary: Clone event (editable)  Clone a new event, requires manual release or firing later
- `T? Sharp.Shared.Managers.IEventManager.CreateEvent<T>(bool force) where T : class, Sharp.Shared.Objects.IGameEvent` [L:46]
  - Modifiers: public, abstract
  - Summary: Create Game Event
- `bool Sharp.Shared.Managers.IEventManager.FindListener(Sharp.Shared.Units.PlayerSlot slot, string name)` [L:62]
  - Modifiers: public, abstract
  - Summary: Check client subscribed events
- `void Sharp.Shared.Managers.IEventManager.HookEvent(string name)` [L:57]
  - Modifiers: public, abstract
  - Summary: Add an event name to the Hook queue
- `void Sharp.Shared.Managers.IEventManager.InstallEventListener(Sharp.Shared.Listeners.IEventListener listener)` [L:31]
  - Modifiers: public, abstract
  - Summary: Add  to listen for events
- `void Sharp.Shared.Managers.IEventManager.RemoveEventListener(Sharp.Shared.Listeners.IEventListener listener)` [L:36]
  - Modifiers: public, abstract
  - Summary: Remove


### interface IFileManager

- FullName: `Sharp.Shared.Managers.IFileManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/FileManager.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.Managers.IValveDirectory? Sharp.Shared.Managers.IFileManager.OpenDirectory(string path, [string pathId = "GAME"])` [L:49]
  - Modifiers: public, abstract
  - Summary: Open directory Uses engine file system, supports vp access
- `Sharp.Shared.Managers.IValveFile? Sharp.Shared.Managers.IFileManager.OpenFile(string filename, [string pathId = "GAME"])` [L:43]
  - Modifiers: public, abstract
  - Summary: Open file Uses engine file system, supports vp access
- `bool Sharp.Shared.Managers.IFileManager.FileExists(string filename, [string pathId = "GAME"])` [L:37]
  - Modifiers: public, abstract
  - Summary: Check if file exists Uses engine file system, supports vp access
- `nint Sharp.Shared.Managers.IFileManager.GetValveFileSystem()` [L:31]
  - Modifiers: public, abstract
  - Summary: Get Source2 file system interface pointer
- `void Sharp.Shared.Managers.IFileManager.AddSearchPath(string path, string pathId, [int addType = 1], [int priority = 0], [int unknown = 0])` [L:54]
  - Modifiers: public, abstract
  - Summary: Add path to engine file system search paths
- `void Sharp.Shared.Managers.IFileManager.RemoveSearchPath(string path, string pathId)` [L:59]
  - Modifiers: public, abstract
  - Summary: Remove search path from engine file system


### interface IForwardType<TParams>

- FullName: `Sharp.Shared.Managers.IForwardType<TParams>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/HookManager.cs:485
- Generated: false
- Constraint: `where TParams : class, Sharp.Shared.HookParams.IFunctionParams`

#### Methods
- `void Sharp.Shared.Managers.IForwardType<out TParams>.InstallForward(System.Action<out TParams> func, [int priority = 0])` [L:491]
  - Modifiers: public, abstract
  - Summary: Listen to this Forward call Higher priority value means higher priority
- `void Sharp.Shared.Managers.IForwardType<out TParams>.RemoveForward(System.Action<out TParams> func)` [L:496]
  - Modifiers: public, abstract
  - Summary: Stop listening to this Forward call


### interface IHookManager

- FullName: `Sharp.Shared.Managers.IHookManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/HookManager.cs:30
- Generated: false

#### Properties
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IEmitMusicForwardParams> Sharp.Shared.Managers.IHookManager.EmitMusic` [L:342]
  - Modifiers: public, abstract, readonly
  - Summary: SoundOpGameSystem::DoStartSoundEvent Only fires when the sound event is treated as music
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IGiveGloveItemForwardParams> Sharp.Shared.Managers.IHookManager.GiveGloveItem` [L:393]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->ItemService::GiveGloveItem
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IMapVoteCreatedForwardParams> Sharp.Shared.Managers.IHookManager.MapVoteCreated` [L:453]
  - Modifiers: public, abstract, readonly
  - Summary: CCSGameRules::CreateEndMatchMapGroupVoteOptions
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerDropWeaponForwardParams> Sharp.Shared.Managers.IHookManager.PlayerDropWeapon` [L:444]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::DropWeapon
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerEquipWeaponForwardParams> Sharp.Shared.Managers.IHookManager.PlayerEquipWeapon` [L:439]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::EquipWeapon
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerKilledForwardParams> Sharp.Shared.Managers.IHookManager.PlayerKilledPost` [L:366]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::Killed
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerKilledForwardParams> Sharp.Shared.Managers.IHookManager.PlayerKilledPre` [L:361]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::Killed
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerProcessMoveForwardParams> Sharp.Shared.Managers.IHookManager.PlayerProcessMovePost` [L:425]
  - Modifiers: public, abstract, readonly
  - Summary: CPlayer_MovementService::ProcessMove
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerProcessMoveForwardParams> Sharp.Shared.Managers.IHookManager.PlayerProcessMovePre` [L:416]
  - Modifiers: public, abstract, readonly
  - Summary: CPlayer_MovementService::ProcessMove
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerSpawnForwardParams> Sharp.Shared.Managers.IHookManager.PlayerSpawnPost` [L:356]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerSpawnForwardParams> Sharp.Shared.Managers.IHookManager.PlayerSpawnPre` [L:351]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::PlayerSpawn
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerSwitchWeaponForwardParams> Sharp.Shared.Managers.IHookManager.PlayerSwitchWeapon` [L:434]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::SwitchWeapon
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerThinkForwardParams> Sharp.Shared.Managers.IHookManager.PlayerPostThink` [L:384]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::PostThink
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerThinkForwardParams> Sharp.Shared.Managers.IHookManager.PlayerPreThink` [L:375]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::PreThink
- `Sharp.Shared.Managers.IForwardType<Sharp.Shared.HookParams.IPlayerWalkMoveForwardParams> Sharp.Shared.Managers.IHookManager.PlayerWalkMove` [L:407]
  - Modifiers: public, abstract, readonly
  - Summary: CPlayer_MovementService::WalkMove
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IClientCanHearHookParams, bool> Sharp.Shared.Managers.IHookManager.ClientCanHear` [L:75]
  - Modifiers: public, abstract, readonly
  - Summary: CServerSideClient::ClientCanHear
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IClientSpeakingHookParams, Sharp.Shared.HookParams.EmptyHookReturn> Sharp.Shared.Managers.IHookManager.ClientSpeaking` [L:85]
  - Modifiers: public, abstract, readonly
  - Summary: CServerSideClient:CLCMsg_VoiceData
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IConnectClientHookParams, Sharp.Shared.Enums.NetworkDisconnectionReason> Sharp.Shared.Managers.IHookManager.ConnectClient` [L:59]
  - Modifiers: public, abstract, readonly
  - Summary: CNetworkGameServer::ConnectClient
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IEmitSoundHookParams, Sharp.Shared.Types.SoundOpEventGuid> Sharp.Shared.Managers.IHookManager.EmitSound` [L:206]
  - Modifiers: public, abstract, readonly
  - Summary: CSoundEmitterSystem::EmitSound
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IEntityDispatchTraceAttackHookParams, long> Sharp.Shared.Managers.IHookManager.EntityDispatchTraceAttack` [L:267]
  - Modifiers: public, abstract, readonly
  - Summary: CBaseEntity::DispatchTraceAttack (No PlayerPawn)
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IGiveNamedItemHookParams, Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Shared.Managers.IHookManager.GiveNamedItem` [L:173]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->ItemService::GiveNamedItem
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams, bool> Sharp.Shared.Managers.IHookManager.HandleCommandJoinTeam` [L:163]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerController::HandleCommandJoinTeam
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerCanAcquireHookParams, Sharp.Shared.Enums.EAcquireResult> Sharp.Shared.Managers.IHookManager.PlayerCanAcquire` [L:151]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayer_ItemServices::CanAcquire
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerDispatchTraceAttackHookParams, long> Sharp.Shared.Managers.IHookManager.PlayerDispatchTraceAttack` [L:244]
  - Modifiers: public, abstract, readonly
  - Summary: CBaseEntity::DispatchTraceAttack (PlayerPawn Only)
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerGetMaxSpeedHookParams, float> Sharp.Shared.Managers.IHookManager.PlayerGetMaxSpeed` [L:140]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn::GetPlayerMaxSpeed
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerRunCommandHookParams, Sharp.Shared.HookParams.EmptyHookReturn> Sharp.Shared.Managers.IHookManager.PlayerRunCommand` [L:191]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->MovementService::RunCommand
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerWeaponCanEquipHookParams, bool> Sharp.Shared.Managers.IHookManager.PlayerWeaponCanEquip` [L:126]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::CanEquip
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerWeaponCanSwitchHookParams, bool> Sharp.Shared.Managers.IHookManager.PlayerWeaponCanSwitch` [L:110]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::WeaponCanSwitch
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPlayerWeaponCanUseHookParams, bool> Sharp.Shared.Managers.IHookManager.PlayerWeaponCanUse` [L:100]
  - Modifiers: public, abstract, readonly
  - Summary: CCSPlayerPawn->WeaponService::WeaponCanUse
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPointServerCommandHookParams, Sharp.Shared.HookParams.EmptyHookReturn> Sharp.Shared.Managers.IHookManager.PointServerCommand` [L:281]
  - Modifiers: public, abstract, readonly
  - Summary: CPointServerCommand::InputCommand
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPostEventAbstractHookParams, Sharp.Shared.Units.NetworkReceiver> Sharp.Shared.Managers.IHookManager.PostEventAbstract` [L:317]
  - Modifiers: public, abstract, readonly
  - Summary: IGameEventSystem::PostEventAbstract
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IPrintStatusHookParams, Sharp.Shared.HookParams.EmptyHookReturn> Sharp.Shared.Managers.IHookManager.PrintStatus` [L:292]
  - Modifiers: public, abstract, readonly
  - Summary: 'status' Command When client is null means it is sent by server
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.ISoundEventHookParams, Sharp.Shared.Types.SoundOpEventGuid> Sharp.Shared.Managers.IHookManager.SoundEvent` [L:217]
  - Modifiers: public, abstract, readonly
  - Summary: SoundOpGameSystem::DoStartSoundEvent
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.ITerminateRoundHookParams, Sharp.Shared.HookParams.EmptyHookReturn> Sharp.Shared.Managers.IHookManager.TerminateRound` [L:328]
  - Modifiers: public, abstract, readonly
  - Summary: CCSGameRules::TerminateRound
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.ITextMsgHookParams, Sharp.Shared.Units.NetworkReceiver> Sharp.Shared.Managers.IHookManager.TextMsg` [L:305]
  - Modifiers: public, abstract, readonly

#### Methods
- `Sharp.Shared.Hooks.IDetourHook Sharp.Shared.Managers.IHookManager.CreateDetourHook()` [L:35]
  - Modifiers: public, abstract
  - Summary: Create DetourHook
- `Sharp.Shared.Hooks.IMidFuncHook Sharp.Shared.Managers.IHookManager.CreateMidFuncHook()` [L:45]
  - Modifiers: public, abstract
  - Summary: Create MidFuncHook
- `Sharp.Shared.Hooks.IVirtualHook Sharp.Shared.Managers.IHookManager.CreateVirtualHook()` [L:40]
  - Modifiers: public, abstract
  - Summary: Create VMThook

#### Obsolete Members
- `Sharp.Shared.Managers.IHookType<Sharp.Shared.HookParams.IClientConnectHookParams, bool> Sharp.Shared.Managers.IHookManager.ClientConnect` [L:65] — Use ConnectClient instead, will be removed in the future


### interface IHookType<TParams, THookReturn>

- FullName: `Sharp.Shared.Managers.IHookType<TParams, THookReturn>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/HookManager.cs:460
- Generated: false
- Constraint: `where TParams : class, Sharp.Shared.HookParams.IFunctionParams`

#### Methods
- `void Sharp.Shared.Managers.IHookType<out TParams, THookReturn>.InstallHookPost(System.Action<out TParams, Sharp.Shared.Types.HookReturnValue<THookReturn>> post, [int priority = 0])` [L:472]
  - Modifiers: public, abstract
  - Summary: Listen to this Hook's Post Higher priority value means higher priority
- `void Sharp.Shared.Managers.IHookType<out TParams, THookReturn>.InstallHookPre(System.Func<out TParams, Sharp.Shared.Types.HookReturnValue<THookReturn>, Sharp.Shared.Types.HookReturnValue<THookReturn>> pre, [int priority = 0])` [L:466]
  - Modifiers: public, abstract
  - Summary: Listen to this Hook's Pre Higher priority value means higher priority
- `void Sharp.Shared.Managers.IHookType<out TParams, THookReturn>.RemoveHookPost(System.Action<out TParams, Sharp.Shared.Types.HookReturnValue<THookReturn>> post)` [L:482]
  - Modifiers: public, abstract
  - Summary: Stop listening to this Hook's Post
- `void Sharp.Shared.Managers.IHookType<out TParams, THookReturn>.RemoveHookPre(System.Func<out TParams, Sharp.Shared.Types.HookReturnValue<THookReturn>, Sharp.Shared.Types.HookReturnValue<THookReturn>> pre)` [L:477]
  - Modifiers: public, abstract
  - Summary: Stop listening to this Hook's Pre


### interface ILibraryModuleManager

- FullName: `Sharp.Shared.Managers.ILibraryModuleManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/LibraryModuleManager.cs:35
- Generated: false
- Summary: Provides access to loaded game libraries (modules) for memory scanning and address retrieval.

#### Properties
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.Engine` [L:38]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.FileSystem` [L:48]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.MatchMaking` [L:47]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.MaterialSystem` [L:50]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.NetworkSystem` [L:45]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.Resource` [L:41]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.Schema` [L:40]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.Server` [L:37]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.SoundSystem` [L:44]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.SteamNetworkingSocket` [L:49]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.Tier0` [L:39]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.VPhysics` [L:43]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.VScript` [L:42]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.ILibraryModule Sharp.Shared.Managers.ILibraryModuleManager.WorldRenderer` [L:46]
  - Modifiers: public, abstract, readonly


### interface IParticleManager

- FullName: `Sharp.Shared.Managers.IParticleManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/ParticleManager.cs:26
- Generated: false

#### Methods
- `void Sharp.Shared.Managers.IParticleManager.DispatchEffect(string effectName, Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.Types.Vector origin, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:56]
  - Modifiers: public, abstract
  - Summary: Dispatch effects (csshocked, cstaserrope, gunshotsplash, csblood etc.)
- `void Sharp.Shared.Managers.IParticleManager.DispatchParticleEffect(string particle, Sharp.Shared.Enums.ParticleAttachmentType attachType, Sharp.Shared.GameEntities.IBaseEntity entity, [byte attachmentIndex = 0], [bool resetEntity = false], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:46]
  - Modifiers: public, abstract
  - Summary: Dispatch particle effect (.vpcf)
- `void Sharp.Shared.Managers.IParticleManager.DispatchParticleEffect(string particle, Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.Types.Vector origin, Sharp.Shared.Types.Vector angles, [bool resetEntity = false], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:36]
  - Modifiers: public, abstract
  - Summary: Dispatch particle effect (.vpcf)
- `void Sharp.Shared.Managers.IParticleManager.DispatchParticleEffect(string particle, Sharp.Shared.Types.Vector origin, Sharp.Shared.Types.Vector angles, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:31]
  - Modifiers: public, abstract
  - Summary: Dispatch particle effect (.vpcf)


### interface IPhysicsQueryManager

- FullName: `Sharp.Shared.Managers.IPhysicsQueryManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/PhysicsQueryManager.cs:27
- Generated: false

#### Methods
- `Sharp.Shared.Types.GameTrace Sharp.Shared.Managers.IPhysicsQueryManager.TraceLine(Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, in Sharp.Shared.Types.RnQueryShapeAttr query, [nint? filterCallback = null])` [L:183]
  - Modifiers: public, abstract
  - Summary: TraceLine
- `Sharp.Shared.Types.GameTrace Sharp.Shared.Managers.IPhysicsQueryManager.TraceLineNoPlayers(Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, in Sharp.Shared.Types.RnQueryShapeAttr query)` [L:209]
  - Modifiers: public, abstract
  - Summary: TraceLine (filters players)
- `Sharp.Shared.Types.GameTrace Sharp.Shared.Managers.IPhysicsQueryManager.TraceShape(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, in Sharp.Shared.Types.RnQueryShapeAttr query, [nint? filterCallback = null])` [L:174]
  - Modifiers: public, abstract
  - Summary: TraceShape
- `Sharp.Shared.Types.GameTrace Sharp.Shared.Managers.IPhysicsQueryManager.TraceShapeNoPlayers(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, in Sharp.Shared.Types.RnQueryShapeAttr query)` [L:201]
  - Modifiers: public, abstract
  - Summary: TraceShape (filters players)
- `Sharp.Shared.Types.GameTrace Sharp.Shared.Managers.IPhysicsQueryManager.TraceShapePlayerMovement(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, in Sharp.Shared.Types.RnQueryShapeAttr query)` [L:192]
  - Modifiers: public, abstract
  - Summary: TraceShapePlayerMovement
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceLine(Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, [Sharp.Shared.Enums.InteractionLayers excludeLayers = Sharp.Shared.Enums.InteractionLayers.None], [Sharp.Shared.GameEntities.IBaseEntity? ignore1 = null], [Sharp.Shared.GameEntities.IBaseEntity? ignore2 = null])` [L:40]
  - Modifiers: public, abstract
  - Summary: TraceLine
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceLineFilter(Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, System.Func<Sharp.Shared.GameEntities.IBaseEntity, bool> filter)` [L:79]
  - Modifiers: public, abstract
  - Summary: TraceLine with custom filter
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceLineNoPlayers(Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, [Sharp.Shared.Enums.InteractionLayers excludeLayers = Sharp.Shared.Enums.InteractionLayers.None], [Sharp.Shared.GameEntities.IBaseEntity? ignore1 = null], [Sharp.Shared.GameEntities.IBaseEntity? ignore2 = null])` [L:60]
  - Modifiers: public, abstract
  - Summary: TraceLine but ignores players
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceShape(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, [Sharp.Shared.Enums.InteractionLayers excludeLayers = Sharp.Shared.Enums.InteractionLayers.None], [Sharp.Shared.GameEntities.IBaseEntity? ignore1 = null], [Sharp.Shared.GameEntities.IBaseEntity? ignore2 = null])` [L:99]
  - Modifiers: public, abstract
  - Summary: TraceShape
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceShapeFilter(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, System.Func<Sharp.Shared.GameEntities.IBaseEntity, bool> filter)` [L:142]
  - Modifiers: public, abstract
  - Summary: TraceShape with custom filter
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceShapeNoPlayers(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, [Sharp.Shared.Enums.InteractionLayers excludeLayers = Sharp.Shared.Enums.InteractionLayers.None], [Sharp.Shared.GameEntities.IBaseEntity? ignore1 = null], [Sharp.Shared.GameEntities.IBaseEntity? ignore2 = null])` [L:121]
  - Modifiers: public, abstract
  - Summary: TraceShape but ignores players
- `int Sharp.Shared.Managers.IPhysicsQueryManager.EntitiesAlongRay(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector origin, in Sharp.Shared.Types.RnQueryShapeAttr query, bool unique, System.Span<uint> entities, [uint test = 1], [nint? filterCallback = null])` [L:222]
  - Modifiers: public, abstract
  - Summary: Enumerate entities along a ray

#### Obsolete Members
- `Sharp.Shared.Types.TraceResult Sharp.Shared.Managers.IPhysicsQueryManager.TraceShapePlayerMovement(Sharp.Shared.Types.TraceShapeRay ray, Sharp.Shared.Types.Vector start, Sharp.Shared.Types.Vector end, Sharp.Shared.Enums.InteractionLayers interactsWith, Sharp.Shared.GameEntities.IPlayerPawn pawn)` [L:160] — Does not work, will be removed in 2.2


### interface ISchemaManager

- FullName: `Sharp.Shared.Managers.ISchemaManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/SchemaManager.cs:33
- Generated: false
- Summary: Low-level interface for interacting with Native Schema.

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<T> Sharp.Shared.Managers.ISchemaManager.GetSchemaFixedArray<T>(nint pointer, Sharp.Shared.SchemaField field, Sharp.Shared.CStrike.ISchemaObject chain) where T : unmanaged` [L:242]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.CStrike.ISchemaArray<T> Sharp.Shared.Managers.ISchemaManager.GetSchemaFixedArray<T>(nint pointer, string classname, string field, Sharp.Shared.CStrike.ISchemaObject chain) where T : unmanaged` [L:232]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.CStrike.ISchemaList<T> Sharp.Shared.Managers.ISchemaManager.GetSchemaList<T>(nint pointer, Sharp.Shared.SchemaField field, Sharp.Shared.CStrike.ISchemaObject chain, bool isStruct) where T : unmanaged` [L:262]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.CStrike.ISchemaList<T> Sharp.Shared.Managers.ISchemaManager.GetSchemaList<T>(nint pointer, string classname, string field, Sharp.Shared.CStrike.ISchemaObject chain, bool isStruct) where T : unmanaged` [L:252]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.SchemaField Sharp.Shared.Managers.ISchemaManager.GetSchemaField(string classname, string field)` [L:42]
  - Modifiers: public, abstract
  - Summary: Gets a Schema field
- `Sharp.Shared.Types.Vector Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [Sharp.Shared.Types.Vector? _ = null]) where T : System.IComparable<Sharp.Shared.Types.Vector>` [L:179]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `bool Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [bool? _ = null]) where T : System.IComparable<bool>` [L:58]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `byte Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [byte? _ = null]) where T : System.IComparable<byte>` [L:69]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `float Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [float? _ = null]) where T : System.IComparable<float>` [L:146]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `int Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [int? _ = null]) where T : System.IComparable<int>` [L:102]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `int Sharp.Shared.Managers.ISchemaManager.GetNetVarOffset(string classname, string field)` [L:48]
  - Modifiers: public, abstract
  - Summary: Gets the offset of a Schema member variable
- `long Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [long? _ = null]) where T : System.IComparable<long>` [L:124]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `nint Sharp.Shared.Managers.ISchemaManager.GetDataMapInputFunc(string classname, string fieldName)` [L:521]
  - Modifiers: public, abstract
  - Summary: Get the datamap input function address.
- `nint Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [nint? _ = null]) where T : System.IComparable<nint>` [L:157]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ref Sharp.Shared.Types.Tier.CUtlString Sharp.Shared.Managers.ISchemaManager.GetNetVarUtlStringRef(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0])` [L:223]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ref Sharp.Shared.Types.Tier.CUtlSymbolLarge Sharp.Shared.Managers.ISchemaManager.GetNetVarUtlSymbolLargeRef(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0])` [L:200]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `short Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [short? _ = null]) where T : System.IComparable<short>` [L:80]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [string? _ = null]) where T : System.IComparable<string>` [L:168]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.Managers.ISchemaManager.GetNetVarUtlString(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0])` [L:213]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.Managers.ISchemaManager.GetNetVarUtlSymbolLarge(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0])` [L:190]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `uint Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [uint? _ = null]) where T : System.IComparable<uint>` [L:113]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ulong Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [ulong? _ = null]) where T : System.IComparable<ulong>` [L:135]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ushort Sharp.Shared.Managers.ISchemaManager.GetNetVar<T>(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, [ushort extraOffset = 0], [ushort? _ = null]) where T : System.IComparable<ushort>` [L:91]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `void Sharp.Shared.Managers.ISchemaManager.NetVarStateChanged(Sharp.Shared.CStrike.INativeObject nativeObject, Sharp.Shared.SchemaClass schemaClass, Sharp.Shared.SchemaClassField schemaField, [ushort extraOffset = 0], [bool isStruct = false])` [L:507]
  - Modifiers: public, abstract
  - Summary: Automatically calls NetworkStateChanged or StateChanged
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, Sharp.Shared.Types.Vector value, [bool isStruct = false], [ushort extraOffset = 0])` [L:457]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, bool value, [bool isStruct = false], [ushort extraOffset = 0])` [L:276]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, byte value, [bool isStruct = false], [ushort extraOffset = 0])` [L:294]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, float value, [bool isStruct = false], [ushort extraOffset = 0])` [L:420]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, int value, [bool isStruct = false], [ushort extraOffset = 0])` [L:348]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, long value, [bool isStruct = false], [ushort extraOffset = 0])` [L:384]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, short value, [bool isStruct = false], [ushort extraOffset = 0])` [L:312]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, string value, int maxLen, [bool isStruct = false], [ushort extraOffset = 0])` [L:438]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, uint value, [bool isStruct = false], [ushort extraOffset = 0])` [L:366]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, ulong value, [bool isStruct = false], [ushort extraOffset = 0])` [L:402]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVar(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, ushort value, [bool isStruct = false], [ushort extraOffset = 0])` [L:330]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVarUtlString(Sharp.Shared.CStrike.INativeObject ptr, string classname, string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:492]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.Managers.ISchemaManager.SetNetVarUtlSymbolLarge(Sharp.Shared.CStrike.INativeObject nativeObject, string classname, string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:475]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member


### interface ISharpModuleManager

- FullName: `Sharp.Shared.Managers.ISharpModuleManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/SharpModuleManager.cs:24
- Generated: false

#### Methods
- `Sharp.Shared.IModSharpModuleInterface<T> Sharp.Shared.Managers.ISharpModuleManager.GetRequiredSharpModuleInterface<T>(string identity) where T : class` [L:35]
  - Modifiers: public, abstract
  - Summary: Get the required sharp module interface. If the interface is not found, an exception is thrown.
- `Sharp.Shared.IModSharpModuleInterface<T>? Sharp.Shared.Managers.ISharpModuleManager.GetOptionalSharpModuleInterface<T>(string identity) where T : class` [L:40]
  - Modifiers: public, abstract
  - Summary: Get the optional sharp module interface.
- `System.Delegate? Sharp.Shared.Managers.ISharpModuleManager.GetDynamicNative(string name)` [L:57]
  - Modifiers: public, abstract
  - Summary: Get dynamic native function
- `void Sharp.Shared.Managers.ISharpModuleManager.RegisterDynamicNative(Sharp.Shared.IModSharpModule owner, string name, System.Delegate function)` [L:46]
  - Modifiers: public, abstract
  - Summary: Register dynamic native functions for convenient debugging, performance is actually decent tooIt is the same as SourceMod, you can use it however you want
- `void Sharp.Shared.Managers.ISharpModuleManager.RegisterSharpModuleInterface<T>(Sharp.Shared.IModSharpModule owner, string identity, T impl) where T : class` [L:29]
  - Modifiers: public, abstract
  - Summary: Register your current module as a library to allow other modules to use the interface


### interface ISoundManager

- FullName: `Sharp.Shared.Managers.ISoundManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/SoundManager.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.Types.SoundOpEventGuid Sharp.Shared.Managers.ISoundManager.StartSoundEvent(string sound, [Sharp.Shared.GameEntities.IBaseEntity? entity = null], [float? volume = null], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:35]
  - Modifiers: public, abstract
  - Summary: Starts a SoundEvent
- `bool Sharp.Shared.Managers.ISoundManager.IsSoundEventValid(string soundEvent)` [L:78]
  - Modifiers: public, abstract
  - Summary: Checks if a SoundEvent is valid
- `bool Sharp.Shared.Managers.ISoundManager.SetSoundEventParam(Sharp.Shared.Types.SoundOpEventGuid guid, string param, Sharp.Shared.Types.Vector value, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:58]
  - Modifiers: public, abstract
  - Summary: Sets a SoundEvent parameter
- `bool Sharp.Shared.Managers.ISoundManager.SetSoundEventParam(Sharp.Shared.Types.SoundOpEventGuid guid, string param, float value, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:53]
  - Modifiers: public, abstract
  - Summary: Sets a SoundEvent parameter
- `bool Sharp.Shared.Managers.ISoundManager.SetSoundEventParam(Sharp.Shared.Types.SoundOpEventGuid guid, string param, int value, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:63]
  - Modifiers: public, abstract
  - Summary: Sets a SoundEvent parameter
- `bool Sharp.Shared.Managers.ISoundManager.SetSoundEventParam(Sharp.Shared.Types.SoundOpEventGuid guid, string param, uint value, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:68]
  - Modifiers: public, abstract
  - Summary: Sets a SoundEvent parameter
- `bool Sharp.Shared.Managers.ISoundManager.SetSoundEventParam(Sharp.Shared.Types.SoundOpEventGuid guid, string param, ulong value, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:73]
  - Modifiers: public, abstract
  - Summary: Sets a SoundEvent parameter
- `float Sharp.Shared.Managers.ISoundManager.GetSoundDuration(string soundEvent)` [L:30]
  - Modifiers: public, abstract
  - Summary: Gets the duration of a SoundEvent
- `void Sharp.Shared.Managers.ISoundManager.StopSoundEvent(Sharp.Shared.Types.SoundOpEventGuid guid)` [L:43]
  - Modifiers: public, abstract
  - Summary: Stops a SoundEvent
- `void Sharp.Shared.Managers.ISoundManager.StopSoundEvent(Sharp.Shared.Types.SoundOpEventGuid guid, Sharp.Shared.Types.RecipientFilter filter)` [L:48]
  - Modifiers: public, abstract
  - Summary: Stops a SoundEvent


### interface ITransmitManager

- FullName: `Sharp.Shared.Managers.ITransmitManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/TransmitManager.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.Enums.TransmitFireBulletState Sharp.Shared.Managers.ITransmitManager.GetWeaponFireBulletState(Sharp.Shared.GameEntities.IBaseWeapon weapon)` [L:117]
  - Modifiers: public, abstract
  - Summary: Gets the blocking state for fire bullet effects (e.g., sound, visual effects).
- `bool Sharp.Shared.Managers.ITransmitManager.AddEntityHooks(Sharp.Shared.GameEntities.IBaseEntity entity, bool defaultTransmit)` [L:33]
  - Modifiers: public, abstract
  - Summary: Hook an entity
- `bool Sharp.Shared.Managers.ITransmitManager.GetEntityBlock(Sharp.Shared.Units.EntityIndex entity)` [L:67]
  - Modifiers: public, abstract
  - Summary: Get whether entity is blocked
- `bool Sharp.Shared.Managers.ITransmitManager.GetEntityState(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex controllerIndex, [int channel = -1])` [L:53]
  - Modifiers: public, abstract
  - Summary: Get entity visibility state for a controller
- `bool Sharp.Shared.Managers.ITransmitManager.GetTempEntState(Sharp.Shared.Enums.BlockTempEntType type, Sharp.Shared.Units.PlayerSlot slot)` [L:93]
  - Modifiers: public, abstract
  - Summary: Checks if a specific temporary entity type is currently blocked for a player.
- `bool Sharp.Shared.Managers.ITransmitManager.IsEntityHooked(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:45]
  - Modifiers: public, abstract
  - Summary: Check if entity is already hooked
- `bool Sharp.Shared.Managers.ITransmitManager.RemoveEntityHooks(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:39]
  - Modifiers: public, abstract
  - Summary: Manually remove hooks
- `bool Sharp.Shared.Managers.ITransmitManager.SetEntityBlock(Sharp.Shared.Units.EntityIndex entity, bool state)` [L:72]
  - Modifiers: public, abstract
  - Summary: Set entity block state
- `bool Sharp.Shared.Managers.ITransmitManager.SetEntityOwner(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex owner)` [L:85]
  - Modifiers: public, abstract
  - Summary: Set entity owner in hook
- `bool Sharp.Shared.Managers.ITransmitManager.SetEntityState(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex controllerIndex, bool transmit, int channel)` [L:62]
  - Modifiers: public, abstract
  - Summary: Set entity visibility state for a controller
- `int Sharp.Shared.Managers.ITransmitManager.GetEntityOwner(Sharp.Shared.Units.EntityIndex entity)` [L:78]
  - Modifiers: public, abstract
  - Summary: Get entity owner from hook
- `void Sharp.Shared.Managers.ITransmitManager.ClearReceiverState(Sharp.Shared.Units.EntityIndex receiverIndex)` [L:110]
  - Modifiers: public, abstract
  - Summary: Reset all entity states for a receiver
- `void Sharp.Shared.Managers.ITransmitManager.SetTempEntState(Sharp.Shared.Enums.BlockTempEntType type, Sharp.Shared.Units.PlayerSlot slot, bool state)` [L:104]
  - Modifiers: public, abstract
  - Summary: Configures whether a specific temporary entity type is blocked for a player.
- `void Sharp.Shared.Managers.ITransmitManager.SetWeaponFireBulletState(Sharp.Shared.GameEntities.IBaseWeapon weapon, Sharp.Shared.Enums.TransmitFireBulletState state)` [L:122]
  - Modifiers: public, abstract
  - Summary: Sets the blocking state for fire bullet effects (e.g., sound, visual effects).


### interface IValveDirectory : System.IDisposable

- FullName: `Sharp.Shared.Managers.IValveDirectory`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/FileManager.cs:80
- Generated: false

#### Methods
- `System.Collections.Generic.IEnumerator<string> Sharp.Shared.Managers.IValveDirectory.GetEnumerator()` [L:85]
  - Modifiers: public, abstract
  - Summary: Iterate through directory


### interface IValveFile : Sharp.Shared.CStrike.INativeObject, System.IDisposable

- FullName: `Sharp.Shared.Managers.IValveFile`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Managers/FileManager.cs:62
- Generated: false

#### Methods
- `int Sharp.Shared.Managers.IValveFile.Size()` [L:77]
  - Modifiers: public, abstract
  - Summary: Get file size
- `void Sharp.Shared.Managers.IValveFile.Read(System.Span<byte> output)` [L:67]
  - Modifiers: public, abstract
  - Summary: Read data from file
- `void Sharp.Shared.Managers.IValveFile.Write(System.ReadOnlySpan<byte> input)` [L:72]
  - Modifiers: public, abstract
  - Summary: Write data to file


