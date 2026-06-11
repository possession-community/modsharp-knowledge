# Sharp.Shared

Project: Sharp.Shared
Types: 12 (0 generated)

### record DataMapField : System.IEquatable<Sharp.Shared.DataMapField>

- FullName: `Sharp.Shared.DataMapField`
- Kind: record
- Modifiers: public
- Source: Sharp.Shared/SharedGameObject.cs:48
- Generated: false

Inheritance: object → **DataMapField**

#### Properties
- `nint Sharp.Shared.DataMapField.InputFunc` [L:53]
  - Attributes: `[JsonIgnore]`
- `required string Sharp.Shared.DataMapField.Name` [L:50]


### interface IGameData

- FullName: `Sharp.Shared.IGameData`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/IGameData.cs:22
- Generated: false

#### Methods
- `bool Sharp.Shared.IGameData.GetAddress(string name, out nint address)` [L:38]
  - Modifiers: public, abstract
  - Summary: Try to get address by key
- `bool Sharp.Shared.IGameData.GetOffset(string name, out int offset)` [L:30]
  - Modifiers: public, abstract
  - Summary: Try to get offset by key
- `bool Sharp.Shared.IGameData.GetVFuncIndex(string name, out int index)` [L:46]
  - Modifiers: public, abstract
  - Summary: Try to get virtual function index by key
- `int Sharp.Shared.IGameData.GetOffset(string classname, string name)` [L:61]
  - Modifiers: public, abstract
  - Summary: Get offset using class::member format
- `int Sharp.Shared.IGameData.GetOffset(string name)` [L:53]
  - Modifiers: public, abstract
  - Summary: Get offset by key, throws exception if not found
- `int Sharp.Shared.IGameData.GetVFuncIndex(string classname, string name)` [L:91]
  - Modifiers: public, abstract
  - Summary: Get virtual function index using class::member format
- `int Sharp.Shared.IGameData.GetVFuncIndex(string name)` [L:83]
  - Modifiers: public, abstract
  - Summary: Get virtual function index by key
- `nint Sharp.Shared.IGameData.GetAddress(string classname, string name)` [L:76]
  - Modifiers: public, abstract
  - Summary: Get address using class::member format
- `nint Sharp.Shared.IGameData.GetAddress(string name)` [L:68]
  - Modifiers: public, abstract
  - Summary: Get address by key, throws exception if not found
- `void Sharp.Shared.IGameData.Register(string path)` [L:97]
  - Modifiers: public, abstract
  - Summary: Register GameData file
- `void Sharp.Shared.IGameData.Unregister(string path)` [L:103]
  - Modifiers: public, abstract
  - Summary: Unregister GameData file


### interface ILibraryModule

- FullName: `Sharp.Shared.ILibraryModule`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/ILibraryModule.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.Types.VirtualTableInfo[] Sharp.Shared.ILibraryModule.FindVirtualTablesPartial(string str)` [L:92]
  - Modifiers: public, abstract
  - Summary: Finds virtual tables that contain the specified partial string in their type descriptor or name.
- `System.Collections.Generic.List<nint> Sharp.Shared.ILibraryModule.FindPatternMulti(string pattern)` [L:66]
  - Modifiers: public, abstract
  - Summary: Find multiple function addresses by IDA pattern.
- `bool Sharp.Shared.ILibraryModule.GetFunctionRange(nint middle, out nint start, out nint end)` [L:179]
  - Modifiers: public, abstract
  - Summary: Determines the start and end boundaries of a function given an address inside it.
- `bool Sharp.Shared.ILibraryModule.IsPointerDerivedFrom(nint ptr, string name)` [L:100]
  - Modifiers: public, abstract
  - Summary: Checks if the object instance at the specified pointer inherits from a class matching the given name.
- `nint Sharp.Shared.ILibraryModule.FindData(System.ReadOnlySpan<byte> data, bool readOnly)` [L:170]
  - Modifiers: public, abstract
  - Summary: Scans the module's known data sections for a specific byte sequence.
- `nint Sharp.Shared.ILibraryModule.FindFunction(System.ReadOnlySpan<nint> ptrs)` [L:145]
  - Modifiers: public, abstract
  - Summary: Finds the start address of a function that references any of the specific pointers (xref).
- `nint Sharp.Shared.ILibraryModule.FindFunction(System.ReadOnlySpan<string> strs)` [L:121]
  - Modifiers: public, abstract
  - Summary: Finds the start address of a function that references the specific string literal.
- `nint Sharp.Shared.ILibraryModule.FindFunction(nint ptr)` [L:139]
  - Modifiers: public, abstract
  - Summary: Finds the start address of a function that references the specific pointer (xref).
- `nint Sharp.Shared.ILibraryModule.FindFunction(string str)` [L:114]
  - Modifiers: public, abstract
  - Summary: Finds the start address of a function that references the specific string literal.
- `nint Sharp.Shared.ILibraryModule.FindInterface(string interfaceName)` [L:59]
  - Modifiers: public, abstract
  - Summary: Find a game VInterface pointer exposed by this module (via CreateInterface).
- `nint Sharp.Shared.ILibraryModule.FindPattern(string pattern, [nint startAddress = 0])` [L:33]
  - Modifiers: public, abstract
  - Summary: Find function address by IDA pattern (non-unique) This method is typically used for iterating through addresses
- `nint Sharp.Shared.ILibraryModule.FindPatternExactly(string pattern)` [L:53]
  - Modifiers: public, abstract
  - Summary: Find function address by IDA pattern (expecting a unique match).
- `nint Sharp.Shared.ILibraryModule.FindPtr(nint ptr)` [L:86]
  - Modifiers: public, abstract
  - Summary: Find the address in memory that contains a pointer to the specific value provided.
- `nint Sharp.Shared.ILibraryModule.FindString(string str)` [L:72]
  - Modifiers: public, abstract
  - Summary: Find address of the given string in the module's data section.
- `nint Sharp.Shared.ILibraryModule.FindStringExact(string str)` [L:80]
  - Modifiers: public, abstract
  - Summary: Find address of the given string in the module's data section.
- `nint Sharp.Shared.ILibraryModule.GetFunctionByName(string functionName)` [L:46]
  - Modifiers: public, abstract
  - Summary: Get exported function address (similar to GetProcAddress or dlsym).
- `nint Sharp.Shared.ILibraryModule.GetVirtualTableByName(string tableName, [bool decorated = false])` [L:40]
  - Modifiers: public, abstract
  - Summary: Find virtual table by name
- `nint[] Sharp.Shared.ILibraryModule.FindFunctions(System.ReadOnlySpan<nint> ptrs)` [L:157]
  - Modifiers: public, abstract
  - Summary: Finds all functions that reference the provided pointers.
- `nint[] Sharp.Shared.ILibraryModule.FindFunctions(System.ReadOnlySpan<string> strs)` [L:133]
  - Modifiers: public, abstract
  - Summary: Finds all functions that reference the provided string literals.
- `nint[] Sharp.Shared.ILibraryModule.FindFunctions(nint ptr)` [L:151]
  - Modifiers: public, abstract
  - Summary: Finds all functions that reference the specific pointer.
- `nint[] Sharp.Shared.ILibraryModule.FindFunctions(string str)` [L:127]
  - Modifiers: public, abstract
  - Summary: Finds all functions that reference the specific string literal.
- `nint[] Sharp.Shared.ILibraryModule.GetReferencesFromPointer(nint ptr)` [L:107]
  - Modifiers: public, abstract
  - Summary: Finds all references to the specified pointer within the module's executable code section (.text).


### interface IModSharp

- FullName: `Sharp.Shared.IModSharp`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/IModSharp.cs:36
- Generated: false

#### Methods
- `Sharp.Shared.Enums.ResourceStatus Sharp.Shared.IModSharp.GetResourceStatus(string filePath)` [L:305]
  - Modifiers: public, abstract
  - Summary: Get resource status
- `Sharp.Shared.GameObjects.IWeaponData? Sharp.Shared.IModSharp.FindWeaponVDataByName(string name)` [L:466]
  - Modifiers: public, abstract
  - Summary: Find weapon VData by name
- `Sharp.Shared.IGameData Sharp.Shared.IModSharp.GetGameData()` [L:68]
  - Modifiers: public, abstract
  - Summary: Get GameData
- `Sharp.Shared.ILibraryModule Sharp.Shared.IModSharp.GetLibraryModule(string module)` [L:431]
  - Modifiers: public, abstract
  - Summary: Get DLL/SO library module
- `Sharp.Shared.Objects.IGameRules Sharp.Shared.IModSharp.GetGameRules()` [L:88]
  - Modifiers: public, abstract
  - Summary: Get GameRules (not available in )
- `Sharp.Shared.Objects.IGameSystem? Sharp.Shared.IModSharp.FindGameSystemByName(string name)` [L:436]
  - Modifiers: public, abstract
  - Summary: Find GameSystem by name
- `Sharp.Shared.Objects.IGlobalVars Sharp.Shared.IModSharp.GetGlobals()` [L:73]
  - Modifiers: public, abstract
  - Summary: Get gpGlobals
- `Sharp.Shared.Objects.IKeyValues Sharp.Shared.IModSharp.CreateKeyValues(string name)` [L:421]
  - Modifiers: public, abstract
  - Summary: Create KeyValues
- `Sharp.Shared.Objects.IKeyValues3 Sharp.Shared.IModSharp.CreateKeyValues3(Sharp.Shared.Enums.KeyValues3Type type, Sharp.Shared.Enums.KeyValues3SubType subType)` [L:426]
  - Modifiers: public, abstract
  - Summary: Create KeyValues3
- `Sharp.Shared.Objects.IMemAlloc Sharp.Shared.IModSharp.GetMemAlloc()` [L:457]
  - Modifiers: public, abstract
  - Summary: Get memory allocator
- `Sharp.Shared.Objects.INetworkServer Sharp.Shared.IModSharp.GetIServer()` [L:78]
  - Modifiers: public, abstract
  - Summary: Get NetworkGameServer (sv)
- `Sharp.Shared.Objects.INetworkingStringTable? Sharp.Shared.IModSharp.FindStringTable(string name)` [L:408]
  - Modifiers: public, abstract
  - Summary: Find StringTable
- `Sharp.Shared.Objects.ISteamApi Sharp.Shared.IModSharp.GetSteamGameServer()` [L:93]
  - Modifiers: public, abstract
  - Summary: Get SteamApi SteamGameServer
- `System.Collections.Generic.List<(ulong PublishFileId, string Name)> Sharp.Shared.IModSharp.ListWorkshopMaps()` [L:508]
  - Modifiers: public, abstract
  - Summary: List all workshop maps added to the server's map list
- `System.Collections.Generic.List<string>? Sharp.Shared.IModSharp.GetMapGroupMapList(string mapGroup)` [L:290]
  - Modifiers: public, abstract
  - Summary: Get map list for given map group
- `System.Guid Sharp.Shared.IModSharp.PushTimer(System.Action action, double interval, [Sharp.Shared.Enums.GameTimerFlags flags = Sharp.Shared.Enums.GameTimerFlags.None])` [L:130]
  - Modifiers: public, abstract
  - Summary: Add timer to queue
- `System.Guid Sharp.Shared.IModSharp.PushTimer(System.Func<Sharp.Shared.Enums.TimerAction> action, double interval, [Sharp.Shared.Enums.GameTimerFlags flags = Sharp.Shared.Enums.GameTimerFlags.None])` [L:135]
  - Modifiers: public, abstract
  - Summary: Add timer to queue
- `System.Threading.Tasks.Task Sharp.Shared.IModSharp.InvokeFrameActionAsync(System.Action action, [System.Threading.CancellationToken cancellationToken = default(System.Threading.CancellationToken)])` [L:125]
  - Modifiers: public, abstract
  - Summary: Invoke action at the end of current frame and wait
- `System.Threading.Tasks.Task<T> Sharp.Shared.IModSharp.InvokeFrameActionAsync<T>(System.Func<T> action, [System.Threading.CancellationToken cancellationToken = default(System.Threading.CancellationToken)])` [L:120]
  - Modifiers: public, abstract
  - Summary: Invoke action at the end of current frame and wait
- `T? Sharp.Shared.IModSharp.CreateNativeObject<T>(nint ptr) where T : class, Sharp.Shared.CStrike.INativeObject` [L:387]
  - Modifiers: public, abstract
  - Summary: Create native object from pointer
- `T? Sharp.Shared.IModSharp.GetCommandLine<T>(string key) where T : System.IParsable<T>` [L:263]
  - Modifiers: public, abstract
  - Summary: Get value for a specific command line argument
- `bool Sharp.Shared.IModSharp.AddWorkshopMap(ulong sharedFileId, string mapName, string path)` [L:492]
  - Modifiers: public, abstract
  - Summary: Add a workshop map to the server's map list
- `bool Sharp.Shared.IModSharp.HasCommandLine(string key)` [L:258]
  - Modifiers: public, abstract
  - Summary: Check if the command line argument exists
- `bool Sharp.Shared.IModSharp.IsMapValid(string map)` [L:283]
  - Modifiers: public, abstract
  - Summary: Check if map is valid
- `bool Sharp.Shared.IModSharp.IsValidTimer(System.Guid uniqueId)` [L:145]
  - Modifiers: public, abstract
  - Summary: Check if timer is in queue
- `bool Sharp.Shared.IModSharp.RemoveWorkshopMap(ulong sharedFileId)` [L:503]
  - Modifiers: public, abstract
  - Summary: Remove map from dedicate server workshop manager
- `bool Sharp.Shared.IModSharp.SendNetMessage<T>(Sharp.Shared.Types.RecipientFilter filter, T data) where T : class, Google.Protobuf.IMessage` [L:238]
  - Modifiers: public, abstract
  - Summary: Send NetMessage
- `bool Sharp.Shared.IModSharp.SetMemoryAccess(nint pMemory, long size, Sharp.Shared.Enums.MemoryAccess access)` [L:446]
  - Modifiers: public, abstract
  - Summary: Set protected memory access
- `bool Sharp.Shared.IModSharp.SetMemoryAccess(nint pMemory, long size, Sharp.Shared.Enums.MemoryAccess access, out Sharp.Shared.Enums.MemoryAccess originalAccess)` [L:451]
  - Modifiers: public, abstract
  - Summary: Set protected memory access
- `bool Sharp.Shared.IModSharp.WorkshopMapExists(ulong sharedFileId)` [L:497]
  - Modifiers: public, abstract
  - Summary: Is map loaded by dedicate server workshop manager
- `byte[]? Sharp.Shared.IModSharp.FindResourceDataBlockInfo(string filePath, string pathId)` [L:298]
  - Modifiers: public, abstract
  - Summary: Read game resource data buffer
- `double Sharp.Shared.IModSharp.EngineTime()` [L:104]
  - Modifiers: public, abstract
  - Summary: Plat_FloatTime, also Source 1's EngineTime
- `int Sharp.Shared.IModSharp.DispatchParticleEffect(string particle, Sharp.Shared.Enums.ParticleAttachmentType attachType, Sharp.Shared.GameEntities.IBaseEntity entity, [byte attachmentIndex = 0], [bool resetEntity = false], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:347]
  - Modifiers: public, abstract
  - Summary: Dispatches a particle effect attached to a specific point on an entity
- `int Sharp.Shared.IModSharp.DispatchParticleEffect(string particle, Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.Types.Vector origin, Sharp.Shared.Types.Vector angles, [bool resetEntity = false], [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:337]
  - Modifiers: public, abstract
  - Summary: Dispatches a particle effect relative to an entity
- `int Sharp.Shared.IModSharp.DispatchParticleEffect(string particle, Sharp.Shared.Types.Vector origin, Sharp.Shared.Types.Vector angles, [Sharp.Shared.Types.RecipientFilter filter = default(Sharp.Shared.Types.RecipientFilter)])` [L:332]
  - Modifiers: public, abstract
  - Summary: Dispatches a particle effect at a specific world location
- `nint Sharp.Shared.IModSharp.FindPattern(string module, string pattern)` [L:394]
  - Modifiers: public, abstract
  - Summary: Find pattern in module, invalid module will cause FatalError
- `nint Sharp.Shared.IModSharp.FindValveInterface(string module, string name)` [L:441]
  - Modifiers: public, abstract
  - Summary: Find Valve interface
- `nint Sharp.Shared.IModSharp.GetIEngine()` [L:83]
  - Modifiers: public, abstract
  - Summary: Get Engine2Server (engine)
- `nint Sharp.Shared.IModSharp.GetNativeFunctionPointer(string name)` [L:99]
  - Modifiers: public, abstract
  - Summary: Get NativeFunction
- `nint Sharp.Shared.IModSharp.GetVirtualTableByClass(string module, string className)` [L:416]
  - Modifiers: public, abstract
  - Summary: Get virtual table for specified C++ class
- `string Sharp.Shared.IModSharp.GetGamePath()` [L:150]
  - Modifiers: public, abstract
  - Summary: Get game absolute path
- `string? Sharp.Shared.IModSharp.GetAddonName()` [L:317]
  - Modifiers: public, abstract
  - Summary: Get currently loaded addon IDs
- `string? Sharp.Shared.IModSharp.GetCommandLine(string key)` [L:268]
  - Modifiers: public, abstract
  - Summary: Get command line argument value as string
- `string? Sharp.Shared.IModSharp.GetMapName()` [L:323]
  - Modifiers: public, abstract
  - Summary: Get map BSP name, e.g. de_mirage, surf_beginner
- `uint Sharp.Shared.IModSharp.MakeStringToken(string str)` [L:188]
  - Modifiers: public, abstract
  - Summary: Returns the MurmurHash2 value of the given string, case-insensitive
- `void Sharp.Shared.IModSharp.ChangeLevel(string map)` [L:278]
  - Modifiers: public, abstract
  - Summary: Change map
- `void Sharp.Shared.IModSharp.DualAddonOverrideCheck(Sharp.Shared.Units.SteamID steamId, double time)` [L:480]
  - Modifiers: public, abstract
  - Summary: Override cache for a player
- `void Sharp.Shared.IModSharp.DualAddonPurgeCheck()` [L:475]
  - Modifiers: public, abstract
  - Summary: Clear dual addon cache
- `void Sharp.Shared.IModSharp.FatalError(string message)` [L:62]
  - Modifiers: public, abstract
  - Summary: Engine error
- `void Sharp.Shared.IModSharp.HookNetMessage(Sharp.Shared.Enums.ProtobufNetMessageType msgId)` [L:243]
  - Modifiers: public, abstract
  - Summary: Install HookNetMessage
- `void Sharp.Shared.IModSharp.InstallEntityThinkHook(System.Action? pre, System.Action? post, [int prePriority = 0], [int postPriority = 0])` [L:163]
  - Modifiers: public, abstract
  - Summary: Install EntityThink Hook
- `void Sharp.Shared.IModSharp.InstallGameFrameHook(System.Action<bool, bool, bool>? pre, System.Action<bool, bool, bool>? post, [int prePriority = 0], [int postPriority = 0])` [L:155]
  - Modifiers: public, abstract
  - Summary: Install GameFrame Hook
- `void Sharp.Shared.IModSharp.InstallGameListener(Sharp.Shared.Listeners.IGameListener listener)` [L:361]
  - Modifiers: public, abstract
  - Summary: Install  to listen for game events
- `void Sharp.Shared.IModSharp.InstallServerGameSimulateHook(System.Action callback, [int priority = 0])` [L:168]
  - Modifiers: public, abstract
  - Summary: Install ServerGameSimulate Hook
- `void Sharp.Shared.IModSharp.InstallSteamListener(Sharp.Shared.Listeners.ISteamListener listener)` [L:371]
  - Modifiers: public, abstract
  - Summary: Install  to listen for Steam events
- `void Sharp.Shared.IModSharp.InvokeAction(System.Action action)` [L:110]
  - Modifiers: public, abstract
  - Summary: Invoke action on main thread If currently on main thread, calls immediately, otherwise calls at end of current frame
- `void Sharp.Shared.IModSharp.InvokeFrameAction(System.Action action)` [L:115]
  - Modifiers: public, abstract
  - Summary: Invoke action at the end of current frame
- `void Sharp.Shared.IModSharp.LogColorText(Sharp.Shared.Types.Color color, string text)` [L:53]
  - Modifiers: public, abstract
  - Summary: Print log (custom color)
- `void Sharp.Shared.IModSharp.LogMessage(string message)` [L:43]
  - Modifiers: public, abstract
  - Summary: Print log (Info)
- `void Sharp.Shared.IModSharp.LogWarning(string message)` [L:48]
  - Modifiers: public, abstract
  - Summary: Print log (Warning)
- `void Sharp.Shared.IModSharp.PrecacheResource(string resource)` [L:273]
  - Modifiers: public, abstract
  - Summary: Precache resource
- `void Sharp.Shared.IModSharp.PrintChannelAll(Sharp.Shared.Enums.HudPrintChannel channel, string message)` [L:207]
  - Modifiers: public, abstract
  - Summary: Send message to all players on specified channel
- `void Sharp.Shared.IModSharp.PrintChannelFilter(Sharp.Shared.Enums.HudPrintChannel channel, string message, Sharp.Shared.Types.RecipientFilter receiver)` [L:212]
  - Modifiers: public, abstract
  - Summary: Send message to filtered players on specified channel
- `void Sharp.Shared.IModSharp.PrintChannelTeam(Sharp.Shared.Enums.HudPrintChannel channel, Sharp.Shared.Enums.CStrikeTeam team, string message)` [L:217]
  - Modifiers: public, abstract
  - Summary: Send message to team players on specified channel
- `void Sharp.Shared.IModSharp.PrintToChat(Sharp.Shared.Enums.CStrikeTeam team, string message)` [L:202]
  - Modifiers: public, abstract
  - Summary: Send chat message to specific team
- `void Sharp.Shared.IModSharp.PrintToChatAll(string message)` [L:197]
  - Modifiers: public, abstract
  - Summary: Send chat message to all players
- `void Sharp.Shared.IModSharp.RadioTextAll(Sharp.Shared.Units.PlayerSlot slot, string name, string? params1, string? params2, string? params3, string? params4)` [L:233]
  - Modifiers: public, abstract
  - Summary: Radio message
- `void Sharp.Shared.IModSharp.RadioTextTeam(Sharp.Shared.Enums.CStrikeTeam team, Sharp.Shared.Units.PlayerSlot slot, string name, string? params1, string? params2, string? params3, string? params4)` [L:222]
  - Modifiers: public, abstract
  - Summary: Radio message (Team)
- `void Sharp.Shared.IModSharp.RemoveEntityThinkHook(System.Action? pre, System.Action? post)` [L:178]
  - Modifiers: public, abstract
  - Summary: Remove EntityThink Hook
- `void Sharp.Shared.IModSharp.RemoveGameFrameHook(System.Action<bool, bool, bool>? pre, System.Action<bool, bool, bool>? post)` [L:173]
  - Modifiers: public, abstract
  - Summary: Remove GameFrame Hook
- `void Sharp.Shared.IModSharp.RemoveGameListener(Sharp.Shared.Listeners.IGameListener listener)` [L:366]
  - Modifiers: public, abstract
  - Summary: Remove
- `void Sharp.Shared.IModSharp.RemoveServerGameSimulateHook(System.Action callback)` [L:183]
  - Modifiers: public, abstract
  - Summary: Remove ServerGameSimulate Hook
- `void Sharp.Shared.IModSharp.RemoveSteamListener(Sharp.Shared.Listeners.ISteamListener listener)` [L:376]
  - Modifiers: public, abstract
  - Summary: Remove
- `void Sharp.Shared.IModSharp.ServerCommand(string command)` [L:311]
  - Modifiers: public, abstract
  - Summary: Execute server command
- `void Sharp.Shared.IModSharp.StopTimer(System.Guid uniqueId)` [L:140]
  - Modifiers: public, abstract
  - Summary: Remove timer from queue

#### Obsolete Members
- `nint Sharp.Shared.IModSharp.GetVTableByClass(string module, string className)` [L:403] — Renamed to GetVirtualTableByClass, will be removed in the future
- `void Sharp.Shared.IModSharp.UnhookNetMessage(Sharp.Shared.Enums.ProtobufNetMessageType msgId)` [L:249] — This is deprecated and do nothing, will be removed in 2.2


### interface IModSharpModule

- FullName: `Sharp.Shared.IModSharpModule`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/IModSharpModule.cs:27
- Generated: false
- Summary: Module Interface the constructor must bepublic YourModule(ISharedSystem sharedSystem, string dllPath, string sharpPath, Version version, IConfiguration coreConfiguration, bool hotReload)

#### Properties
- `string Sharp.Shared.IModSharpModule.DisplayAuthor` [L:30]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.IModSharpModule.DisplayName` [L:29]
  - Modifiers: public, abstract, readonly

#### Methods
- `bool Sharp.Shared.IModSharpModule.Init()` [L:35]
  - Modifiers: public, abstract
  - Summary: Load
- `void Sharp.Shared.IModSharpModule.OnAllModulesLoaded()` [L:81]
  - Modifiers: public, virtual
  - Summary: Called after all modules loaded
- `void Sharp.Shared.IModSharpModule.OnLibraryConnected(string name)` [L:63]
  - Modifiers: public, virtual
  - Summary: Called after modules loaded, this does not call for the current module itself.
- `void Sharp.Shared.IModSharpModule.OnLibraryDisconnect(string name)` [L:74]
  - Modifiers: public, virtual
  - Summary: Called before library unloaded, this does not call for the current module itself
- `void Sharp.Shared.IModSharpModule.PostInit()` [L:41]
  - Modifiers: public, virtual
  - Summary: Post Load Safe to register dynamic native or shared interface here
- `void Sharp.Shared.IModSharpModule.Shutdown()` [L:48]
  - Modifiers: public, abstract
  - Summary: Shutdown


### interface IModSharpModuleInterface<T>

- FullName: `Sharp.Shared.IModSharpModuleInterface<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/IModSharpModule.cs:86
- Generated: false
- Constraint: `where T : class`

#### Properties
- `T? Sharp.Shared.IModSharpModuleInterface<out T>.Instance` [L:102]
  - Modifiers: public, abstract, readonly
  - Summary: Instance of this interface null if interface no more available
- `bool Sharp.Shared.IModSharpModuleInterface<out T>.IsAvailable` [L:91]
  - Modifiers: public, virtual, readonly
  - Summary: Is the interface available, safe to use
- `string Sharp.Shared.IModSharpModuleInterface<out T>.Identity` [L:96]
  - Modifiers: public, abstract, readonly
  - Summary: Identity of this interface


### interface ISharedSystem

- FullName: `Sharp.Shared.ISharedSystem`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/ISharedSystem.cs:25
- Generated: false

#### Methods
- `Microsoft.Extensions.Logging.ILoggerFactory Sharp.Shared.ISharedSystem.GetLoggerFactory()` [L:39]
  - Modifiers: public, abstract
- `Sharp.Shared.IModSharp Sharp.Shared.ISharedSystem.GetModSharp()` [L:37]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IClientManager Sharp.Shared.ISharedSystem.GetClientManager()` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IConVarManager Sharp.Shared.ISharedSystem.GetConVarManager()` [L:33]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IEconItemManager Sharp.Shared.ISharedSystem.GetEconItemManager()` [L:47]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IEntityManager Sharp.Shared.ISharedSystem.GetEntityManager()` [L:27]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IEventManager Sharp.Shared.ISharedSystem.GetEventManager()` [L:31]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IFileManager Sharp.Shared.ISharedSystem.GetFileManager()` [L:43]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IHookManager Sharp.Shared.ISharedSystem.GetHookManager()` [L:35]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.ILibraryModuleManager Sharp.Shared.ISharedSystem.GetLibraryModuleManager()` [L:49]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IParticleManager Sharp.Shared.ISharedSystem.GetParticleManager()` [L:57]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.IPhysicsQueryManager Sharp.Shared.ISharedSystem.GetPhysicsQueryManager()` [L:53]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.ISchemaManager Sharp.Shared.ISharedSystem.GetSchemaManager()` [L:45]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.ISharpModuleManager Sharp.Shared.ISharedSystem.GetSharpModuleManager()` [L:55]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.ISoundManager Sharp.Shared.ISharedSystem.GetSoundManager()` [L:51]
  - Modifiers: public, abstract
- `Sharp.Shared.Managers.ITransmitManager Sharp.Shared.ISharedSystem.GetTransmitManager()` [L:41]
  - Modifiers: public, abstract


### class MemoryAllocator

- FullName: `Sharp.Shared.MemoryAllocator`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/MemoryAllocator.cs:49
- Generated: false
- Summary: Provides direct access to the Source Engine's internal memory allocator.

Inheritance: object → **MemoryAllocator**

#### Methods
- `static nuint Sharp.Shared.MemoryAllocator.GetSize(void* ptr)` [L:96]
  - Modifiers: public, static
  - Summary: Gets the size of a memory block allocated on the native game heap.
- `static void Sharp.Shared.MemoryAllocator.Free(void* ptr)` [L:90]
  - Modifiers: public, static
  - Summary: Frees a memory block previously allocated by  or .
- `static void Sharp.Shared.MemoryAllocator.MemMove(void* dest, void* src, nuint count)` [L:102]
  - Modifiers: public, static
  - Summary: Copies bytes from a source to a destination. Handles overlapping memory regions correctly.
- `static void* Sharp.Shared.MemoryAllocator.Alloc(nuint size)` [L:74]
  - Modifiers: public, static
  - Summary: Allocates a block of memory on the native game heap.
- `static void* Sharp.Shared.MemoryAllocator.Realloc(void* ptr, nuint size)` [L:83]
  - Modifiers: public, static
  - Summary: Reallocates a block of memory on the native game heap, preserving its content.
- `static void* Sharp.Shared.MemoryAllocator.VectorMemory_Alloc(void* pMem, bool bRealloc, int nNewSize, int nOldSize)` [L:110]
  - Modifiers: public, static
  - Summary: Internal allocator used specifically for Source Engine's  growth strategy.


### record SchemaClass : System.IEquatable<Sharp.Shared.SchemaClass>

- FullName: `Sharp.Shared.SchemaClass`
- Kind: record
- Modifiers: public
- Source: Sharp.Shared/SharedGameObject.cs:28
- Generated: false

Inheritance: object → **SchemaClass**

#### Properties
- `required System.Collections.Frozen.FrozenDictionary<string, Sharp.Shared.SchemaClassField> Sharp.Shared.SchemaClass.Fields` [L:34]
- `required System.Collections.Generic.List<Sharp.Shared.DataMapField> Sharp.Shared.SchemaClass.DataMapFields` [L:36]
- `required System.Collections.Generic.List<string> Sharp.Shared.SchemaClass.BaseClasses` [L:35]
- `required byte Sharp.Shared.SchemaClass.AlignOf` [L:33]
- `required int Sharp.Shared.SchemaClass.Size` [L:32]
- `required string Sharp.Shared.SchemaClass.ClassName` [L:30]
- `required ushort Sharp.Shared.SchemaClass.ChainOffset` [L:31]


### record SchemaClassField : System.IEquatable<Sharp.Shared.SchemaClassField>

- FullName: `Sharp.Shared.SchemaClassField`
- Kind: record
- Modifiers: public
- Source: Sharp.Shared/SharedGameObject.cs:39
- Generated: false

Inheritance: object → **SchemaClassField**

#### Properties
- `required Sharp.Shared.Enums.SchemaTypeCategory Sharp.Shared.SchemaClassField.Category` [L:45]
- `required bool Sharp.Shared.SchemaClassField.IsArray` [L:44]
- `required bool Sharp.Shared.SchemaClassField.Networked` [L:42]
- `required int Sharp.Shared.SchemaClassField.Offset` [L:41]
- `required string Sharp.Shared.SchemaClassField.Type` [L:43]


### record SchemaField : System.IEquatable<Sharp.Shared.SchemaField>

- FullName: `Sharp.Shared.SchemaField`
- Kind: record
- Modifiers: public
- Source: Sharp.Shared/SharedGameObject.cs:56
- Generated: false

Inheritance: object → **SchemaField**

#### Properties
- `bool Sharp.Shared.SchemaField.Networked` [L:59]
- `int Sharp.Shared.SchemaField.ArraySize` [L:61]
- `int Sharp.Shared.SchemaField.ChainOffset` [L:60]
- `int Sharp.Shared.SchemaField.Offset` [L:58]


### class SharedGameObject

- FullName: `Sharp.Shared.SharedGameObject`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/SharedGameObject.cs:68
- Generated: false
- Summary: Do not modify anything here if you don't know what you're doing Modifying can lead to unexpected results

Inheritance: object → **SharedGameObject**

#### Fields
- `static System.Collections.Frozen.FrozenDictionary<string, Sharp.Shared.GameObjects.IEconItemDefinition> Sharp.Shared.SharedGameObject.EconItemDefinitionsByName` [L:72]
  - Modifiers: public, static
- `static System.Collections.Frozen.FrozenDictionary<string, Sharp.Shared.SchemaClass> Sharp.Shared.SharedGameObject.SchemaInfo` [L:70]
  - Modifiers: public, static
- `static System.Collections.Frozen.FrozenDictionary<uint, Sharp.Shared.GameObjects.IPaintKit> Sharp.Shared.SharedGameObject.PaintKits` [L:73]
  - Modifiers: public, static
- `static System.Collections.Frozen.FrozenDictionary<ushort, Sharp.Shared.GameObjects.IEconItemDefinition> Sharp.Shared.SharedGameObject.EconItemDefinitionsById` [L:71]
  - Modifiers: public, static


