# Sharp.Extensions.GameEventManager

Project: Sharp.Extensions.GameEventManager
Types: 4 (0 generated)

### class DependencyInjection

- FullName: `Sharp.Extensions.GameEventManager.DependencyInjection`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Extensions/GameEventManager/src/DependencyInjection.cs:28
- Generated: false

Inheritance: object → **DependencyInjection**

#### Methods
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.GameEventManager.DependencyInjection.AddGameEventManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services)` [L:47]
  - Modifiers: public, static, this
  - Summary: Add GameEventManager to the service collection. requires register  before add this
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.GameEventManager.DependencyInjection.AddGameEventManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services, Sharp.Shared.ISharedSystem shared)` [L:33]
  - Modifiers: public, static, this
  - Summary: Add GameEventManager to the service collection.


### interface IGameEventManager

- FullName: `Sharp.Extensions.GameEventManager.IGameEventManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Extensions/GameEventManager/src/IGameEventManager.cs:25
- Generated: false

#### Methods
- `Sharp.Shared.Objects.IGameEvent? Sharp.Extensions.GameEventManager.IGameEventManager.CreateEvent(string eventName, bool force)` [L:46]
  - Modifiers: public, abstract
  - Summary: 创建游戏事件 通常需要手动销毁事件
- `T? Sharp.Extensions.GameEventManager.IGameEventManager.CloneEvent<T>(T e) where T : class, Sharp.Shared.Objects.IGameEvent` [L:58]
  - Modifiers: public, abstract
  - Summary: 克隆游戏事件 通常需要手动销毁事件
- `T? Sharp.Extensions.GameEventManager.IGameEventManager.CreateEvent<T>(bool force) where T : class, Sharp.Shared.Objects.IGameEvent` [L:52]
  - Modifiers: public, abstract
  - Summary: 创建游戏事件 通常需要手动销毁事件
- `void Sharp.Extensions.GameEventManager.IGameEventManager.HookEvent(string eventName, Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnHookEvent callback)` [L:35]
  - Modifiers: public, abstract
  - Summary: Hook 游戏事件发射 通常用于修改事件内容或阻止传播
- `void Sharp.Extensions.GameEventManager.IGameEventManager.ListenEvent(string eventName, Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnEventFired callback)` [L:40]
  - Modifiers: public, abstract
  - Summary: 监听游戏事件


### delegate DelegateOnEventFired : System.MulticastDelegate

- FullName: `Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnEventFired`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/GameEventManager/src/IGameEventManager.cs:27
- Generated: false
- Invoke: `virtual void Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnEventFired.Invoke(Sharp.Shared.Objects.IGameEvent e)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateOnEventFired**


### delegate DelegateOnHookEvent : System.MulticastDelegate

- FullName: `Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnHookEvent`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/GameEventManager/src/IGameEventManager.cs:29
- Generated: false
- Invoke: `virtual Sharp.Shared.Types.HookReturnValue<bool> Sharp.Extensions.GameEventManager.IGameEventManager.DelegateOnHookEvent.Invoke(Sharp.Shared.Objects.IGameEvent e, ref bool serverOnly)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateOnHookEvent**


