# Sharp.Modules.ClientPreferences.Core

Project: Sharp.Modules.ClientPreferences
Types: 1 (0 generated)

### class ClientPreferences : Sharp.Modules.ClientPreferences.Shared.IClientPreference, Sharp.Shared.IModSharpModule, Sharp.Shared.Listeners.IClientListener

- FullName: `Sharp.Modules.ClientPreferences.Core.ClientPreferences`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/ClientPreferences/src/ClientPreferences.cs:39
- Generated: false

Inheritance: object → **ClientPreferences**

#### Constructors
- `Sharp.Modules.ClientPreferences.Core.ClientPreferences.ClientPreferences(Sharp.Shared.ISharedSystem sharedSystem, string dllPath, string sharpPath, System.Version version, Microsoft.Extensions.Configuration.IConfiguration configuration, bool hotReload)` [L:58]

#### Properties
- `string Sharp.Modules.ClientPreferences.Core.ClientPreferences.DisplayAuthor` [L:42]
  - Modifiers: public, readonly
- `string Sharp.Modules.ClientPreferences.Core.ClientPreferences.DisplayName` [L:41]
  - Modifiers: public, readonly

#### Methods
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Core.ClientPreferences.SetCookie(Sharp.Shared.Units.SteamID identity, string key, bool value)` [L:312]
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Core.ClientPreferences.SetCookie(Sharp.Shared.Units.SteamID identity, string key, double value)` [L:334]
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Core.ClientPreferences.SetCookie(Sharp.Shared.Units.SteamID identity, string key, long value)` [L:315]
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Core.ClientPreferences.SetCookie(Sharp.Shared.Units.SteamID identity, string key, string value)` [L:353]
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Core.ClientPreferences.SetCookie<T>(Sharp.Shared.Units.SteamID identity, string key, T value) where T : Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<T>` [L:372]
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem? Sharp.Modules.ClientPreferences.Core.ClientPreferences.GetCookie(Sharp.Shared.Units.SteamID identity, string key)` [L:292]
- `System.IDisposable Sharp.Modules.ClientPreferences.Core.ClientPreferences.ListenOnLoad(System.Action<Sharp.Shared.Objects.IGameClient> callback)` [L:279]
- `bool Sharp.Modules.ClientPreferences.Core.ClientPreferences.DeleteCookie(Sharp.Shared.Units.SteamID identity, string key)` [L:302]
- `bool Sharp.Modules.ClientPreferences.Core.ClientPreferences.Init()` [L:124]
- `bool Sharp.Modules.ClientPreferences.Core.ClientPreferences.IsLoaded(Sharp.Shared.Units.SteamID identity)` [L:287]
- `void Sharp.Modules.ClientPreferences.Core.ClientPreferences.OnClientDisconnected(Sharp.Shared.Objects.IGameClient client, Sharp.Shared.Enums.NetworkDisconnectionReason reason)` [L:182]
- `void Sharp.Modules.ClientPreferences.Core.ClientPreferences.OnClientPostAdminCheck(Sharp.Shared.Objects.IGameClient client)` [L:155]
- `void Sharp.Modules.ClientPreferences.Core.ClientPreferences.PostInit()` [L:127]
- `void Sharp.Modules.ClientPreferences.Core.ClientPreferences.Shutdown()` [L:134]


