# Sharp.Modules.AdminFlatFile

Project: Sharp.Modules.AdminFlatFile
Types: 1 (0 generated)

### class AdminFlatFile : Sharp.Shared.IModSharpModule, Sharp.Shared.Listeners.IClientListener

- FullName: `Sharp.Modules.AdminFlatFile.AdminFlatFile`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/AdminFlatFile/src/AdminFlatFile.cs:35
- Generated: false

Inheritance: object → **AdminFlatFile**

#### Constructors
- `Sharp.Modules.AdminFlatFile.AdminFlatFile.AdminFlatFile(Sharp.Shared.ISharedSystem sharedSystem, string dllPath, string sharpPath, System.Version version, Microsoft.Extensions.Configuration.IConfiguration coreConfiguration, bool hotReload)` [L:44]

#### Properties
- `string Sharp.Modules.AdminFlatFile.AdminFlatFile.DisplayAuthor` [L:38]
  - Modifiers: public, readonly
- `string Sharp.Modules.AdminFlatFile.AdminFlatFile.DisplayName` [L:37]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Modules.AdminFlatFile.AdminFlatFile.Init()` [L:56]
- `void Sharp.Modules.AdminFlatFile.AdminFlatFile.OnAdminCacheReload()` [L:76]
- `void Sharp.Modules.AdminFlatFile.AdminFlatFile.PostInit()` [L:59]
- `void Sharp.Modules.AdminFlatFile.AdminFlatFile.Shutdown()` [L:68]


