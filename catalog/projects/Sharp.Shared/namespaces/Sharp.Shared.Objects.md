# Sharp.Shared.Objects

Project: Sharp.Shared
Types: 15 (0 generated)

### interface IAdmin

- FullName: `Sharp.Shared.Objects.IAdmin`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IAdmin.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Units.SteamID Sharp.Shared.Objects.IAdmin.Identity` [L:35]
  - Modifiers: public, abstract, readonly
  - Summary: Steam ID
- `System.Collections.Generic.IReadOnlySet<string> Sharp.Shared.Objects.IAdmin.Permissions` [L:45]
  - Modifiers: public, abstract, readonly
  - Summary: Set of permissions
- `byte Sharp.Shared.Objects.IAdmin.Immunity` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: Immunity level
- `string Sharp.Shared.Objects.IAdmin.Name` [L:30]
  - Modifiers: public, abstract, readonly
  - Summary: Administrator name

#### Methods
- `bool Sharp.Shared.Objects.IAdmin.AddPermission(string permission)` [L:59]
  - Modifiers: public, abstract
  - Summary: Add permission to admin
- `bool Sharp.Shared.Objects.IAdmin.HasPermission(string permission)` [L:52]
  - Modifiers: public, abstract
  - Summary: Check if admin has specific permission
- `bool Sharp.Shared.Objects.IAdmin.RemovePermission(string permission)` [L:66]
  - Modifiers: public, abstract
  - Summary: Remove permission from admin


### interface IConVar : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IConVar`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IConVar.cs:30
- Generated: false

#### Properties
- `Sharp.Shared.Enums.ConVarFlags Sharp.Shared.Objects.IConVar.Flags` [L:50]
  - Modifiers: public, abstract
  - Summary: ConVar flags
- `Sharp.Shared.Enums.ConVarType Sharp.Shared.Objects.IConVar.Type` [L:55]
  - Modifiers: public, abstract, readonly
  - Summary: ConVar value type
- `string Sharp.Shared.Objects.IConVar.DefaultValue` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: Default value
- `string Sharp.Shared.Objects.IConVar.HelpString` [L:45]
  - Modifiers: public, abstract, readonly
  - Summary: Help description text
- `string Sharp.Shared.Objects.IConVar.Name` [L:35]
  - Modifiers: public, abstract, readonly
  - Summary: ConVar name

#### Methods
- `bool Sharp.Shared.Objects.IConVar.GetBool()` [L:57]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IConVar.SetMaxBound(Sharp.Shared.Types.ConVarVariantValue value)` [L:89]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IConVar.SetMinBound(Sharp.Shared.Types.ConVarVariantValue value)` [L:87]
  - Modifiers: public, abstract
- `double Sharp.Shared.Objects.IConVar.GetDouble()` [L:73]
  - Modifiers: public, abstract
- `float Sharp.Shared.Objects.IConVar.GetFloat()` [L:71]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.IConVar.GetInt32()` [L:63]
  - Modifiers: public, abstract
- `long Sharp.Shared.Objects.IConVar.GetInt64()` [L:67]
  - Modifiers: public, abstract
- `ref Sharp.Shared.Types.ConVarVariantValue Sharp.Shared.Objects.IConVar.Get()` [L:75]
  - Modifiers: public, abstract
- `short Sharp.Shared.Objects.IConVar.GetInt16()` [L:59]
  - Modifiers: public, abstract
- `string Sharp.Shared.Objects.IConVar.GetString()` [L:108]
  - Modifiers: public, abstract
  - Summary: Returns the ConVar value as a string.
- `uint Sharp.Shared.Objects.IConVar.GetUInt32()` [L:65]
  - Modifiers: public, abstract
- `ulong Sharp.Shared.Objects.IConVar.GetUInt64()` [L:69]
  - Modifiers: public, abstract
- `ushort Sharp.Shared.Objects.IConVar.GetUInt16()` [L:61]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.ReplicateToClient(Sharp.Shared.Objects.IGameClient client, string value)` [L:115]
  - Modifiers: public, abstract
  - Summary: Sends the specified value to the client without changing the server-side ConVar.
- `void Sharp.Shared.Objects.IConVar.Set(Sharp.Shared.Types.ConVarVariantValue value)` [L:85]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.Set(bool value)` [L:79]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.Set(float value)` [L:81]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.Set(int value)` [L:77]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.Set(string value)` [L:83]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IConVar.SetString(string value)` [L:102]
  - Modifiers: public, abstract
  - Summary: Universal method to set the ConVar value by parsing a string.


### interface IGameClient : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IGameClient`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IGameClient.cs:31
- Generated: false

#### Properties
- `Sharp.Shared.Enums.SignOnState Sharp.Shared.Objects.IGameClient.SignOnState` [L:118]
  - Modifiers: public, abstract, readonly
  - Summary: Client sign-on state
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.Objects.IGameClient.ControllerIndex` [L:148]
  - Modifiers: public, abstract, readonly
  - Summary: Controller entity index
- `Sharp.Shared.Units.PlayerSlot Sharp.Shared.Objects.IGameClient.Slot` [L:143]
  - Modifiers: public, abstract, readonly
  - Summary: Client engine slot (PlayerSlot)
- `Sharp.Shared.Units.SteamID Sharp.Shared.Objects.IGameClient.SteamId` [L:138]
  - Modifiers: public, abstract, readonly
  - Summary: Steam ID (64-bit)
- `Sharp.Shared.Units.UserID Sharp.Shared.Objects.IGameClient.UserId` [L:133]
  - Modifiers: public, abstract, readonly
  - Summary: User ID
- `bool Sharp.Shared.Objects.IGameClient.IsAuthenticated` [L:163]
  - Modifiers: public, abstract, readonly
  - Summary: Whether Steam ID has been authenticated by Steam servers
- `bool Sharp.Shared.Objects.IGameClient.IsConnected` [L:173]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this client is connected
- `bool Sharp.Shared.Objects.IGameClient.IsFakeClient` [L:123]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this is a fake client
- `bool Sharp.Shared.Objects.IGameClient.IsHltv` [L:128]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this is HLTV
- `bool Sharp.Shared.Objects.IGameClient.IsInGame` [L:178]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this client is in-game
- `bool Sharp.Shared.Objects.IGameClient.IsValid` [L:168]
  - Modifiers: public, abstract, readonly
  - Summary: Whether this client pointer is valid
- `bool Sharp.Shared.Objects.IGameClient.PerfectWorld` [L:158]
  - Modifiers: public, abstract, readonly
  - Summary: Whether client is Perfect World user or has low violence mode enabled
- `float Sharp.Shared.Objects.IGameClient.TimeConnected` [L:185]
  - Modifiers: public, abstract, readonly
  - Summary: For players: time since joining server (persists across map changes)For bots/HLTV: always returns server uptime
- `string Sharp.Shared.Objects.IGameClient.Name` [L:153]
  - Modifiers: public, abstract, readonly
  - Summary: Player name
- `string? Sharp.Shared.Objects.IGameClient.Address` [L:191]
  - Modifiers: public, abstract, readonly
  - Summary: Client IP address and port Always null for bots/HLTV

#### Methods
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.Objects.IGameClient.GetPlayerController()` [L:95]
  - Modifiers: public, abstract
  - Summary: Get
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IGameClient.GetConVars()` [L:87]
  - Modifiers: public, abstract
  - Summary: Get client ConVars as KeyValues object
- `bool Sharp.Shared.Objects.IGameClient.Equals(object? obj)` [L:195]
  - Modifiers: public, abstract
- `float Sharp.Shared.Objects.IGameClient.GetTimeConnected()` [L:57]
  - Modifiers: public, abstract
  - Summary: Get time since client connected
- `int Sharp.Shared.Objects.IGameClient.GetHashCode()` [L:193]
  - Modifiers: public, abstract
- `string? Sharp.Shared.Objects.IGameClient.GetAddress(bool withPort)` [L:52]
  - Modifiers: public, abstract
  - Summary: Get client IP address
- `string? Sharp.Shared.Objects.IGameClient.GetConVarValue(string cvarName)` [L:82]
  - Modifiers: public, abstract
  - Summary: Get client info ConVar value
- `void Sharp.Shared.Objects.IGameClient.Command(string command)` [L:62]
  - Modifiers: public, abstract
  - Summary: Execute command (via Client/NetChannel)
- `void Sharp.Shared.Objects.IGameClient.ConsolePrint(string message)` [L:36]
  - Modifiers: public, abstract
  - Summary: Print message to client console
- `void Sharp.Shared.Objects.IGameClient.ExecuteStringCommand(string command)` [L:72]
  - Modifiers: public, abstract
  - Summary: Execute command (via Engine)
- `void Sharp.Shared.Objects.IGameClient.FakeCommand(string command)` [L:67]
  - Modifiers: public, abstract
  - Summary: Execute command (via GameClients)
- `void Sharp.Shared.Objects.IGameClient.ForceFullUpdate()` [L:77]
  - Modifiers: public, abstract
  - Summary: Force send full update to client
- `void Sharp.Shared.Objects.IGameClient.Print(Sharp.Shared.Enums.HudPrintChannel channel, string message, [string? param1 = null], [string? param2 = null], [string? param3 = null], [string? param4 = null])` [L:100]
  - Modifiers: public, abstract
  - Summary: Print message to this player
- `void Sharp.Shared.Objects.IGameClient.PrintCenterHtml(string message, [int duration = 1])` [L:113]
  - Modifiers: public, abstract
  - Summary: Print a hud message with limited html format support to this player.
- `void Sharp.Shared.Objects.IGameClient.SayChatMessage(bool teamOnly, string message)` [L:46]
  - Modifiers: public, abstract
  - Summary: Send chat message as this client
- `void Sharp.Shared.Objects.IGameClient.SetName(string name)` [L:41]
  - Modifiers: public, abstract
  - Summary: Override player's in-game name


### interface IGameEvent : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IGameEvent`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IGameEvent.cs:30
- Generated: false

#### Properties
- `bool Sharp.Shared.Objects.IGameEvent.Editable` [L:213]
  - Modifiers: public, abstract, readonly
  - Summary: Whether event can be modified or fired
- `string Sharp.Shared.Objects.IGameEvent.Name` [L:208]
  - Modifiers: public, abstract, readonly
  - Summary: Event name

#### Indexers
- `object Sharp.Shared.Objects.IGameEvent.this[string key]` [L:218]
  - Modifiers: public, abstract
  - Summary: Set value using indexer

#### Methods
- `Sharp.Shared.GameEntities.IBasePlayerPawn? Sharp.Shared.Objects.IGameEvent.GetBasePlayerPawn(string key)` [L:113]
  - Modifiers: public, abstract
  - Summary: Get BasePlayerPawn, matches original game behavior
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.Objects.IGameEvent.GetPlayerController(string key)` [L:100]
  - Modifiers: public, abstract
  - Summary: Get event field as PlayerController
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.Objects.IGameEvent.GetPlayerPawn(string key)` [L:108]
  - Modifiers: public, abstract
  - Summary: Get event field as PlayerPawn
- `T Sharp.Shared.Objects.IGameEvent.Get<T>(string key, [int defaultValue = 0]) where T : System.Enum` [L:223]
  - Modifiers: public, abstract
  - Summary: Get event value and convert to enum
- `bool Sharp.Shared.Objects.IGameEvent.GetBool(string key)` [L:75]
  - Modifiers: public, abstract
  - Summary: Get event field as boolean value
- `float Sharp.Shared.Objects.IGameEvent.GetFloat(string key, [float defaultValue = 0])` [L:85]
  - Modifiers: public, abstract
  - Summary: Get event field as float value
- `int Sharp.Shared.Objects.IGameEvent.GetInt(string key, [int defaultValue = 0])` [L:90]
  - Modifiers: public, abstract
  - Summary: Get event field as integer value
- `string Sharp.Shared.Objects.IGameEvent.GetName()` [L:119]
  - Modifiers: public, abstract
  - Summary: Get event name
- `string Sharp.Shared.Objects.IGameEvent.GetString(string key, [string defaultValue = ""])` [L:80]
  - Modifiers: public, abstract
  - Summary: Get event field as string value
- `ulong Sharp.Shared.Objects.IGameEvent.GetUInt64(string key, [ulong defaultValue = 0])` [L:95]
  - Modifiers: public, abstract
  - Summary: Get event field as 64-bit unsigned integer value
- `void Sharp.Shared.Objects.IGameEvent.Dispose()` [L:203]
  - Modifiers: public, abstract
  - Summary: Manually dispose of the event object.
- `void Sharp.Shared.Objects.IGameEvent.Fire(bool serverOnly)` [L:137]
  - Modifiers: public, abstract
  - Summary: Fire the event.
- `void Sharp.Shared.Objects.IGameEvent.FireToClient(Sharp.Shared.Objects.IGameClient client)` [L:169]
  - Modifiers: public, abstract
  - Summary: Fire the event to a specific client.
- `void Sharp.Shared.Objects.IGameEvent.FireToClient(int slot)` [L:153]
  - Modifiers: public, abstract
  - Summary: Fire the event to a specific client identified by their slot index.
- `void Sharp.Shared.Objects.IGameEvent.FireToClients()` [L:184]
  - Modifiers: public, abstract
  - Summary: Fire the event to all connected clients.
- `void Sharp.Shared.Objects.IGameEvent.SetBool(string key, bool value)` [L:70]
  - Modifiers: public, abstract
  - Summary: Set event field to boolean value
- `void Sharp.Shared.Objects.IGameEvent.SetFloat(string key, float value)` [L:40]
  - Modifiers: public, abstract
  - Summary: Set event field to float value
- `void Sharp.Shared.Objects.IGameEvent.SetInt(string key, int value)` [L:45]
  - Modifiers: public, abstract
  - Summary: Set event field to integer value
- `void Sharp.Shared.Objects.IGameEvent.SetPlayer(string key, Sharp.Shared.GameEntities.IPlayerController controller)` [L:55]
  - Modifiers: public, abstract
  - Summary: Set event field to player controller
- `void Sharp.Shared.Objects.IGameEvent.SetPlayer(string key, Sharp.Shared.GameEntities.IPlayerPawn pawn)` [L:60]
  - Modifiers: public, abstract
  - Summary: Set event field to player pawn
- `void Sharp.Shared.Objects.IGameEvent.SetPlayer(string key, int slot)` [L:65]
  - Modifiers: public, abstract
  - Summary: Set event field to player by slot
- `void Sharp.Shared.Objects.IGameEvent.SetString(string key, string value)` [L:35]
  - Modifiers: public, abstract
  - Summary: Set event field to string value
- `void Sharp.Shared.Objects.IGameEvent.SetUInt64(string key, ulong value)` [L:50]
  - Modifiers: public, abstract
  - Summary: Set event field to 64-bit unsigned integer value


### interface IGameRules : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.Objects.IGameRules`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IGameRules.cs:30
- Generated: false

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.Objects.IGameRules.RoundWinStatus` [L:170]
  - Modifiers: public, abstract, readonly
  - Summary: Team that won the round
- `Sharp.Shared.Enums.GamePhase Sharp.Shared.Objects.IGameRules.GamePhase` [L:75]
  - Modifiers: public, abstract, readonly
  - Summary: Current game phase
- `Sharp.Shared.Enums.RoundEndReason Sharp.Shared.Objects.IGameRules.RoundWinReason` [L:165]
  - Modifiers: public, abstract, readonly
  - Summary: Reason for round end
- `bool Sharp.Shared.Objects.IGameRules.ForceTeamChangeSilent` [L:70]
  - Modifiers: public, abstract
  - Summary: Force team change without message
- `bool Sharp.Shared.Objects.IGameRules.IsForceTeamChangeSilent` [L:135]
  - Modifiers: public, abstract, readonly
  - Summary: Hide team selection messages
- `bool Sharp.Shared.Objects.IGameRules.IsFreezePeriod` [L:80]
  - Modifiers: public, abstract, readonly
  - Summary: Whether in freeze period
- `bool Sharp.Shared.Objects.IGameRules.IsGamePaused` [L:90]
  - Modifiers: public, abstract, readonly
  - Summary: Whether game is paused
- `bool Sharp.Shared.Objects.IGameRules.IsGameRestart` [L:145]
  - Modifiers: public, abstract
  - Summary: Game restart flag (m_bGameRestart)
- `bool Sharp.Shared.Objects.IGameRules.IsMatchStarted` [L:130]
  - Modifiers: public, abstract, readonly
  - Summary: Whether match has started
- `bool Sharp.Shared.Objects.IGameRules.IsTeamIntroPeriod` [L:95]
  - Modifiers: public, abstract, readonly
  - Summary: Whether in team intro period
- `bool Sharp.Shared.Objects.IGameRules.IsValveDS` [L:140]
  - Modifiers: public, abstract
  - Summary: Whether this is a Valve dedicated server
- `bool Sharp.Shared.Objects.IGameRules.IsWarmupPeriod` [L:85]
  - Modifiers: public, abstract, readonly
  - Summary: Whether in warmup period
- `bool Sharp.Shared.Objects.IGameRules.MatchWaitingForResume` [L:115]
  - Modifiers: public, abstract
  - Summary: Whether match is waiting for resume
- `bool Sharp.Shared.Objects.IGameRules.PlayedTeamIntroVO` [L:160]
  - Modifiers: public, abstract
  - Summary: Whether team intro voice-over has been played
- `bool Sharp.Shared.Objects.IGameRules.SwitchingTeamsAtRoundReset` [L:65]
  - Modifiers: public, abstract
  - Summary: Switch teams at round reset
- `float Sharp.Shared.Objects.IGameRules.GameStartTime` [L:105]
  - Modifiers: public, abstract
  - Summary: Game start time
- `float Sharp.Shared.Objects.IGameRules.RestartRoundTime` [L:120]
  - Modifiers: public, abstract, readonly
  - Summary: Round restart time (based on CurTime)
- `float Sharp.Shared.Objects.IGameRules.RoundStartTime` [L:110]
  - Modifiers: public, abstract
  - Summary: Round start time (based on CurTime)
- `int Sharp.Shared.Objects.IGameRules.CTTimeOuts` [L:45]
  - Modifiers: public, abstract, readonly
  - Summary: Remaining timeouts for CT team
- `int Sharp.Shared.Objects.IGameRules.MaxNumCTs` [L:60]
  - Modifiers: public, abstract
  - Summary: Maximum allowed CT players
- `int Sharp.Shared.Objects.IGameRules.MaxNumTEs` [L:55]
  - Modifiers: public, abstract
  - Summary: Maximum allowed terrorist players
- `int Sharp.Shared.Objects.IGameRules.NumCT` [L:35]
  - Modifiers: public, abstract, readonly
  - Summary: Current number of CT players
- `int Sharp.Shared.Objects.IGameRules.NumTE` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: Current number of terrorist players
- `int Sharp.Shared.Objects.IGameRules.RoundTime` [L:100]
  - Modifiers: public, abstract
  - Summary: Round time in seconds
- `int Sharp.Shared.Objects.IGameRules.RoundsPlayedThisPhase` [L:155]
  - Modifiers: public, abstract
  - Summary: Rounds played in current phase
- `int Sharp.Shared.Objects.IGameRules.TETimeOuts` [L:50]
  - Modifiers: public, abstract, readonly
  - Summary: Remaining timeouts for terrorist team
- `int Sharp.Shared.Objects.IGameRules.TotalRoundsPlayed` [L:125]
  - Modifiers: public, abstract, readonly
  - Summary: Total rounds played

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<int> Sharp.Shared.Objects.IGameRules.GetEndMatchMapGroupVoteOptions()` [L:207]
  - Modifiers: public, abstract
  - Summary: End match map group vote options (m_nEndMatchMapGroupVoteOptions)
- `Sharp.Shared.CStrike.ISchemaArray<int> Sharp.Shared.Objects.IGameRules.GetEndMatchMapGroupVoteTypes()` [L:201]
  - Modifiers: public, abstract
  - Summary: End match map group vote types (m_nEndMatchMapGroupVoteTypes)
- `float Sharp.Shared.Objects.IGameRules.GetMapRemainingTime()` [L:195]
  - Modifiers: public, abstract
  - Summary: Get remaining time on map
- `float Sharp.Shared.Objects.IGameRules.GetRoundElapsedTime()` [L:185]
  - Modifiers: public, abstract
  - Summary: Get elapsed time in current round
- `float Sharp.Shared.Objects.IGameRules.GetRoundRemainingTime()` [L:180]
  - Modifiers: public, abstract
  - Summary: Get remaining time in current round
- `void Sharp.Shared.Objects.IGameRules.RestartGame()` [L:150]
  - Modifiers: public, abstract
  - Summary: Restart the game
- `void Sharp.Shared.Objects.IGameRules.TerminateRound(float delay, Sharp.Shared.Enums.RoundEndReason reason, [bool bypassHook = false], [Sharp.Shared.Types.TeamRewardInfo[]? info = null])` [L:175]
  - Modifiers: public, abstract
  - Summary: End the current round


### interface IGameSystem : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IGameSystem`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IGameSystem.cs:24
- Generated: false


### interface IGlobalVars : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IGlobalVars`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IGlobalVars.cs:9
- Generated: false

#### Properties
- `bool Sharp.Shared.Objects.IGlobalVars.InSimulation` [L:54]
  - Modifiers: public, abstract, readonly
  - Summary: Whether simulation is running
- `float Sharp.Shared.Objects.IGlobalVars.AbsoluteFrameStartTimeStdDev` [L:29]
  - Modifiers: public, abstract, readonly
  - Summary: Frame start time standard deviation based on engine time
- `float Sharp.Shared.Objects.IGlobalVars.AbsoluteFrameTime` [L:24]
  - Modifiers: public, abstract, readonly
  - Summary: Frame time based on engine time
- `float Sharp.Shared.Objects.IGlobalVars.CurTime` [L:44]
  - Modifiers: public, abstract, readonly
  - Summary: Current game time
- `float Sharp.Shared.Objects.IGlobalVars.FrameTime` [L:39]
  - Modifiers: public, abstract, readonly
  - Summary: Time between frames
- `float Sharp.Shared.Objects.IGlobalVars.RealTime` [L:14]
  - Modifiers: public, abstract, readonly
  - Summary: Real time in seconds
- `float Sharp.Shared.Objects.IGlobalVars.RenderTime` [L:49]
  - Modifiers: public, abstract, readonly
  - Summary: Render time
- `float Sharp.Shared.Objects.IGlobalVars.SubTickFraction` [L:64]
  - Modifiers: public, abstract, readonly
  - Summary: Sub-tick fraction
- `int Sharp.Shared.Objects.IGlobalVars.FrameCount` [L:19]
  - Modifiers: public, abstract, readonly
  - Summary: Current frame number
- `int Sharp.Shared.Objects.IGlobalVars.MaxClients` [L:34]
  - Modifiers: public, abstract, readonly
  - Summary: Maximum allowed client connections
- `int Sharp.Shared.Objects.IGlobalVars.MaxEntities` [L:75]
  - Modifiers: public, abstract, readonly
  - Summary: Maximum number of entities Refers to maximum Edict count
- `int Sharp.Shared.Objects.IGlobalVars.TickCount` [L:59]
  - Modifiers: public, abstract, readonly
  - Summary: Current tick count
- `string Sharp.Shared.Objects.IGlobalVars.MapName` [L:69]
  - Modifiers: public, abstract, readonly
  - Summary: Current map name


### interface IKeyValues : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IKeyValues`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IKeyValues.cs:27
- Generated: false

#### Methods
- `Sharp.Shared.Enums.KeyValuesDataType Sharp.Shared.Objects.IKeyValues.GetDataType([string? name = null])` [L:127]
  - Modifiers: public, abstract
  - Summary: Get data type of value
- `Sharp.Shared.Objects.IKeyValues Sharp.Shared.Objects.IKeyValues.AddKey(string name)` [L:122]
  - Modifiers: public, abstract
  - Summary: Add new key
- `Sharp.Shared.Objects.IKeyValues Sharp.Shared.Objects.IKeyValues.Clone()` [L:41]
  - Modifiers: public, abstract
  - Summary: Clone this KeyValues instance
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.FindKey(string name, [bool bCreate = false])` [L:112]
  - Modifiers: public, abstract
  - Summary: Find key by name, optionally create if not found
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.FindLastSubKey()` [L:90]
  - Modifiers: public, abstract
  - Summary: Get last sub-key (includes both keys and key-value pairs)
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.GetFirstSubKey()` [L:85]
  - Modifiers: public, abstract
  - Summary: Get first sub-key (includes both keys and key-value pairs)
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.GetFirstTrueSubKey()` [L:100]
  - Modifiers: public, abstract
  - Summary: Get first sub-key (keys only, not key-value pairs)
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.GetNextKey()` [L:95]
  - Modifiers: public, abstract
  - Summary: Get next key
- `Sharp.Shared.Objects.IKeyValues? Sharp.Shared.Objects.IKeyValues.GetNextTrueSubKey()` [L:105]
  - Modifiers: public, abstract
  - Summary: Get next sub-key (keys only, not key-value pairs)
- `bool Sharp.Shared.Objects.IKeyValues.FindAndDeleteSubKey(string name)` [L:117]
  - Modifiers: public, abstract
  - Summary: Find and delete sub-key by name
- `bool Sharp.Shared.Objects.IKeyValues.GetBool([string? name = null], [bool defaultValue = false])` [L:139]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues.IsEmpty([string? name = null])` [L:141]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues.LoadFromFile(string filename, [string? pathId = null])` [L:51]
  - Modifiers: public, abstract
  - Summary: Load from file
- `bool Sharp.Shared.Objects.IKeyValues.LoadFromString(string buffer)` [L:61]
  - Modifiers: public, abstract
  - Summary: Load from string
- `bool Sharp.Shared.Objects.IKeyValues.SaveToFile(string filename, [string? pathId = null], [bool allowEmptyString = false])` [L:56]
  - Modifiers: public, abstract
  - Summary: Save to file
- `bool Sharp.Shared.Objects.IKeyValues.SaveToString(int size, out string result, [int indent = 0], [bool sort = false], [bool allowEmptyString = false])` [L:66]
  - Modifiers: public, abstract
  - Summary: Export to string
- `float Sharp.Shared.Objects.IKeyValues.GetFloat([string? name = null], [float defaultValue = 0])` [L:133]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.IKeyValues.GetInt([string? name = null], [int defaultValue = 0])` [L:129]
  - Modifiers: public, abstract
- `nint Sharp.Shared.Objects.IKeyValues.GetPtr([string? name = null])` [L:137]
  - Modifiers: public, abstract
- `string Sharp.Shared.Objects.IKeyValues.GetSectionName()` [L:75]
  - Modifiers: public, abstract
  - Summary: Get current section name
- `string Sharp.Shared.Objects.IKeyValues.GetString([string? name = null], [string defaultValue = ""])` [L:135]
  - Modifiers: public, abstract
- `ulong Sharp.Shared.Objects.IKeyValues.GetUint64([string? name = null], [ulong defaultValue = 0])` [L:131]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.Clear()` [L:46]
  - Modifiers: public, abstract
  - Summary: Clear all keys and sub-keys
- `void Sharp.Shared.Objects.IKeyValues.DeleteThis()` [L:36]
  - Modifiers: public, abstract
  - Summary: Destroy this instance
- `void Sharp.Shared.Objects.IKeyValues.SetBool(string name, bool value)` [L:153]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.SetFloat(string name, float value)` [L:149]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.SetInt(string name, int value)` [L:145]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.SetPtr(string name, nint value)` [L:151]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.SetSectionName(string name)` [L:80]
  - Modifiers: public, abstract
  - Summary: Set section name
- `void Sharp.Shared.Objects.IKeyValues.SetString(string name, string value)` [L:143]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues.SetUint64(string name, ulong value)` [L:147]
  - Modifiers: public, abstract


### interface IKeyValues3 : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.IKeyValues3`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IKeyValues.cs:156
- Generated: false

#### Methods
- `Sharp.Shared.Enums.KeyValues3SubType Sharp.Shared.Objects.IKeyValues3.GetSubType()` [L:217]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.KeyValues3Type Sharp.Shared.Objects.IKeyValues3.GetKvType()` [L:187]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IKeyValues3? Sharp.Shared.Objects.IKeyValues3.AddArrayElementToTail()` [L:223]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IKeyValues3? Sharp.Shared.Objects.IKeyValues3.FindMember(string name)` [L:233]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IKeyValues3? Sharp.Shared.Objects.IKeyValues3.FindOrCreateMember(string name, out bool create)` [L:235]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IKeyValues3? Sharp.Shared.Objects.IKeyValues3.GetArrayElement(int index)` [L:221]
  - Modifiers: public, abstract
- `Sharp.Shared.Objects.IKeyValues3? Sharp.Shared.Objects.IKeyValues3.GetMember(int index)` [L:229]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Color32 Sharp.Shared.Objects.IKeyValues3.GetColor()` [L:266]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Matrix3x4 Sharp.Shared.Objects.IKeyValues3.GetMatrix()` [L:272]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.Objects.IKeyValues3.GetQAngle()` [L:270]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.Objects.IKeyValues3.GetVector()` [L:268]
  - Modifiers: public, abstract
- `System.ReadOnlySpan<byte> Sharp.Shared.Objects.IKeyValues3.GetBinaryBlob()` [L:264]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.GetBool([bool defaultValue = false])` [L:240]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsArray()` [L:211]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsBinaryBlob()` [L:209]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsBool()` [L:193]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsDouble()` [L:205]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsInt()` [L:195]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsIntegral()` [L:203]
  - Modifiers: public, abstract
  - Summary: IsInt || IsUInt
- `bool Sharp.Shared.Objects.IKeyValues3.IsInvalid()` [L:189]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsNull()` [L:191]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsNullOrInvalid()` [L:215]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsString()` [L:207]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsTable()` [L:213]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.IsUInt()` [L:197]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.LoadFromBuffer(byte[] buffer, out string error)` [L:185]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.LoadFromCompiledFile(string file, string pathId, Sharp.Shared.Enums.ResourceBlockType block, out string error)` [L:183]
  - Modifiers: public, abstract
  - Summary: Load the given datablock type from the given compiled resource
- `bool Sharp.Shared.Objects.IKeyValues3.LoadFromCompiledFile(string file, string pathId, out string error)` [L:173]
  - Modifiers: public, abstract
  - Summary: Load the  type from the given compiled resource
- `bool Sharp.Shared.Objects.IKeyValues3.LoadFromFile(string file, string pathId, out string error)` [L:164]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.IKeyValues3.RemoveMember(string name)` [L:237]
  - Modifiers: public, abstract
- `byte Sharp.Shared.Objects.IKeyValues3.GetUInt8([byte defaultValue = 0])` [L:250]
  - Modifiers: public, abstract
- `double Sharp.Shared.Objects.IKeyValues3.GetDouble([double defaultValue = 0])` [L:260]
  - Modifiers: public, abstract
- `float Sharp.Shared.Objects.IKeyValues3.GetFloat([float defaultValue = 0])` [L:258]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.IKeyValues3.GetArrayElementCount()` [L:219]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.IKeyValues3.GetInt32([int defaultValue = 0])` [L:246]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.IKeyValues3.GetMemberCount()` [L:227]
  - Modifiers: public, abstract
- `long Sharp.Shared.Objects.IKeyValues3.GetInt64([long defaultValue = 0])` [L:248]
  - Modifiers: public, abstract
- `sbyte Sharp.Shared.Objects.IKeyValues3.GetInt8([sbyte defaultValue = 0])` [L:242]
  - Modifiers: public, abstract
- `short Sharp.Shared.Objects.IKeyValues3.GetInt16([short defaultValue = 0])` [L:244]
  - Modifiers: public, abstract
- `string Sharp.Shared.Objects.IKeyValues3.GetMemberName(int index)` [L:231]
  - Modifiers: public, abstract
- `string Sharp.Shared.Objects.IKeyValues3.GetString([string defaultValue = ""])` [L:262]
  - Modifiers: public, abstract
- `uint Sharp.Shared.Objects.IKeyValues3.GetUInt32([uint defaultValue = 0])` [L:254]
  - Modifiers: public, abstract
- `ulong Sharp.Shared.Objects.IKeyValues3.GetUInt64([ulong defaultValue = 0])` [L:256]
  - Modifiers: public, abstract
- `ushort Sharp.Shared.Objects.IKeyValues3.GetUInt16([ushort defaultValue = 0])` [L:252]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.DeleteThis()` [L:162]
  - Modifiers: public, abstract
  - Summary: Destroy this instance Only instances created by  can be destroyed
- `void Sharp.Shared.Objects.IKeyValues3.RemoveArrayElement(int index)` [L:225]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetBool(bool value)` [L:275]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetColor(Sharp.Shared.Types.Color32 value)` [L:299]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetDouble(double value)` [L:295]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetFloat(float value)` [L:293]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetInt16(short value)` [L:279]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetInt32(int value)` [L:281]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetInt64(long value)` [L:283]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetInt8(sbyte value)` [L:277]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetMatrix(Sharp.Shared.Types.Matrix3x4 value)` [L:305]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetQAngle(Sharp.Shared.Types.Vector value)` [L:303]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetString(string value)` [L:297]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetUInt16(ushort value)` [L:287]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetUInt32(uint value)` [L:289]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetUInt64(ulong value)` [L:291]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetUInt8(byte value)` [L:285]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IKeyValues3.SetVector(Sharp.Shared.Types.Vector value)` [L:301]
  - Modifiers: public, abstract


### interface IMemAlloc

- FullName: `Sharp.Shared.Objects.IMemAlloc`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/IMemAlloc.cs:22
- Generated: false

#### Methods
- `nint Sharp.Shared.Objects.IMemAlloc.Alloc(int size)` [L:24]
  - Modifiers: public, abstract
- `nint Sharp.Shared.Objects.IMemAlloc.ReAlloc(nint pMem, int size)` [L:26]
  - Modifiers: public, abstract
- `void Sharp.Shared.Objects.IMemAlloc.Free(nint pMem)` [L:28]
  - Modifiers: public, abstract


### interface INativeProtobuf : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.INativeProtobuf`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/INativeProtobuf.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.Objects.INativeProtobuf? Sharp.Shared.Objects.INativeProtobuf.AddMessage(string field)` [L:120]
  - Modifiers: public, abstract
  - Summary: Add new message to field
- `Sharp.Shared.Objects.INativeProtobuf? Sharp.Shared.Objects.INativeProtobuf.ReadMessage(string field, [int repeatedIndex = -1])` [L:113]
  - Modifiers: public, abstract
  - Summary: Read nested message
- `T Sharp.Shared.Objects.INativeProtobuf.Deserialize<T>() where T : class, Google.Protobuf.IMessage<T>, Google.Protobuf.IMessage, new()` [L:138]
  - Modifiers: public, abstract
  - Summary: Deserialize to C# readable  object
- `bool Sharp.Shared.Objects.INativeProtobuf.CopyFromOtherMessage(Google.Protobuf.IMessage message)` [L:133]
  - Modifiers: public, abstract
  - Summary: Copy data from another  and overwrite
- `bool Sharp.Shared.Objects.INativeProtobuf.HasField(string field)` [L:42]
  - Modifiers: public, abstract
  - Summary: Check if field exists
- `bool Sharp.Shared.Objects.INativeProtobuf.RemoveRepeatedFieldValue(string field, int repeatedIndex)` [L:128]
  - Modifiers: public, abstract
  - Summary: Remove value from repeated field
- `bool Sharp.Shared.Objects.INativeProtobuf.SetBool(string field, bool value, [int repeatedIndex = -1])` [L:77]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetBytes(string field, byte[] value, [int repeatedIndex = -1])` [L:87]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetDouble(string field, double value, [int repeatedIndex = -1])` [L:83]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetEnum(string field, int value, [int repeatedIndex = -1])` [L:79]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetFloat(string field, float value, [int repeatedIndex = -1])` [L:81]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetInt32(string field, int value, [int repeatedIndex = -1])` [L:69]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetInt64(string field, long value, [int repeatedIndex = -1])` [L:73]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetString(string field, string value, [int repeatedIndex = -1])` [L:85]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetUInt32(string field, uint value, [int repeatedIndex = -1])` [L:71]
  - Modifiers: public, abstract
- `bool Sharp.Shared.Objects.INativeProtobuf.SetUInt64(string field, ulong value, [int repeatedIndex = -1])` [L:75]
  - Modifiers: public, abstract
- `bool? Sharp.Shared.Objects.INativeProtobuf.ReadBool(string field, [int repeatedIndex = -1])` [L:57]
  - Modifiers: public, abstract
- `byte[]? Sharp.Shared.Objects.INativeProtobuf.ReadBytes(string field, [int repeatedIndex = -1])` [L:67]
  - Modifiers: public, abstract
- `double? Sharp.Shared.Objects.INativeProtobuf.ReadDouble(string field, [int repeatedIndex = -1])` [L:63]
  - Modifiers: public, abstract
- `float? Sharp.Shared.Objects.INativeProtobuf.ReadFloat(string field, [int repeatedIndex = -1])` [L:61]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddBool(string field, bool value)` [L:97]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddBytes(string field, byte[] value)` [L:107]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddDouble(string field, double value)` [L:103]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddEnum(string field, int value)` [L:99]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddFloat(string field, float value)` [L:101]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddInt32(string field, int value)` [L:89]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddInt64(string field, long value)` [L:93]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddString(string field, string value)` [L:105]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddUInt32(string field, uint value)` [L:91]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.AddUInt64(string field, ulong value)` [L:95]
  - Modifiers: public, abstract
- `int Sharp.Shared.Objects.INativeProtobuf.GetRepeatedFieldCount(string field)` [L:47]
  - Modifiers: public, abstract
  - Summary: Get number of elements in repeated field
- `int? Sharp.Shared.Objects.INativeProtobuf.ReadEnum(string field, [int repeatedIndex = -1])` [L:59]
  - Modifiers: public, abstract
- `int? Sharp.Shared.Objects.INativeProtobuf.ReadInt32(string field, [int repeatedIndex = -1])` [L:49]
  - Modifiers: public, abstract
- `long? Sharp.Shared.Objects.INativeProtobuf.ReadInt64(string field, [int repeatedIndex = -1])` [L:53]
  - Modifiers: public, abstract
- `string Sharp.Shared.Objects.INativeProtobuf.GetName()` [L:31]
  - Modifiers: public, abstract
  - Summary: Get message name
- `string? Sharp.Shared.Objects.INativeProtobuf.ReadString(string field, [int repeatedIndex = -1])` [L:65]
  - Modifiers: public, abstract
- `uint? Sharp.Shared.Objects.INativeProtobuf.ReadUInt32(string field, [int repeatedIndex = -1])` [L:51]
  - Modifiers: public, abstract
- `ulong Sharp.Shared.Objects.INativeProtobuf.GetSize()` [L:37]
  - Modifiers: public, abstract
  - Summary: Get message size in bytes
- `ulong? Sharp.Shared.Objects.INativeProtobuf.ReadUInt64(string field, [int repeatedIndex = -1])` [L:55]
  - Modifiers: public, abstract


### interface INetMessage : Sharp.Shared.Objects.INativeProtobuf

- FullName: `Sharp.Shared.Objects.INetMessage`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/INetMessage.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Enums.ProtobufNetMessageType Sharp.Shared.Objects.INetMessage.MessageId` [L:26]
  - Modifiers: public, abstract, readonly


### interface INetworkServer : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.INetworkServer`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/INetworkServer.cs:28
- Generated: false

#### Methods
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Objects.INetworkServer.GetGameClient(Sharp.Shared.Units.PlayerSlot slot)` [L:44]
  - Modifiers: public, abstract
  - Summary: Get client by player slot
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Objects.INetworkServer.GetGameClient(Sharp.Shared.Units.SteamID steamId)` [L:54]
  - Modifiers: public, abstract
  - Summary: Get client by Steam ID
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.Objects.INetworkServer.GetGameClient(Sharp.Shared.Units.UserID userId)` [L:49]
  - Modifiers: public, abstract
  - Summary: Get client by user ID
- `Sharp.Shared.Types.Tier.CUtlVector<nint>* Sharp.Shared.Objects.INetworkServer.GetGameClientPointers()` [L:72]
  - Modifiers: public, abstract
  - Summary: Retrieves a pointer to the internal server client list container.
- `System.Collections.Generic.List<Sharp.Shared.Objects.IGameClient> Sharp.Shared.Objects.INetworkServer.GetGameClients(bool connected, [bool inGame = false])` [L:66]
  - Modifiers: public, abstract
  - Summary: Get filtered list of clients  will override
- `int Sharp.Shared.Objects.INetworkServer.GetClientCount()` [L:33]
  - Modifiers: public, abstract
  - Summary: Get total number of clients in pool
- `int Sharp.Shared.Objects.INetworkServer.GetClientCount(bool connected, [bool inGame = false])` [L:39]
  - Modifiers: public, abstract
  - Summary: Get number of clients in pool with filters

#### Obsolete Members
- `System.Collections.Generic.IReadOnlyList<Sharp.Shared.Objects.IGameClient> Sharp.Shared.Objects.INetworkServer.GetGameClients()` [L:60] — Use overload GetGameClients(bool, bool) instead, will be removed in 2.2
- `int Sharp.Shared.Objects.INetworkServer.GetGameClientCount([bool fullyInGame = false])` [L:78] — Use GetClientCount(bool, bool) instead, will be removed in 2.2


### interface INetworkingStringTable : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.Objects.INetworkingStringTable`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/INetworkingStringTable.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.Types.StringTableUserData* Sharp.Shared.Objects.INetworkingStringTable.GetStringUserData(int index)` [L:59]
  - Modifiers: public, abstract
  - Summary: Get UserData from given index
- `int Sharp.Shared.Objects.INetworkingStringTable.AddString(bool server, string value, byte[]? data)` [L:49]
  - Modifiers: public, abstract
  - Summary: Insert a new string to current string table
- `int Sharp.Shared.Objects.INetworkingStringTable.FindStringIndex(string value)` [L:70]
  - Modifiers: public, abstract
  - Summary: Get the index from given string value
- `int Sharp.Shared.Objects.INetworkingStringTable.GetId()` [L:35]
  - Modifiers: public, abstract
  - Summary: Table ID
- `int Sharp.Shared.Objects.INetworkingStringTable.GetStringCount()` [L:41]
  - Modifiers: public, abstract
  - Summary: Get How many entries this table has
- `string Sharp.Shared.Objects.INetworkingStringTable.GetName()` [L:30]
  - Modifiers: public, abstract
  - Summary: Table name
- `string Sharp.Shared.Objects.INetworkingStringTable.GetString(int index)` [L:54]
  - Modifiers: public, abstract
  - Summary: Get string value by index
- `void Sharp.Shared.Objects.INetworkingStringTable.SetStringUserData(int index, byte[]? data)` [L:64]
  - Modifiers: public, abstract
  - Summary: Override UserData


### interface ISteamApi

- FullName: `Sharp.Shared.Objects.ISteamApi`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Objects/ISteamApi.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.Enums.UserHasLicenseForApp Sharp.Shared.Objects.ISteamApi.UserHasLicenseForApp(Sharp.Shared.Units.SteamID steamId, uint appId)` [L:99]
  - Modifiers: public, abstract
  - Summary: After receiving a user's authentication data, and passing it to SendUserConnectAndAuthenticate, use this function
- `Sharp.Shared.Enums.WorkshopItemState Sharp.Shared.Objects.ISteamApi.GetItemState(ulong sharedFileId)` [L:104]
  - Modifiers: public, abstract
  - Summary: Get Steam Workshop item state
- `Sharp.Shared.Units.SteamID Sharp.Shared.Objects.ISteamApi.GetSteamId()` [L:51]
  - Modifiers: public, abstract
  - Summary: Get server Steam ID
- `bool Sharp.Shared.Objects.ISteamApi.BLoggedOn()` [L:41]
  - Modifiers: public, abstract
  - Summary: Check if logged into Steam
- `bool Sharp.Shared.Objects.ISteamApi.BSecure()` [L:46]
  - Modifiers: public, abstract
  - Summary: Check if server is VAC secured
- `bool Sharp.Shared.Objects.ISteamApi.DownloadItem(ulong sharedFileId, bool highPriority)` [L:115]
  - Modifiers: public, abstract
  - Summary: Download Steam Workshop item
- `bool Sharp.Shared.Objects.ISteamApi.GetItemDownloadInfo(ulong sharedFileId, out ulong bytesDownloaded, out ulong bytesTotal)` [L:109]
  - Modifiers: public, abstract
  - Summary: Get download progress information
- `bool Sharp.Shared.Objects.ISteamApi.IsAvailable()` [L:30]
  - Modifiers: public, abstract
  - Summary: Check if Steam service is available
- `bool Sharp.Shared.Objects.ISteamApi.RequestUserGroupStatus(Sharp.Shared.Units.SteamID steamId, Sharp.Shared.Units.SteamID groupId)` [L:92]
  - Modifiers: public, abstract
  - Summary: Ask if a user in the specified group, results returns async by GSUserGroupStatus_t
- `bool Sharp.Shared.Objects.ISteamApi.WasRestartRequested()` [L:56]
  - Modifiers: public, abstract
  - Summary: Returns true if the master server has requested a restart.
- `uint Sharp.Shared.Objects.ISteamApi.GetPublicIP()` [L:126]
  - Modifiers: public, abstract
  - Summary: Get public IP address from master server
- `void Sharp.Shared.Objects.ISteamApi.SetBotPlayerCount(int count)` [L:66]
  - Modifiers: public, abstract
  - Summary: Number of bots.  Default value is zero
- `void Sharp.Shared.Objects.ISteamApi.SetGameDescription(string description)` [L:36]
  - Modifiers: public, abstract
  - Summary: Description of the game.  This is a required field and is displayed in the steam server browser....for now. This is
- `void Sharp.Shared.Objects.ISteamApi.SetGameTags(string tags)` [L:87]
  - Modifiers: public, abstract
  - Summary: Sets a string defining the "gametags" for this server, this is optional, but if it is set
- `void Sharp.Shared.Objects.ISteamApi.SetMapName(string name)` [L:76]
  - Modifiers: public, abstract
  - Summary: Set name of map to report in the server browser
- `void Sharp.Shared.Objects.ISteamApi.SetMaxPlayerCount(int count)` [L:61]
  - Modifiers: public, abstract
  - Summary: Max player count that will be reported to server browser and client queries
- `void Sharp.Shared.Objects.ISteamApi.SetPasswordProtected(bool protect)` [L:81]
  - Modifiers: public, abstract
  - Summary: Let people know if your server will require a password
- `void Sharp.Shared.Objects.ISteamApi.SetServerName(string name)` [L:71]
  - Modifiers: public, abstract
  - Summary: Set the name of server as it will appear in the server browser
- `void Sharp.Shared.Objects.ISteamApi.SuspendDownloads(bool suspend)` [L:120]
  - Modifiers: public, abstract
  - Summary: Suspend or resume downloads


