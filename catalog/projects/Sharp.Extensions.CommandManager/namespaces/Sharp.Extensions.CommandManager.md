# Sharp.Extensions.CommandManager

Project: Sharp.Extensions.CommandManager
Types: 4 (0 generated)

### class DependencyInjection

- FullName: `Sharp.Extensions.CommandManager.DependencyInjection`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Extensions/CommandManager/src/DependencyInjection.cs:28
- Generated: false

Inheritance: object → **DependencyInjection**

#### Methods
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.CommandManager.DependencyInjection.AddCommandManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services)` [L:47]
  - Modifiers: public, static, this
  - Summary: Add CommandManager to the service collection. requires register  before add this
- `static Microsoft.Extensions.DependencyInjection.IServiceCollection Sharp.Extensions.CommandManager.DependencyInjection.AddCommandManager(Microsoft.Extensions.DependencyInjection.IServiceCollection services, Sharp.Shared.ISharedSystem shared)` [L:33]
  - Modifiers: public, static, this
  - Summary: Add CommandManager to the service collection.


### interface ICommandManager

- FullName: `Sharp.Extensions.CommandManager.ICommandManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Extensions/CommandManager/src/ICommandManager.cs:26
- Generated: false

#### Methods
- `void Sharp.Extensions.CommandManager.ICommandManager.RegisterClientCommand(string command, Sharp.Extensions.CommandManager.ICommandManager.DelegateOnClientCommand callback)` [L:36]
  - Modifiers: public, abstract
  - Summary: 注册仅限客户端的控制台和聊天框命令 控制台会自动加上ms_前缀
- `void Sharp.Extensions.CommandManager.ICommandManager.RegisterServerCommand(string command, string description, Sharp.Extensions.CommandManager.ICommandManager.DelegateOnServerCommand callback)` [L:48]
  - Modifiers: public, abstract
  - Summary: 注册仅限服务端控制台执行的命令

#### Obsolete Members
- `void Sharp.Extensions.CommandManager.ICommandManager.RegisterAdminCommand(string command, Sharp.Extensions.CommandManager.ICommandManager.DelegateOnClientCommand callback, string permission)` [L:43] — This has been merged into AdminManager. Will be removed at 2.2


### delegate DelegateOnClientCommand : System.MulticastDelegate

- FullName: `Sharp.Extensions.CommandManager.ICommandManager.DelegateOnClientCommand`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/CommandManager/src/ICommandManager.cs:30
- Generated: false
- Invoke: `virtual void Sharp.Extensions.CommandManager.ICommandManager.DelegateOnClientCommand.Invoke(Sharp.Shared.Objects.IGameClient client, Sharp.Shared.Types.StringCommand command)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateOnClientCommand**


### delegate DelegateOnServerCommand : System.MulticastDelegate

- FullName: `Sharp.Extensions.CommandManager.ICommandManager.DelegateOnServerCommand`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Extensions/CommandManager/src/ICommandManager.cs:28
- Generated: false
- Invoke: `virtual void Sharp.Extensions.CommandManager.ICommandManager.DelegateOnServerCommand.Invoke(Sharp.Shared.Types.StringCommand command)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateOnServerCommand**


