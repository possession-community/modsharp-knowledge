# Sharp.Extensions.EntityHookManager

Project: Sharp.Extensions.EntityHookManager
Types: 6 (0 generated)

### class DependencyInjection

- FullName: `Sharp.Extensions.EntityHookManager.DependencyInjection`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Extensions/EntityHookManager/src/DependencyInjection.cs:28
- Generated: false

Inheritance: object → **DependencyInjection**

#### Methods
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.EntityHookManager.DependencyInjection.AddEntityHookManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services)` [L:47]
  - Modifiers: public, static, this
  - Summary: Add EntityHookManager to the service collection. requires register  before add this
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.EntityHookManager.DependencyInjection.AddEntityHookManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services, Sharp.Shared.ISharedSystem shared)` [L:33]
  - Modifiers: public, static, this
  - Summary: Add EntityHookManager to the service collection.


### interface IEntityHookManager

- FullName: `Sharp.Extensions.EntityHookManager.IEntityHookManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Extensions/EntityHookManager/src/IEntityHookManager.cs:26
- Generated: false

#### Methods
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.HookEntityInput(string classname, string input, Sharp.Extensions.EntityHookManager.IEntityHookManager.InputDelegate callback)` [L:70]
  - Modifiers: public, abstract
  - Summary: Hook 实体IO中的 Input
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.HookEntityOutput(string classname, string output, Sharp.Extensions.EntityHookManager.IEntityHookManager.OutputDelegate callback)` [L:75]
  - Modifiers: public, abstract
  - Summary: Hook 实体IO中的 Output
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.ListenEntityCreate(string classname, Sharp.Extensions.EntityHookManager.IEntityHookManager.EventDelegate callback)` [L:50]
  - Modifiers: public, abstract
  - Summary: 监听实体创建事件
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.ListenEntityDelete(string classname, Sharp.Extensions.EntityHookManager.IEntityHookManager.EventDelegate callback)` [L:55]
  - Modifiers: public, abstract
  - Summary: 监听实体删除事件
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.ListenEntitySpawn(string classname, Sharp.Extensions.EntityHookManager.IEntityHookManager.EventDelegate callback)` [L:60]
  - Modifiers: public, abstract
  - Summary: 监听实体生成事件
- `void Sharp.Extensions.EntityHookManager.IEntityHookManager.ListenWeaponSpawn(Sharp.Extensions.EntityHookManager.IEntityHookManager.WeaponEventDelegate callback)` [L:65]
  - Modifiers: public, abstract
  - Summary: 监听武器生成事件


### delegate EventDelegate : System.MulticastDelegate

- FullName: `Sharp.Extensions.EntityHookManager.IEntityHookManager.EventDelegate`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/EntityHookManager/src/IEntityHookManager.cs:28
- Generated: false
- Invoke: `virtual void Sharp.Extensions.EntityHookManager.IEntityHookManager.EventDelegate.Invoke(string classname, Sharp.Shared.GameEntities.IBaseEntity entity)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **EventDelegate**


### delegate InputDelegate : System.MulticastDelegate

- FullName: `Sharp.Extensions.EntityHookManager.IEntityHookManager.InputDelegate`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/EntityHookManager/src/IEntityHookManager.cs:39
- Generated: false
- Invoke: `virtual void Sharp.Extensions.EntityHookManager.IEntityHookManager.InputDelegate.Invoke(string classname, string input, in Sharp.Shared.Types.EntityVariant value, Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller, ref Sharp.Shared.Enums.EHookAction result)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **InputDelegate**


### delegate OutputDelegate : System.MulticastDelegate

- FullName: `Sharp.Extensions.EntityHookManager.IEntityHookManager.OutputDelegate`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/EntityHookManager/src/IEntityHookManager.cs:32
- Generated: false
- Invoke: `virtual void Sharp.Extensions.EntityHookManager.IEntityHookManager.OutputDelegate.Invoke(string classname, string output, Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.GameEntities.IBaseEntity? activator, float delay, ref Sharp.Shared.Enums.EHookAction result)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **OutputDelegate**


### delegate WeaponEventDelegate : System.MulticastDelegate

- FullName: `Sharp.Extensions.EntityHookManager.IEntityHookManager.WeaponEventDelegate`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/EntityHookManager/src/IEntityHookManager.cs:30
- Generated: false
- Invoke: `virtual void Sharp.Extensions.EntityHookManager.IEntityHookManager.WeaponEventDelegate.Invoke(string classname, Sharp.Shared.GameEntities.IBaseWeapon weapon)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **WeaponEventDelegate**


