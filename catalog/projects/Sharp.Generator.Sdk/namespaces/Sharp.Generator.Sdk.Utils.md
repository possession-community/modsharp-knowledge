# Sharp.Generator.Sdk.Utils

Project: Sharp.Generator.Sdk
Types: 6 (0 generated)

### class CodeWriter

- FullName: `Sharp.Generator.Sdk.Utils.CodeWriter`
- Kind: class
- Modifiers: public
- Source: Sharp.Generator.Sdk/Utils/CodeWriter.cs:25
- Generated: false

Inheritance: object → **CodeWriter**

#### Constructors
- `Sharp.Generator.Sdk.Utils.CodeWriter.CodeWriter()` [L:27]

#### Methods
- `System.IDisposable Sharp.Generator.Sdk.Utils.CodeWriter.BeginScope()` [L:50]
- `System.IDisposable Sharp.Generator.Sdk.Utils.CodeWriter.BeginScope(string line)` [L:43]
- `override string Sharp.Generator.Sdk.Utils.CodeWriter.ToString()` [L:70]
  - Modifiers: public, override
- `void Sharp.Generator.Sdk.Utils.CodeWriter.Append(string line)` [L:34]
- `void Sharp.Generator.Sdk.Utils.CodeWriter.AppendLine()` [L:40]
- `void Sharp.Generator.Sdk.Utils.CodeWriter.AppendLine(string line)` [L:37]
- `void Sharp.Generator.Sdk.Utils.CodeWriter.EndLine()` [L:58]
- `void Sharp.Generator.Sdk.Utils.CodeWriter.EndScope()` [L:61]
- `void Sharp.Generator.Sdk.Utils.CodeWriter.StartLine()` [L:67]


### class MethodSymbolExtensions

- FullName: `Sharp.Generator.Sdk.Utils.MethodSymbolExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Generator.Sdk/Utils/Extensions.cs:285
- Generated: false

Inheritance: object → **MethodSymbolExtensions**

#### Methods
- `static Sharp.Generator.Sdk.Utils.MethodSymbolParamContext Sharp.Generator.Sdk.Utils.MethodSymbolExtensions.GetParams(Microsoft.CodeAnalysis.IMethodSymbol symbol)` [L:287]
  - Modifiers: public, static, this


### class MethodSymbolParam

- FullName: `Sharp.Generator.Sdk.Utils.MethodSymbolParam`
- Kind: class
- Modifiers: public
- Source: Sharp.Generator.Sdk/Utils/Extensions.cs:84
- Generated: false

Inheritance: object → **MethodSymbolParam**

#### Properties
- `bool Sharp.Generator.Sdk.Utils.MethodSymbolParam.IsNativeObject` [L:90]
- `bool Sharp.Generator.Sdk.Utils.MethodSymbolParam.IsRef` [L:91]
- `int Sharp.Generator.Sdk.Utils.MethodSymbolParam.Utf8Size` [L:89]
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParam.Name` [L:86]
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParam.Type` [L:87]
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParam.UnmanagedType` [L:88]


### class MethodSymbolParamContext

- FullName: `Sharp.Generator.Sdk.Utils.MethodSymbolParamContext`
- Kind: class
- Modifiers: public
- Source: Sharp.Generator.Sdk/Utils/Extensions.cs:94
- Generated: false

Inheritance: object → **MethodSymbolParamContext**

#### Constructors
- `Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.MethodSymbolParamContext(System.Collections.Generic.List<Sharp.Generator.Sdk.Utils.MethodSymbolParam> @params, string returnType)` [L:99]

#### Properties
- `System.Collections.Generic.List<Sharp.Generator.Sdk.Utils.MethodSymbolParam> Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.Params` [L:96]
  - Modifiers: public, readonly
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.ReturnType` [L:97]
  - Modifiers: public, readonly

#### Methods
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.GetCallDelegateUnmanagedPointerArgsString([string? prefixParam = null])` [L:148]
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.GetDelegateUnmanagedPointerString([string? prefixParam = null])` [L:117]
- `string Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.GetParametersString([string? prefixParam = null])` [L:105]
- `void Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.BuildCallAndReturnDelegateUnmanagedPointer(Sharp.Generator.Sdk.Utils.CodeWriter builder, string methodName, [string? prefixParam = null])` [L:177]
- `void Sharp.Generator.Sdk.Utils.MethodSymbolParamContext.BuildUtf8ConvertCode(Sharp.Generator.Sdk.Utils.CodeWriter builder)` [L:228]


### class NamedTypeSymbolExtensions

- FullName: `Sharp.Generator.Sdk.Utils.NamedTypeSymbolExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Generator.Sdk/Utils/Extensions.cs:27
- Generated: false

Inheritance: object → **NamedTypeSymbolExtensions**

#### Methods
- `static Microsoft.CodeAnalysis.INamedTypeSymbol? Sharp.Generator.Sdk.Utils.NamedTypeSymbolExtensions.GetFinalBaseType(Microsoft.CodeAnalysis.INamedTypeSymbol symbol)` [L:29]
  - Modifiers: public, static, this
- `static bool Sharp.Generator.Sdk.Utils.NamedTypeSymbolExtensions.IsAssignableFrom(Microsoft.CodeAnalysis.INamedTypeSymbol symbol, string name)` [L:43]
  - Modifiers: public, static, this


### class SyntaxNodeExtensions

- FullName: `Sharp.Generator.Sdk.Utils.SyntaxNodeExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Generator.Sdk/Utils/Extensions.cs:71
- Generated: false

Inheritance: object → **SyntaxNodeExtensions**

#### Methods
- `static string Sharp.Generator.Sdk.Utils.SyntaxNodeExtensions.GetNameSpace(Microsoft.CodeAnalysis.SyntaxNode syntax)` [L:73]
  - Modifiers: public, static, this


