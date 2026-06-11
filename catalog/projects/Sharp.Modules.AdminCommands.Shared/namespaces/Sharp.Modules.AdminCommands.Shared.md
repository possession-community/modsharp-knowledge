# Sharp.Modules.AdminCommands.Shared

Project: Sharp.Modules.AdminCommands.Shared
Types: 10 (0 generated)

### record AdminOperationRecord : System.IEquatable<Sharp.Modules.AdminCommands.Shared.AdminOperationRecord>

- FullName: `Sharp.Modules.AdminCommands.Shared.AdminOperationRecord`
- Kind: record
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/AdminOperationRecord.cs:26
- Generated: false

Inheritance: object → **AdminOperationRecord**

#### Constructors
- `Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.AdminOperationRecord(Sharp.Shared.Units.SteamID SteamId, Sharp.Modules.AdminCommands.Shared.AdminOperationType Type, Sharp.Shared.Units.SteamID? AdminSteamId, System.DateTime CreatedAt, System.DateTime? ExpiresAt, string Reason, [string? Metadata = null], [Sharp.Shared.Units.SteamID? RemovedBy = null], [System.DateTime? RemovedAt = null], [string? RemoveReason = null])` [L:26]

#### Properties
- `Sharp.Modules.AdminCommands.Shared.AdminOperationType Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.Type` [L:28]
- `Sharp.Shared.Units.SteamID Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.SteamId` [L:27]
- `Sharp.Shared.Units.SteamID? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.AdminSteamId` [L:29]
- `Sharp.Shared.Units.SteamID? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.RemovedBy` [L:34]
- `System.DateTime Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.CreatedAt` [L:30]
- `System.DateTime? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.ExpiresAt` [L:31]
- `System.DateTime? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.RemovedAt` [L:35]
- `bool Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.IsExpired` [L:39]
  - Modifiers: public, readonly
- `bool Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.IsPermanent` [L:40]
  - Modifiers: public, readonly
- `string Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.Reason` [L:32]
- `string? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.Metadata` [L:33]
- `string? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.RemoveReason` [L:36]

#### Methods
- `T? Sharp.Modules.AdminCommands.Shared.AdminOperationRecord.GetMetadata<T>()` [L:42]


### class AdminOperationStorageExtensions

- FullName: `Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Modules/AdminCommands/Shared/AdminOperationStorageExtensions.cs:29
- Generated: false
- Summary: Convenience helpers for constructing admin operation records against the storage contract.

Inheritance: object → **AdminOperationStorageExtensions**

#### Methods
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.AddBanAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, System.TimeSpan? duration, string reason, [string? metadata = null])` [L:31]
  - Modifiers: public, static, this
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.AddGagAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, System.TimeSpan? duration, string reason, [string? metadata = null])` [L:59]
  - Modifiers: public, static, this
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.AddMuteAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, System.TimeSpan? duration, string reason, [string? metadata = null])` [L:45]
  - Modifiers: public, static, this
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.RemoveBanAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, string? removeReason)` [L:39]
  - Modifiers: public, static, this
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.RemoveGagAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, string? removeReason)` [L:67]
  - Modifiers: public, static, this
- `static System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.AdminOperationStorageExtensions.RemoveMuteAsync(Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService storage, Sharp.Shared.Units.SteamID targetId, Sharp.Shared.Units.SteamID? adminId, string? removeReason)` [L:53]
  - Modifiers: public, static, this


### record struct AdminOperationType : System.ValueType, System.IEquatable<Sharp.Modules.AdminCommands.Shared.AdminOperationType>

- FullName: `Sharp.Modules.AdminCommands.Shared.AdminOperationType`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Modules/AdminCommands/Shared/AdminOperationType.cs:24
- Generated: false

Inheritance: object → System.ValueType → **AdminOperationType**

#### Constructors
- `Sharp.Modules.AdminCommands.Shared.AdminOperationType.AdminOperationType(string Value)` [L:24]

#### Fields
- `static readonly Sharp.Modules.AdminCommands.Shared.AdminOperationType Sharp.Modules.AdminCommands.Shared.AdminOperationType.Ban` [L:26]
  - Modifiers: public, static, readonly
- `static readonly Sharp.Modules.AdminCommands.Shared.AdminOperationType Sharp.Modules.AdminCommands.Shared.AdminOperationType.Gag` [L:28]
  - Modifiers: public, static, readonly
- `static readonly Sharp.Modules.AdminCommands.Shared.AdminOperationType Sharp.Modules.AdminCommands.Shared.AdminOperationType.Mute` [L:27]
  - Modifiers: public, static, readonly

#### Properties
- `string Sharp.Modules.AdminCommands.Shared.AdminOperationType.Value` [L:24]

#### Methods
- `bool Sharp.Modules.AdminCommands.Shared.AdminOperationType.Equals(Sharp.Modules.AdminCommands.Shared.AdminOperationType other)` [L:33]
  - Modifiers: public, readonly
- `override int Sharp.Modules.AdminCommands.Shared.AdminOperationType.GetHashCode()` [L:36]
  - Modifiers: public, override, readonly
- `override string Sharp.Modules.AdminCommands.Shared.AdminOperationType.ToString()` [L:30]
  - Modifiers: public, override, readonly


### interface IAdminOperationHandler

- FullName: `Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IAdminOperationHandler.cs:31
- Generated: false
- Summary: Handler for a specific admin operation type (e.g. Ban, Mute, Gag).

#### Properties
- `Sharp.Modules.AdminCommands.Shared.AdminOperationType Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler.Type` [L:36]
  - Modifiers: public, abstract, readonly
  - Summary: The operation type this handler is responsible for.

#### Methods
- `(string Key, string Fallback) Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler.GetAppliedNotification(Sharp.Shared.Objects.IGameClient target, string durationText)` [L:55]
  - Modifiers: public, abstract
  - Summary: Returns the localization key and fallback message when this operation is applied.
- `(string Key, string Fallback) Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler.GetRemovedNotification(Sharp.Shared.Objects.IGameClient target)` [L:60]
  - Modifiers: public, abstract
  - Summary: Returns the localization key and fallback message when this operation is removed.
- `void Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler.OnApplied(Sharp.Modules.AdminCommands.Shared.AdminOperationRecord record, Sharp.Shared.Objects.IGameClient? targetClient)` [L:43]
  - Modifiers: public, abstract
  - Summary: Called when an operation is applied.
- `void Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler.OnRemoved(Sharp.Shared.Units.SteamID steamId, Sharp.Shared.Objects.IGameClient? targetClient)` [L:50]
  - Modifiers: public, abstract
  - Summary: Called when an operation is removed.


### interface IAdminOperationStorageService

- FullName: `Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IAdminOperationStorageService.cs:36
- Generated: false
- Summary: Storage contract for admin operations (ban/mute/gag). This is the primary external extension point; implement this

#### Fields
- `const string Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.Identity = "IAdminOperationStorageService"` [L:38]
  - Modifiers: public, static, const

#### Methods
- `System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.AddAsync(Sharp.Modules.AdminCommands.Shared.AdminOperationRecord record)` [L:53]
  - Modifiers: public, abstract
  - Summary: Adds a new record. Implementations should be idempotent if desired (skip or replace duplicates as needed).
- `System.Threading.Tasks.Task Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.RemoveAsync(Sharp.Shared.Units.SteamID targetId, Sharp.Modules.AdminCommands.Shared.AdminOperationType type, Sharp.Shared.Units.SteamID? removedBy, string? reason)` [L:58]
  - Modifiers: public, abstract
  - Summary: Removes a record of the given type for the SteamID (no-op if missing).
- `System.Threading.Tasks.Task<Sharp.Modules.AdminCommands.Shared.AdminOperationRecord?> Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.GetAsync(Sharp.Shared.Units.SteamID steamId, Sharp.Modules.AdminCommands.Shared.AdminOperationType type)` [L:43]
  - Modifiers: public, abstract
  - Summary: Returns a single record for the given SteamID and operation type, or null if none/expired.
- `System.Threading.Tasks.Task<System.Collections.Generic.IReadOnlyList<Sharp.Modules.AdminCommands.Shared.AdminOperationRecord>> Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.GetAllAsync(Sharp.Shared.Units.SteamID steamId)` [L:48]
  - Modifiers: public, abstract
  - Summary: Returns all records for a SteamID (may include expired/removed ones depending on implementation policy).
- `System.Threading.Tasks.Task<bool> Sharp.Modules.AdminCommands.Shared.IAdminOperationStorageService.HasActiveAsync(Sharp.Shared.Units.SteamID steamId, Sharp.Modules.AdminCommands.Shared.AdminOperationType type)` [L:63]
  - Modifiers: public, abstract
  - Summary: Returns true if there is an active (non-expired/non-removed) record of the given type.


### interface IAdminService

- FullName: `Sharp.Modules.AdminCommands.Shared.IAdminService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IAdminService.cs:30
- Generated: false
- Summary: Aggregated admin operation services (ban/mute/gag/silence) exposed to consumers.

#### Fields
- `const string Sharp.Modules.AdminCommands.Shared.IAdminService.Identity = "IAdminService"` [L:32]
  - Modifiers: public, static, const

#### Properties
- `Sharp.Modules.AdminCommands.Shared.IBanService Sharp.Modules.AdminCommands.Shared.IAdminService.Ban` [L:34]
  - Modifiers: public, abstract, readonly
- `Sharp.Modules.AdminCommands.Shared.IGagService Sharp.Modules.AdminCommands.Shared.IAdminService.Gag` [L:36]
  - Modifiers: public, abstract, readonly
- `Sharp.Modules.AdminCommands.Shared.IMuteService Sharp.Modules.AdminCommands.Shared.IAdminService.Mute` [L:35]
  - Modifiers: public, abstract, readonly
- `Sharp.Modules.AdminCommands.Shared.ISilenceService Sharp.Modules.AdminCommands.Shared.IAdminService.Silence` [L:37]
  - Modifiers: public, abstract, readonly

#### Methods
- `Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler? Sharp.Modules.AdminCommands.Shared.IAdminService.GetHandler(Sharp.Modules.AdminCommands.Shared.AdminOperationType type)` [L:106]
  - Modifiers: public, abstract
  - Summary: Returns the currently registered handler for the given operation type, or null if none is registered.
- `void Sharp.Modules.AdminCommands.Shared.IAdminService.Apply(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, Sharp.Modules.AdminCommands.Shared.AdminOperationType type, System.TimeSpan? duration, string reason, [bool silent = false])` [L:53]
  - Modifiers: public, abstract
  - Summary: Applies an admin operation to an online target.
- `void Sharp.Modules.AdminCommands.Shared.IAdminService.Apply(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID target, Sharp.Modules.AdminCommands.Shared.AdminOperationType type, System.TimeSpan? duration, string reason)` [L:68]
  - Modifiers: public, abstract
  - Summary: Applies an admin operation to an offline target.
- `void Sharp.Modules.AdminCommands.Shared.IAdminService.RegisterHandler(string moduleIdentity, Sharp.Modules.AdminCommands.Shared.IAdminOperationHandler handler)` [L:43]
  - Modifiers: public, abstract
  - Summary: Registers a new operation handler. It is not recommended to register handlers outside OnAllModuleLoaded or
- `void Sharp.Modules.AdminCommands.Shared.IAdminService.Remove(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, Sharp.Modules.AdminCommands.Shared.AdminOperationType type, string reason, [bool silent = false])` [L:81]
  - Modifiers: public, abstract
  - Summary: Removes an admin operation from an online target.
- `void Sharp.Modules.AdminCommands.Shared.IAdminService.Remove(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID target, Sharp.Modules.AdminCommands.Shared.AdminOperationType type, string reason)` [L:94]
  - Modifiers: public, abstract
  - Summary: Removes an admin operation from an offline target.


### interface IBanService

- FullName: `Sharp.Modules.AdminCommands.Shared.IBanService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IBanService.cs:31
- Generated: false
- Summary: Ban/unban operations. Provided for callers; not intended for external implementations.

#### Methods
- `void Sharp.Modules.AdminCommands.Shared.IBanService.Ban(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, System.TimeSpan? duration, string reason)` [L:36]
  - Modifiers: public, abstract
  - Summary: Ban an online target (may kick/notify, updates cache).
- `void Sharp.Modules.AdminCommands.Shared.IBanService.Ban(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID steamId, System.TimeSpan? duration, string reason)` [L:41]
  - Modifiers: public, abstract
  - Summary: Ban by SteamID (offline path; updates cache/storage, may kick if target joins).
- `void Sharp.Modules.AdminCommands.Shared.IBanService.Unban(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID steamId, string reason)` [L:46]
  - Modifiers: public, abstract
  - Summary: Remove a ban for the given SteamID (updates cache/storage).


### interface IGagService

- FullName: `Sharp.Modules.AdminCommands.Shared.IGagService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IGagService.cs:31
- Generated: false
- Summary: Gag/ungag operations. Provided for callers; not intended for external implementations.

#### Methods
- `void Sharp.Modules.AdminCommands.Shared.IGagService.Gag(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, System.TimeSpan? duration, string reason)` [L:36]
  - Modifiers: public, abstract
  - Summary: Gag an online target (updates cache/storage, may notify).
- `void Sharp.Modules.AdminCommands.Shared.IGagService.Gag(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID steamId, System.TimeSpan? duration, string reason)` [L:41]
  - Modifiers: public, abstract
  - Summary: Gag by SteamID (offline path; updates cache/storage when player joins).
- `void Sharp.Modules.AdminCommands.Shared.IGagService.Ungag(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, string reason)` [L:46]
  - Modifiers: public, abstract
  - Summary: Remove gag on an online target (updates cache/storage).


### interface IMuteService

- FullName: `Sharp.Modules.AdminCommands.Shared.IMuteService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/IMuteService.cs:31
- Generated: false
- Summary: Mute/unmute operations. Provided for callers; not intended for external implementations.

#### Methods
- `void Sharp.Modules.AdminCommands.Shared.IMuteService.Mute(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, System.TimeSpan? duration, string reason)` [L:36]
  - Modifiers: public, abstract
  - Summary: Mute an online target (updates cache/storage, may notify).
- `void Sharp.Modules.AdminCommands.Shared.IMuteService.Mute(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Units.SteamID steamId, System.TimeSpan? duration, string reason)` [L:41]
  - Modifiers: public, abstract
  - Summary: Mute by SteamID (offline path; updates cache/storage when player joins).
- `void Sharp.Modules.AdminCommands.Shared.IMuteService.Unmute(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, string reason)` [L:46]
  - Modifiers: public, abstract
  - Summary: Unmute an online target (updates cache/storage).


### interface ISilenceService

- FullName: `Sharp.Modules.AdminCommands.Shared.ISilenceService`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminCommands/Shared/ISilenceService.cs:30
- Generated: false
- Summary: Silence/unsilence operations (mute+gag). Provided for callers; not intended for external implementations.

#### Methods
- `void Sharp.Modules.AdminCommands.Shared.ISilenceService.Silence(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, System.TimeSpan? duration, string reason)` [L:35]
  - Modifiers: public, abstract
  - Summary: Apply silence (mute+gag) to an online target (updates cache/storage, may notify).
- `void Sharp.Modules.AdminCommands.Shared.ISilenceService.Unsilence(Sharp.Shared.Objects.IGameClient? admin, Sharp.Shared.Objects.IGameClient target, string reason)` [L:40]
  - Modifiers: public, abstract
  - Summary: Remove silence (mute+gag) from an online target (updates cache/storage).


