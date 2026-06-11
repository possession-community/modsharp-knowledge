# Sharp.Shared.Types

Project: Sharp.Shared
Types: 44 (0 generated)

### struct CEntityHandle<T> : System.ValueType, System.IEquatable<Sharp.Shared.Types.CEntityHandle<T>>, System.IEquatable<uint>

- FullName: `Sharp.Shared.Types.CEntityHandle<T>`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/CEntityHandle.cs:28
- Generated: false
- Attributes: `[StructLayout(0, Size = 4)]`
- Constraint: `where T : class, Sharp.Shared.GameEntities.IBaseEntity`

Inheritance: object → System.ValueType → **CEntityHandle**

#### Constructors
- `Sharp.Shared.Types.CEntityHandle<T>.CEntityHandle([uint value = 4294967295])` [L:34]
- `Sharp.Shared.Types.CEntityHandle<T>.CEntityHandle(int index, int serial)` [L:37]

#### Methods
- `Sharp.Shared.Types.CEntityHandle<TOut> Sharp.Shared.Types.CEntityHandle<T>.As<TOut>() where TOut : class, Sharp.Shared.GameEntities.IBaseEntity` [L:66]
  - Modifiers: public, readonly
  - Summary: Casts the handle to a different entity type.
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.Types.CEntityHandle<T>.GetEntryIndex()` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Types.CEntityHandle<T>.Equals(Sharp.Shared.Types.CEntityHandle<T> other)` [L:100]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Types.CEntityHandle<T>.Equals(uint other)` [L:84]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Types.CEntityHandle<T>.IsValid()` [L:40]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.CEntityHandle<T>.GetEHandleInt()` [L:59]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.CEntityHandle<T>.GetSerialNum()` [L:53]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Types.CEntityHandle<T>.Equals(object? obj)` [L:87]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Types.CEntityHandle<T>.GetHashCode()` [L:97]
  - Modifiers: public, override, readonly
- `static Sharp.Shared.Types.CEntityHandle<T> Sharp.Shared.Types.CEntityHandle<T>.FromPackedValue(uint packed)` [L:122]
  - Modifiers: public, static
  - Summary: Reconstructs a CEntityHandle from a compressed 24-bit integer.
- `uint Sharp.Shared.Types.CEntityHandle<T>.GetPackedValue()` [L:107]
  - Modifiers: public, readonly
  - Summary: Compresses the handle into a 24-bit integer (Index + Truncated Serial).
- `uint Sharp.Shared.Types.CEntityHandle<T>.GetValue()` [L:56]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.CEntityHandle<T>.implicit operator Sharp.Shared.Types.CEntityHandle<T>(uint e)` [L:69]
  - Modifiers: public, static
- `static Sharp.Shared.Types.CEntityHandle<T>.implicit operator uint(Sharp.Shared.Types.CEntityHandle<T> e)` [L:72]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.CEntityHandle<T>.operator !=(Sharp.Shared.Types.CEntityHandle<T> left, Sharp.Shared.Types.CEntityHandle<T> right)` [L:78]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.CEntityHandle<T>.operator ==(Sharp.Shared.Types.CEntityHandle<T> left, Sharp.Shared.Types.CEntityHandle<T> right)` [L:75]
  - Modifiers: public, static


### struct CInButtonState : System.ValueType

- FullName: `Sharp.Shared.Types.CInButtonState`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CInButtonState.cs:26
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 32)]`

Inheritance: object → System.ValueType → **CInButtonState**

#### Fields
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CInButtonState.ButtonChanged` [L:32]
  - Attributes: `[FieldOffset(16)]`
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CInButtonState.ButtonPressed` [L:29]
  - Attributes: `[FieldOffset(8)]`
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CInButtonState.ButtonScroll` [L:35]
  - Attributes: `[FieldOffset(24)]`


### struct CTraceFilter : System.ValueType

- FullName: `Sharp.Shared.Types.CTraceFilter`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/CTraceFilter.cs:25
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 72)]`

Inheritance: object → System.ValueType → **CTraceFilter**

#### Fields
- `Sharp.Shared.Types.CTraceFilterVirtualTableDescriptor* Sharp.Shared.Types.CTraceFilter.Vtable` [L:28]
  - Attributes: `[FieldOffset(0)]`
- `Sharp.Shared.Types.RnQueryShapeAttr Sharp.Shared.Types.CTraceFilter.QueryAttribute` [L:31]
  - Attributes: `[FieldOffset(8)]`
- `bool Sharp.Shared.Types.CTraceFilter.m_bIterateEntities` [L:34]
  - Attributes: `[FieldOffset(64)]`


### struct CTraceFilterVirtualTableDescriptor : System.ValueType

- FullName: `Sharp.Shared.Types.CTraceFilterVirtualTableDescriptor`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CTraceFilter.cs:37
- Generated: false

Inheritance: object → System.ValueType → **CTraceFilterVirtualTableDescriptor**

#### Fields
- `delegate* unmanaged<Sharp.Shared.Types.CTraceFilter*, nint, bool> Sharp.Shared.Types.CTraceFilterVirtualTableDescriptor.ShouldHitEntity` [L:40]
- `delegate* unmanaged<nint, void> Sharp.Shared.Types.CTraceFilterVirtualTableDescriptor.Deconstructor` [L:39]


### struct CUserCmd : System.ValueType

- FullName: `Sharp.Shared.Types.CUserCmd`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/CUserCmd.cs:26
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 144)]`

Inheritance: object → System.ValueType → **CUserCmd**

#### Fields
- `Sharp.Shared.Types.CInButtonState Sharp.Shared.Types.CUserCmd.ButtonState` [L:35]
  - Attributes: `[FieldOffset(88)]`
- `Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb Sharp.Shared.Types.CUserCmd.CSGOUserCmd` [L:32]
  - Attributes: `[FieldOffset(16)]`
- `uint Sharp.Shared.Types.CUserCmd.CommandNumber` [L:29]
  - Attributes: `[FieldOffset(8)]`


### struct Color : System.ValueType, System.IEquatable<Sharp.Shared.Types.Color>

- FullName: `Sharp.Shared.Types.Color`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Color.cs:26
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **Color**

#### Constructors
- `Sharp.Shared.Types.Color.Color(byte r, byte g, byte b)` [L:32]

#### Properties
- `byte Sharp.Shared.Types.Color.B` [L:30]
- `byte Sharp.Shared.Types.Color.G` [L:29]
- `byte Sharp.Shared.Types.Color.R` [L:28]

#### Indexers
- `byte Sharp.Shared.Types.Color.this[int key]` [L:55]

#### Methods
- `bool Sharp.Shared.Types.Color.Equals(Sharp.Shared.Types.Color other)` [L:93]
- `override bool Sharp.Shared.Types.Color.Equals(object? obj)` [L:42]
  - Modifiers: public, override
- `override int Sharp.Shared.Types.Color.GetHashCode()` [L:52]
  - Modifiers: public, override
- `readonly bool Sharp.Shared.Types.Color.Same(Sharp.Shared.Types.Color32 other)` [L:39]
  - Modifiers: public, readonly

#### Operators
- `static bool Sharp.Shared.Types.Color.operator !=(Sharp.Shared.Types.Color a, Sharp.Shared.Types.Color b)` [L:90]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Color.operator ==(Sharp.Shared.Types.Color a, Sharp.Shared.Types.Color b)` [L:87]
  - Modifiers: public, static


### struct Color32 : System.ValueType, System.IEquatable<Sharp.Shared.Types.Color32>

- FullName: `Sharp.Shared.Types.Color32`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Color.cs:100
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **Color32**

#### Constructors
- `Sharp.Shared.Types.Color32.Color32(byte r, byte g, byte b, byte a)` [L:107]

#### Properties
- `byte Sharp.Shared.Types.Color32.A` [L:105]
- `byte Sharp.Shared.Types.Color32.B` [L:104]
- `byte Sharp.Shared.Types.Color32.G` [L:103]
- `byte Sharp.Shared.Types.Color32.R` [L:102]

#### Indexers
- `byte Sharp.Shared.Types.Color32.this[int key]` [L:131]

#### Methods
- `bool Sharp.Shared.Types.Color32.Equals(Sharp.Shared.Types.Color32 other)` [L:177]
- `override bool Sharp.Shared.Types.Color32.Equals(object? obj)` [L:118]
  - Modifiers: public, override
- `override int Sharp.Shared.Types.Color32.GetHashCode()` [L:128]
  - Modifiers: public, override
- `readonly bool Sharp.Shared.Types.Color32.Same(Sharp.Shared.Types.Color32 other)` [L:115]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.Color32.implicit operator uint(Sharp.Shared.Types.Color32 color)` [L:174]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Color32.operator !=(Sharp.Shared.Types.Color32 a, Sharp.Shared.Types.Color32 b)` [L:171]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Color32.operator ==(Sharp.Shared.Types.Color32 a, Sharp.Shared.Types.Color32 b)` [L:168]
  - Modifiers: public, static


### struct ConVarVariantValue : System.ValueType

- FullName: `Sharp.Shared.Types.ConVarVariantValue`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/ConVarVariantValue.cs:27
- Generated: false
- Attributes: `[StructLayout(2)]`

Inheritance: object → System.ValueType → **ConVarVariantValue**

#### Constructors
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(Sharp.Shared.Types.Color value)` [L:101]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(Sharp.Shared.Types.Vector value)` [L:107]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(Sharp.Shared.Types.Vector2D value)` [L:104]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(Sharp.Shared.Types.Vector4D value)` [L:110]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(bool value)` [L:71]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(double value)` [L:95]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(float value)` [L:92]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(int value)` [L:80]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(long value)` [L:86]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(nint value)` [L:98]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(short value)` [L:74]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(uint value)` [L:83]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(ulong value)` [L:89]
- `Sharp.Shared.Types.ConVarVariantValue.ConVarVariantValue(ushort value)` [L:77]

#### Properties
- `Sharp.Shared.Types.Color Sharp.Shared.Types.ConVarVariantValue.AsColor` [L:169]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.ConVarVariantValue.AsVector3D` [L:181]
- `Sharp.Shared.Types.Vector2D Sharp.Shared.Types.ConVarVariantValue.AsVector2D` [L:175]
- `Sharp.Shared.Types.Vector4D Sharp.Shared.Types.ConVarVariantValue.AsVector4D` [L:187]
- `bool Sharp.Shared.Types.ConVarVariantValue.AsBool` [L:113]
- `double Sharp.Shared.Types.ConVarVariantValue.AsDouble` [L:161]
- `float Sharp.Shared.Types.ConVarVariantValue.AsFloat` [L:155]
- `int Sharp.Shared.Types.ConVarVariantValue.AsInt32` [L:131]
- `long Sharp.Shared.Types.ConVarVariantValue.AsInt64` [L:143]
- `short Sharp.Shared.Types.ConVarVariantValue.AsInt16` [L:119]
- `string Sharp.Shared.Types.ConVarVariantValue.AsString` [L:167]
  - Modifiers: public, readonly
- `uint Sharp.Shared.Types.ConVarVariantValue.AsUInt32` [L:137]
- `ulong Sharp.Shared.Types.ConVarVariantValue.AsUInt64` [L:149]
- `ushort Sharp.Shared.Types.ConVarVariantValue.AsUInt16` [L:125]

#### Operators
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(bool value)` [L:193]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(double value)` [L:217]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(float value)` [L:214]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(int value)` [L:202]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(long value)` [L:208]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(short value)` [L:196]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(uint value)` [L:205]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(ulong value)` [L:211]
  - Modifiers: public, static
- `static Sharp.Shared.Types.ConVarVariantValue.implicit operator Sharp.Shared.Types.ConVarVariantValue(ushort value)` [L:199]
  - Modifiers: public, static


### struct EntityVariant : System.ValueType

- FullName: `Sharp.Shared.Types.EntityVariant`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/EntityVariant.cs:31
- Generated: false
- Attributes: `[StructLayout(2)]`

Inheritance: object → System.ValueType → **EntityVariant**

#### Properties
- `readonly Sharp.Shared.Enums.VariantFieldType Sharp.Shared.Types.EntityVariant.Type` [L:51]
  - Modifiers: public, readonly
- `readonly bool Sharp.Shared.Types.EntityVariant.AsBool` [L:63]
  - Modifiers: public, readonly
- `readonly float Sharp.Shared.Types.EntityVariant.AsFloat` [L:62]
  - Modifiers: public, readonly
- `readonly int Sharp.Shared.Types.EntityVariant.AsInt32` [L:61]
  - Modifiers: public, readonly
- `readonly string Sharp.Shared.Types.EntityVariant.AsString` [L:53]
  - Modifiers: public, readonly

#### Methods
- `override string Sharp.Shared.Types.EntityVariant.ToString()` [L:77]
  - Modifiers: public, override
- `readonly string Sharp.Shared.Types.EntityVariant.AutoCastString()` [L:92]
  - Modifiers: public, readonly
  - Summary: In IO triggered by VScript, the Type is labeled as String, but the actual data used is CString.


### struct FireBulletInfo : System.ValueType

- FullName: `Sharp.Shared.Types.FireBulletInfo`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/FireBulletInfo.cs:25
- Generated: false
- Attributes: `[StructLayout(2, Pack = 4, Size = 56)]`

Inheritance: object → System.ValueType → **FireBulletInfo**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.FireBulletInfo.ShootAngles` [L:31]
  - Attributes: `[FieldOffset(12)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.FireBulletInfo.ShootPosition` [L:28]
  - Attributes: `[FieldOffset(0)]`
- `float Sharp.Shared.Types.FireBulletInfo.Penetration` [L:40]
  - Attributes: `[FieldOffset(32)]`
- `float Sharp.Shared.Types.FireBulletInfo.Range` [L:34]
  - Attributes: `[FieldOffset(24)]`
- `float Sharp.Shared.Types.FireBulletInfo.RangeModifier` [L:37]
  - Attributes: `[FieldOffset(28)]`
- `float Sharp.Shared.Types.FireBulletInfo.SpreadX` [L:52]
  - Attributes: `[FieldOffset(48)]`
- `float Sharp.Shared.Types.FireBulletInfo.SpreadY` [L:55]
  - Attributes: `[FieldOffset(52)]`
- `int Sharp.Shared.Types.FireBulletInfo.CurrentBullet` [L:49]
  - Attributes: `[FieldOffset(44)]`
- `int Sharp.Shared.Types.FireBulletInfo.Damage` [L:46]
  - Attributes: `[FieldOffset(40)]`
- `int Sharp.Shared.Types.FireBulletInfo.PenetrationCount` [L:43]
  - Attributes: `[FieldOffset(36)]`


### struct GameTrace : System.ValueType

- FullName: `Sharp.Shared.Types.GameTrace`
- Kind: struct
- Modifiers: public, readonly, ref
- Source: Sharp.Shared/Types/GameTrace.cs:66
- Generated: false
- Attributes: `[StructLayout(2)]`
- Summary: CGameTrace must be readonly, changing it can cause crashes

Inheritance: object → System.ValueType → **GameTrace**

#### Fields
- `readonly Sharp.Shared.Enums.TraceRayType Sharp.Shared.Types.GameTrace.RayType` [L:114]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(182)]`
- `readonly Sharp.Shared.Types.HitBoxData* Sharp.Shared.Types.GameTrace.HitBoxData` [L:75]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(16)]`
- `readonly Sharp.Shared.Types.PhysicsSurfaceProperties* Sharp.Shared.Types.GameTrace.SurfaceProp` [L:69]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Types.RnCollisionAttr Sharp.Shared.Types.GameTrace.ShapeAttributes` [L:87]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(80)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.GameTrace.EndPosition` [L:93]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(132)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.GameTrace.HitPoint` [L:99]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(156)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.GameTrace.PlaneNormal` [L:96]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(144)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.GameTrace.StartPosition` [L:90]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(120)]`
- `readonly bool Sharp.Shared.Types.GameTrace.ExactHitPoint` [L:120]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(184)]`
- `readonly bool Sharp.Shared.Types.GameTrace.StartInSolid` [L:117]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(183)]`
- `readonly float Sharp.Shared.Types.GameTrace.Fraction` [L:105]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(172)]`
- `readonly float Sharp.Shared.Types.GameTrace.HitOffset` [L:102]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(168)]`
- `readonly float Sharp.Shared.Types.GameTrace.Triangle` [L:108]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(176)]`
- `readonly nint Sharp.Shared.Types.GameTrace.Entity` [L:72]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(8)]`
- `readonly nint Sharp.Shared.Types.GameTrace.PhysicsBody` [L:78]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(24)]`
- `readonly nint Sharp.Shared.Types.GameTrace.PhysicsShape` [L:81]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(32)]`
- `readonly short Sharp.Shared.Types.GameTrace.HitBoxBoneIndex` [L:111]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(180)]`
- `readonly uint Sharp.Shared.Types.GameTrace.Contents` [L:84]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(40)]`

#### Methods
- `bool Sharp.Shared.Types.GameTrace.DidHit()` [L:122]
  - Modifiers: public, readonly


### struct HitBoxData : System.ValueType

- FullName: `Sharp.Shared.Types.HitBoxData`
- Kind: struct
- Modifiers: public, readonly, ref
- Source: Sharp.Shared/Types/GameTrace.cs:127
- Generated: false
- Attributes: `[StructLayout(2)]`

Inheritance: object → System.ValueType → **HitBoxData**

#### Fields
- `readonly Sharp.Shared.Enums.HitGroupType Sharp.Shared.Types.HitBoxData.HitGroup` [L:133]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(56)]`
- `readonly int Sharp.Shared.Types.HitBoxData.HitBoxId` [L:136]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(72)]`
- `readonly sbyte* Sharp.Shared.Types.HitBoxData.pName` [L:130]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`


### record struct HookReturnValue<T> : System.ValueType, System.IEquatable<Sharp.Shared.Types.HookReturnValue<T>>

- FullName: `Sharp.Shared.Types.HookReturnValue<T>`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/HookReturnValue.cs:24
- Generated: false

Inheritance: object → System.ValueType → **HookReturnValue**

#### Constructors
- `Sharp.Shared.Types.HookReturnValue<T>.HookReturnValue(Sharp.Shared.Enums.EHookAction action)` [L:34]
- `Sharp.Shared.Types.HookReturnValue<T>.HookReturnValue(Sharp.Shared.Enums.EHookAction action, T? returnValue)` [L:40]

#### Properties
- `Sharp.Shared.Enums.EHookAction Sharp.Shared.Types.HookReturnValue<T>.Action` [L:27]
  - Modifiers: public, readonly
- `T? Sharp.Shared.Types.HookReturnValue<T>.ReturnValue` [L:32]
  - Modifiers: public, readonly
  - Summary: Return value, void when EmptyHookReturn


### struct KeyValuesVariantValueItem : System.ValueType

- FullName: `Sharp.Shared.Types.KeyValuesVariantValueItem`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/KeyValuesVariantItem.cs:25
- Generated: false

Inheritance: object → System.ValueType → **KeyValuesVariantValueItem**

#### Constructors
- `Sharp.Shared.Types.KeyValuesVariantValueItem.KeyValuesVariantValueItem(bool value)` [L:50]
- `Sharp.Shared.Types.KeyValuesVariantValueItem.KeyValuesVariantValueItem(float value)` [L:62]
- `Sharp.Shared.Types.KeyValuesVariantValueItem.KeyValuesVariantValueItem(int value)` [L:56]
- `Sharp.Shared.Types.KeyValuesVariantValueItem.KeyValuesVariantValueItem(nint value)` [L:68]
- `Sharp.Shared.Types.KeyValuesVariantValueItem.KeyValuesVariantValueItem(string value)` [L:74]

#### Fields
- `Sharp.Shared.Enums.EntityKeyValuesVariantType Sharp.Shared.Types.KeyValuesVariantValueItem.Type` [L:27]

#### Properties
- `bool Sharp.Shared.Types.KeyValuesVariantValueItem.BoolValue` [L:80]
  - Modifiers: public, readonly
- `float Sharp.Shared.Types.KeyValuesVariantValueItem.FloatValue` [L:84]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.KeyValuesVariantValueItem.IntValue` [L:82]
  - Modifiers: public, readonly
- `nint Sharp.Shared.Types.KeyValuesVariantValueItem.PointerValue` [L:90]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.KeyValuesVariantValueItem.StringValue` [L:87]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.KeyValuesVariantValueItem.implicit operator Sharp.Shared.Types.KeyValuesVariantValueItem(bool value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Types.KeyValuesVariantValueItem.implicit operator Sharp.Shared.Types.KeyValuesVariantValueItem(float value)` [L:41]
  - Modifiers: public, static
- `static Sharp.Shared.Types.KeyValuesVariantValueItem.implicit operator Sharp.Shared.Types.KeyValuesVariantValueItem(int value)` [L:35]
  - Modifiers: public, static
- `static Sharp.Shared.Types.KeyValuesVariantValueItem.implicit operator Sharp.Shared.Types.KeyValuesVariantValueItem(nint value)` [L:47]
  - Modifiers: public, static
- `static Sharp.Shared.Types.KeyValuesVariantValueItem.implicit operator Sharp.Shared.Types.KeyValuesVariantValueItem(string value)` [L:44]
  - Modifiers: public, static


### struct Matrix3x4 : System.ValueType

- FullName: `Sharp.Shared.Types.Matrix3x4`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Matrix3X4.cs:29
- Generated: false
- Attributes: `[InlineArray(3)]` `[StructLayout(0, Pack = 4)]`

Inheritance: object → System.ValueType → **Matrix3x4**

#### Methods
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Matrix3x4.GetAngles()` [L:42]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Matrix3x4.GetOrigin()` [L:39]
- `static float Sharp.Shared.Types.Matrix3x4.Rad2Deg(float x)` [L:91]
  - Modifiers: public, static


### struct Row : System.ValueType

- FullName: `Sharp.Shared.Types.Matrix3x4.Row`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Matrix3X4.cs:32
- Generated: false
- Attributes: `[InlineArray(4)]`

Inheritance: object → System.ValueType → **Row**


### struct MoveData : System.ValueType

- FullName: `Sharp.Shared.Types.MoveData`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/MoveData.cs:28
- Generated: false
- Attributes: `[StructLayout(2, Pack = 1)]`

Inheritance: object → System.ValueType → **MoveData**

#### Fields
- `Sharp.Shared.Types.Tier.CUtlVector<Sharp.Shared.Types.SubTickAttack> Sharp.Shared.Types.MoveData.SubTickAttacks` [L:65]
  - Attributes: `[FieldOffset(120)]`
- `Sharp.Shared.Types.Tier.CUtlVector<Sharp.Shared.Types.SubTickMove> Sharp.Shared.Types.MoveData.SubTickMoves` [L:62]
  - Attributes: `[FieldOffset(96)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.AbsOrigin` [L:68]
  - Attributes: `[FieldOffset(200)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.AbsViewAngles` [L:38]
  - Attributes: `[FieldOffset(8)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.Angles` [L:59]
  - Attributes: `[FieldOffset(68)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.LastMovementImpulses` [L:44]
  - Attributes: `[FieldOffset(32)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.Velocity` [L:56]
  - Attributes: `[FieldOffset(56)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.ViewAngles` [L:41]
  - Attributes: `[FieldOffset(20)]`
- `byte Sharp.Shared.Types.MoveData.MoveDataFlags` [L:35]
  - Attributes: `[FieldOffset(0)]`
- `float Sharp.Shared.Types.MoveData.ForwardMove` [L:47]
  - Attributes: `[FieldOffset(44)]`
- `float Sharp.Shared.Types.MoveData.SideMove` [L:50]
  - Attributes: `[FieldOffset(48)]`
- `float Sharp.Shared.Types.MoveData.UpMove` [L:53]
  - Attributes: `[FieldOffset(52)]`

#### Properties
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.MoveData.OutWishVel` [L:81]
- `bool Sharp.Shared.Types.MoveData.InAir` [L:99]
- `float Sharp.Shared.Types.MoveData.ClientMaxSpeed` [L:93]
- `float Sharp.Shared.Types.MoveData.MaxSpeed` [L:87]


### struct PhysicsSurfaceProperties : System.ValueType

- FullName: `Sharp.Shared.Types.PhysicsSurfaceProperties`
- Kind: struct
- Modifiers: public, readonly, ref
- Source: Sharp.Shared/Types/GameTrace.cs:140
- Generated: false
- Attributes: `[StructLayout(2)]`

Inheritance: object → System.ValueType → **PhysicsSurfaceProperties**

#### Fields
- `readonly sbyte* Sharp.Shared.Types.PhysicsSurfaceProperties.pName` [L:143]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`


### struct Pointer<T> : System.ValueType

- FullName: `Sharp.Shared.Types.Pointer<T>`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Pointer.cs:26
- Generated: false
- Attributes: `[StructLayout(0)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **Pointer**

#### Fields
- `T* Sharp.Shared.Types.Pointer<T>.Value` [L:28]

#### Methods
- `ref T Sharp.Shared.Types.Pointer<T>.AsRef()` [L:30]

#### Operators
- `static Sharp.Shared.Types.Pointer<T>.implicit operator Sharp.Shared.Types.Pointer<T>(T* value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Pointer<T>.implicit operator Sharp.Shared.Types.Pointer<T>(nint value)` [L:36]
  - Modifiers: public, static


### struct RecipientFilter : System.ValueType

- FullName: `Sharp.Shared.Types.RecipientFilter`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/RecipientFilter.cs:32
- Generated: false
- Attributes: `[StructLayout(2, Pack = 16, Size = 16)]`

Inheritance: object → System.ValueType → **RecipientFilter**

#### Constructors
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter()` [L:109]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.Enums.CStrikeTeam team)` [L:46]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.GameEntities.IPlayerController controller)` [L:67]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.Objects.IGameClient client)` [L:60]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.Units.EntityIndex index)` [L:74]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.Units.NetworkReceiver receiver)` [L:81]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(Sharp.Shared.Units.PlayerSlot slot)` [L:53]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> players)` [L:102]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(System.Collections.Generic.IEnumerable<Sharp.Shared.Units.PlayerSlot> players)` [L:88]
- `Sharp.Shared.Types.RecipientFilter.RecipientFilter(System.Collections.Generic.IReadOnlyCollection<Sharp.Shared.Units.PlayerSlot> players)` [L:95]

#### Fields
- `readonly Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.Types.RecipientFilter.Team` [L:38]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(4)]`
- `readonly Sharp.Shared.Enums.RecipientFilterType Sharp.Shared.Types.RecipientFilter.Type` [L:35]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Units.NetworkReceiver Sharp.Shared.Types.RecipientFilter.Receivers` [L:41]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(8)]`
- `readonly ulong Sharp.Shared.Types.RecipientFilter.ReceiverSlot` [L:44]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(8)]`

#### Methods
- `bool Sharp.Shared.Types.RecipientFilter.IsEmpty()` [L:116]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.RecipientFilter.DestructureTransform()` [L:133]
  - Modifiers: public, readonly


### struct ResponseContext : System.ValueType

- FullName: `Sharp.Shared.Types.ResponseContext`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/ResponseContext.cs:26
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 24)]`

Inheritance: object → System.ValueType → **ResponseContext**

#### Fields
- `float Sharp.Shared.Types.ResponseContext.ExpirationTime` [L:35]
  - Attributes: `[FieldOffset(16)]`
- `sbyte* Sharp.Shared.Types.ResponseContext.pName` [L:29]
  - Attributes: `[FieldOffset(0)]`
- `sbyte* Sharp.Shared.Types.ResponseContext.pValue` [L:32]
  - Attributes: `[FieldOffset(8)]`

#### Properties
- `string Sharp.Shared.Types.ResponseContext.Name` [L:37]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.ResponseContext.Value` [L:39]
  - Modifiers: public, readonly


### struct RnCollisionAttr : System.ValueType

- FullName: `Sharp.Shared.Types.RnCollisionAttr`
- Kind: struct
- Modifiers: public, readonly, ref
- Source: Sharp.Shared/Types/GameTrace.cs:26
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 40)]`

Inheritance: object → System.ValueType → **RnCollisionAttr**

#### Fields
- `readonly Sharp.Shared.Enums.CollisionGroupType Sharp.Shared.Types.RnCollisionAttr.CollisionGroup` [L:56]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(38)]`
- `readonly Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnCollisionAttr.InteractsAs` [L:29]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnCollisionAttr.InteractsExclude` [L:35]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(16)]`
- `readonly Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnCollisionAttr.InteractsWith` [L:32]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(8)]`
- `readonly byte Sharp.Shared.Types.RnCollisionAttr.CollisionFunctionMask` [L:59]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(39)]`
- `readonly byte Sharp.Shared.Types.RnCollisionAttr.DetailLayerMaskType` [L:50]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(36)]`
- `readonly byte Sharp.Shared.Types.RnCollisionAttr.TargetDetailLayer` [L:53]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(37)]`
- `readonly uint Sharp.Shared.Types.RnCollisionAttr.EntityId` [L:38]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(24)]`
- `readonly uint Sharp.Shared.Types.RnCollisionAttr.OwnerId` [L:41]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(28)]`
- `readonly ushort Sharp.Shared.Types.RnCollisionAttr.DetailLayerMask` [L:47]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(34)]`
- `readonly ushort Sharp.Shared.Types.RnCollisionAttr.HierarchyId` [L:44]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(32)]`


### struct RnQueryShapeAttr : System.ValueType

- FullName: `Sharp.Shared.Types.RnQueryShapeAttr`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/RnQueryShapeAttr.cs:29
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 56)]`

Inheritance: object → System.ValueType → **RnQueryShapeAttr**

#### Constructors
- `Sharp.Shared.Types.RnQueryShapeAttr.RnQueryShapeAttr()` [L:64]

#### Fields
- `Sharp.Shared.Enums.CollisionGroupType Sharp.Shared.Types.RnQueryShapeAttr.m_nCollisionGroup` [L:59]
  - Attributes: `[FieldOffset(48)]`
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnQueryShapeAttr.m_nInteractsAs` [L:38]
  - Attributes: `[FieldOffset(16)]`
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnQueryShapeAttr.m_nInteractsExclude` [L:35]
  - Attributes: `[FieldOffset(8)]`
- `Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Types.RnQueryShapeAttr.m_nInteractsWith` [L:32]
  - Attributes: `[FieldOffset(0)]`
- `Sharp.Shared.Enums.RnQueryObjectSet Sharp.Shared.Types.RnQueryShapeAttr.m_nObjectSetMask` [L:56]
  - Attributes: `[FieldOffset(47)]`
- `uint* Sharp.Shared.Types.RnQueryShapeAttr.m_nEntityIdsToIgnore` [L:41]
  - Attributes: `[FieldOffset(24)]`
- `uint* Sharp.Shared.Types.RnQueryShapeAttr.m_nOwnerIdsToIgnore` [L:44]
  - Attributes: `[FieldOffset(32)]`
- `ushort* Sharp.Shared.Types.RnQueryShapeAttr.m_nHierarchyIds` [L:47]
  - Attributes: `[FieldOffset(40)]`

#### Properties
- `bool Sharp.Shared.Types.RnQueryShapeAttr.ForceHitEverything` [L:194]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.HitSolid` [L:114]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.HitSolidRequiresGenerateContacts` [L:130]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.HitTrigger` [L:146]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.IgnoreIfBothInteractWithHitBoxes` [L:178]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.ShouldIgnoreDisabledPairs` [L:162]
- `bool Sharp.Shared.Types.RnQueryShapeAttr.Unknown` [L:210]

#### Methods
- `static Sharp.Shared.Types.RnQueryShapeAttr Sharp.Shared.Types.RnQueryShapeAttr.Bullets()` [L:240]
  - Modifiers: public, static
- `static Sharp.Shared.Types.RnQueryShapeAttr Sharp.Shared.Types.RnQueryShapeAttr.Knife()` [L:253]
  - Modifiers: public, static
- `static Sharp.Shared.Types.RnQueryShapeAttr Sharp.Shared.Types.RnQueryShapeAttr.PlayerMovement(Sharp.Shared.Enums.InteractionLayers interactsWithLayers)` [L:226]
  - Modifiers: public, static
- `void Sharp.Shared.Types.RnQueryShapeAttr.SetEntityToIgnore(Sharp.Shared.GameEntities.IBaseEntity entityToIgnore, int index)` [L:81]


### struct ShootInfo : System.ValueType

- FullName: `Sharp.Shared.Types.ShootInfo`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/ShootInfo.cs:25
- Generated: false
- Attributes: `[StructLayout(2, Pack = 4, Size = 88)]`

Inheritance: object → System.ValueType → **ShootInfo**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.ShootInfo.AttackAngles` [L:46]
  - Attributes: `[FieldOffset(32)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.ShootInfo.AttackPos` [L:43]
  - Attributes: `[FieldOffset(20)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.ShootInfo.PunchAngles` [L:49]
  - Attributes: `[FieldOffset(44)]`
- `bool Sharp.Shared.Types.ShootInfo.FirstShot` [L:52]
  - Attributes: `[FieldOffset(56)]`
- `float Sharp.Shared.Types.ShootInfo.AirInaccuracy` [L:67]
  - Attributes: `[FieldOffset(76)]`
- `float Sharp.Shared.Types.ShootInfo.AttackTickFraction` [L:31]
  - Attributes: `[FieldOffset(4)]`
- `float Sharp.Shared.Types.ShootInfo.AttackTime` [L:34]
  - Attributes: `[FieldOffset(8)]`
- `float Sharp.Shared.Types.ShootInfo.GroundInaccuracy` [L:64]
  - Attributes: `[FieldOffset(72)]`
- `float Sharp.Shared.Types.ShootInfo.Inaccuracy` [L:61]
  - Attributes: `[FieldOffset(68)]`
- `float Sharp.Shared.Types.ShootInfo.RecoilIndex` [L:70]
  - Attributes: `[FieldOffset(80)]`
- `float Sharp.Shared.Types.ShootInfo.RenderTickFraction` [L:40]
  - Attributes: `[FieldOffset(16)]`
- `int Sharp.Shared.Types.ShootInfo.AttackTickCount` [L:28]
  - Attributes: `[FieldOffset(0)]`
- `int Sharp.Shared.Types.ShootInfo.RenderTickCount` [L:37]
  - Attributes: `[FieldOffset(12)]`
- `int Sharp.Shared.Types.ShootInfo.ServerTick` [L:58]
  - Attributes: `[FieldOffset(64)]`
- `int Sharp.Shared.Types.ShootInfo.State` [L:55]
  - Attributes: `[FieldOffset(60)]`


### struct SoundEventGuid : System.ValueType

- FullName: `Sharp.Shared.Types.SoundEventGuid`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/SoundEventGuid.cs:25
- Generated: false
- Attributes: `[StructLayout(0, Size = 4)]`

Inheritance: object → System.ValueType → **SoundEventGuid**

#### Fields
- `readonly uint Sharp.Shared.Types.SoundEventGuid.Id` [L:33]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Types.SoundEventGuid.IsValid()` [L:38]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.SoundEventGuid.implicit operator Sharp.Shared.Types.SoundEventGuid(uint id)` [L:30]
  - Modifiers: public, static
- `static Sharp.Shared.Types.SoundEventGuid.implicit operator uint(Sharp.Shared.Types.SoundEventGuid guid)` [L:27]
  - Modifiers: public, static


### struct SoundOpEventGuid : System.ValueType

- FullName: `Sharp.Shared.Types.SoundOpEventGuid`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/SoundOpEventGuid.cs:25
- Generated: false
- Attributes: `[StructLayout(0, Size = 8)]`

Inheritance: object → System.ValueType → **SoundOpEventGuid**

#### Fields
- `readonly Sharp.Shared.Types.SoundEventGuid Sharp.Shared.Types.SoundOpEventGuid.Guid` [L:27]
  - Modifiers: public, readonly
- `readonly int Sharp.Shared.Types.SoundOpEventGuid.Hash` [L:28]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Types.SoundOpEventGuid.IsValid()` [L:55]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.SoundOpEventGuid.implicit operator Sharp.Shared.Types.SoundOpEventGuid(long value)` [L:36]
  - Modifiers: public, static
- `static Sharp.Shared.Types.SoundOpEventGuid.implicit operator long(Sharp.Shared.Types.SoundOpEventGuid value)` [L:47]
  - Modifiers: public, static


### record struct StringCommand : System.ValueType, System.IEquatable<Sharp.Shared.Types.StringCommand>

- FullName: `Sharp.Shared.Types.StringCommand`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/StringCommand.cs:30
- Generated: false

Inheritance: object → System.ValueType → **StringCommand**

#### Constructors
- `Sharp.Shared.Types.StringCommand.StringCommand(string command, bool chatTrigger, string? argumentString)` [L:39]

#### Properties
- `bool Sharp.Shared.Types.StringCommand.ChatTrigger` [L:33]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.StringCommand.ArgCount` [L:35]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.StringCommand.ArgString` [L:34]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.StringCommand.CommandName` [L:32]
  - Modifiers: public, readonly

#### Indexers
- `string Sharp.Shared.Types.StringCommand.this[int index]` [L:55]
  - Modifiers: public, readonly
  - Summary: Get command argument as string

#### Methods
- `T Sharp.Shared.Types.StringCommand.Get<T>(int index)` [L:81]
  - Modifiers: public, readonly
  - Summary: Get command argument converted to specified type
- `T Sharp.Shared.Types.StringCommand.GetEnum<T>(int index) where T : System.Enum` [L:197]
  - Modifiers: public, readonly
  - Summary: Get command argument and parse as enum value
- `T? Sharp.Shared.Types.StringCommand.TryGet<T>(int index)` [L:142]
  - Modifiers: public, readonly
  - Summary: Try to get command argument converted to specified type, returns null if conversion fails
- `string Sharp.Shared.Types.StringCommand.GetArg(int index)` [L:62]
  - Modifiers: public, readonly
  - Summary: Get command argument as string
- `string Sharp.Shared.Types.StringCommand.GetCommandString()` [L:48]
  - Modifiers: public, readonly


### struct StringTableUserData : System.ValueType

- FullName: `Sharp.Shared.Types.StringTableUserData`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/StringTableUserData.cs:25
- Generated: false
- Attributes: `[StructLayout(2)]`

Inheritance: object → System.ValueType → **StringTableUserData**

#### Fields
- `byte* Sharp.Shared.Types.StringTableUserData.Data` [L:28]
  - Attributes: `[FieldOffset(0)]`
- `int Sharp.Shared.Types.StringTableUserData.Size` [L:31]
  - Attributes: `[FieldOffset(8)]`


### struct SubTickAttack : System.ValueType

- FullName: `Sharp.Shared.Types.SubTickAttack`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/MoveData.cs:107
- Generated: false
- Attributes: `[StructLayout(2, Size = 24, Pack = 8)]`

Inheritance: object → System.ValueType → **SubTickAttack**

#### Fields
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.SubTickAttack.Button` [L:113]
  - Attributes: `[FieldOffset(8)]`
- `bool Sharp.Shared.Types.SubTickAttack.Pressed` [L:116]
  - Attributes: `[FieldOffset(16)]`
- `float Sharp.Shared.Types.SubTickAttack.When` [L:110]
  - Attributes: `[FieldOffset(0)]`


### struct SubTickMove : System.ValueType

- FullName: `Sharp.Shared.Types.SubTickMove`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/MoveData.cs:120
- Generated: false
- Attributes: `[StructLayout(2, Size = 32, Pack = 8)]`

Inheritance: object → System.ValueType → **SubTickMove**

#### Fields
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.SubTickMove.Button` [L:126]
  - Attributes: `[FieldOffset(8)]`
- `bool Sharp.Shared.Types.SubTickMove.Pressed` [L:129]
  - Attributes: `[FieldOffset(16)]`
- `float Sharp.Shared.Types.SubTickMove.AnalogForwardDelta` [L:132]
  - Attributes: `[FieldOffset(16)]`
- `float Sharp.Shared.Types.SubTickMove.AnalogLeftDelta` [L:135]
  - Attributes: `[FieldOffset(20)]`
- `float Sharp.Shared.Types.SubTickMove.AnalogPitchDelta` [L:138]
  - Attributes: `[FieldOffset(24)]`
- `float Sharp.Shared.Types.SubTickMove.AnalogYawDelta` [L:141]
  - Attributes: `[FieldOffset(28)]`
- `float Sharp.Shared.Types.SubTickMove.When` [L:123]
  - Attributes: `[FieldOffset(0)]`

#### Properties
- `bool Sharp.Shared.Types.SubTickMove.IsAnalogInput` [L:143]
  - Modifiers: public, readonly

#### Methods
- `override string Sharp.Shared.Types.SubTickMove.ToString()` [L:145]
  - Modifiers: public, override


### struct TakeDamageInfo : System.ValueType

- FullName: `Sharp.Shared.Types.TakeDamageInfo`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/TakeDamageInfo.cs:27
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 288)]`

Inheritance: object → System.ValueType → **TakeDamageInfo**

#### Constructors
- `Sharp.Shared.Types.TakeDamageInfo.TakeDamageInfo()` [L:141]
- `Sharp.Shared.Types.TakeDamageInfo.TakeDamageInfo(Sharp.Shared.GameEntities.IPlayerPawn killer)` [L:156]

#### Fields
- `Sharp.Shared.Enums.DamageFlagBits Sharp.Shared.Types.TakeDamageInfo.DamageType` [L:60]
  - Attributes: `[FieldOffset(76)]`
- `Sharp.Shared.Enums.HitGroupType Sharp.Shared.Types.TakeDamageInfo.HitGroupId` [L:87]
  - Attributes: `[FieldOffset(120)]`
- `Sharp.Shared.Enums.TakeDamageFlags Sharp.Shared.Types.TakeDamageInfo.TakeDamageFlags` [L:84]
  - Attributes: `[FieldOffset(112)]`
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.Types.TakeDamageInfo.Ability` [L:51]
  - Attributes: `[FieldOffset(64)]`
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.Types.TakeDamageInfo.Attacker` [L:48]
  - Attributes: `[FieldOffset(60)]`
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.Types.TakeDamageInfo.Inflictor` [L:45]
  - Attributes: `[FieldOffset(56)]`
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IPlayerPawn> Sharp.Shared.Types.TakeDamageInfo.AttackerPawnHandle` [L:116]
  - Attributes: `[FieldOffset(236)]`
- `Sharp.Shared.Types.ShootInfo Sharp.Shared.Types.TakeDamageInfo.ShootInfo` [L:99]
  - Attributes: `[FieldOffset(136)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TakeDamageInfo.DamageDirection` [L:42]
  - Attributes: `[FieldOffset(44)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TakeDamageInfo.DamageForce` [L:33]
  - Attributes: `[FieldOffset(8)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TakeDamageInfo.DamagePosition` [L:36]
  - Attributes: `[FieldOffset(20)]`
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TakeDamageInfo.ReportedPosition` [L:39]
  - Attributes: `[FieldOffset(32)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.InTakeDamageFlow` [L:133]
  - Attributes: `[FieldOffset(272)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.IsPawn` [L:110]
  - Attributes: `[FieldOffset(233)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.IsWorld` [L:113]
  - Attributes: `[FieldOffset(234)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.NeedInit` [L:107]
  - Attributes: `[FieldOffset(232)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.ShouldBleed` [L:72]
  - Attributes: `[FieldOffset(100)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.ShouldSpark` [L:75]
  - Attributes: `[FieldOffset(101)]`
- `bool Sharp.Shared.Types.TakeDamageInfo.StoppedBullet` [L:96]
  - Attributes: `[FieldOffset(132)]`
- `byte Sharp.Shared.Types.TakeDamageInfo.AmmoType` [L:66]
  - Attributes: `[FieldOffset(84)]`
- `float Sharp.Shared.Types.TakeDamageInfo.Damage` [L:54]
  - Attributes: `[FieldOffset(68)]`
- `float Sharp.Shared.Types.TakeDamageInfo.FriendlyFireDamageReductionRatio` [L:93]
  - Attributes: `[FieldOffset(128)]`
- `float Sharp.Shared.Types.TakeDamageInfo.OriginalDamage` [L:69]
  - Attributes: `[FieldOffset(96)]`
- `float Sharp.Shared.Types.TakeDamageInfo.TotalledDamage` [L:57]
  - Attributes: `[FieldOffset(72)]`
- `int Sharp.Shared.Types.TakeDamageInfo.AttackerPlayerSlot` [L:122]
  - Attributes: `[FieldOffset(240)]`
  - Summary: Attacker PlayerSlot
- `int Sharp.Shared.Types.TakeDamageInfo.DamageCustom` [L:63]
  - Attributes: `[FieldOffset(80)]`
- `int Sharp.Shared.Types.TakeDamageInfo.NumObjectsPenetrated` [L:90]
  - Attributes: `[FieldOffset(124)]`
- `int Sharp.Shared.Types.TakeDamageInfo.Team` [L:128]
  - Attributes: `[FieldOffset(248)]`
- `int Sharp.Shared.Types.TakeDamageInfo.TeamChecked` [L:125]
  - Attributes: `[FieldOffset(244)]`
- `int Sharp.Shared.Types.TakeDamageInfo.UnknownFinal` [L:136]
  - Attributes: `[FieldOffset(284)]`
- `void* Sharp.Shared.Types.TakeDamageInfo.ScriptInstance` [L:102]
  - Attributes: `[FieldOffset(224)]`
- `void* Sharp.Shared.Types.TakeDamageInfo.pVTable` [L:30]
  - Attributes: `[FieldOffset(0)]`

#### Properties
- `readonly Sharp.Shared.Types.GameTrace* Sharp.Shared.Types.TakeDamageInfo.Trace` [L:81]
  - Modifiers: public, readonly

#### Methods
- `Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.AddDamageFlags(Sharp.Shared.Enums.TakeDamageFlags flags)` [L:217]
- `Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.AddDamageType(Sharp.Shared.Enums.DamageFlagBits bits)` [L:210]
- `Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.SetDamage(float damage)` [L:224]
- `Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.SetInitDamage(float damage)` [L:231]
- `static Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.CreateCustom(Sharp.Shared.GameEntities.IPlayerPawn killer, Sharp.Shared.GameEntities.IBaseEntity weapon, Sharp.Shared.Enums.DamageFlagBits damageType)` [L:204]
  - Modifiers: public, static
- `static Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.CreateFromBullet(Sharp.Shared.GameEntities.IPlayerPawn killer, Sharp.Shared.GameEntities.IBaseWeapon weapon, bool headShot)` [L:189]
  - Modifiers: public, static
- `static Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.CreateFromFire(Sharp.Shared.GameEntities.IBaseEntity inflictor, Sharp.Shared.GameEntities.IPlayerPawn killer)` [L:174]
  - Modifiers: public, static
- `static Sharp.Shared.Types.TakeDamageInfo Sharp.Shared.Types.TakeDamageInfo.CreateFromSlash(Sharp.Shared.GameEntities.IPlayerPawn killer, Sharp.Shared.GameEntities.IBaseEntity weapon)` [L:183]
  - Modifiers: public, static


### struct TakeDamageResult : System.ValueType

- FullName: `Sharp.Shared.Types.TakeDamageResult`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/TakeDamageResult.cs:27
- Generated: false
- Attributes: `[StructLayout(2, Size = 80)]`

Inheritance: object → System.ValueType → **TakeDamageResult**

#### Fields
- `Sharp.Shared.Types.TakeDamageInfo* Sharp.Shared.Types.TakeDamageResult.OriginatingInfo` [L:30]
  - Attributes: `[FieldOffset(0)]`
- `bool Sharp.Shared.Types.TakeDamageResult.SuppressFlinch` [L:65]
  - Attributes: `[FieldOffset(65)]`
- `bool Sharp.Shared.Types.TakeDamageResult.WasDamageSuppressed` [L:62]
  - Attributes: `[FieldOffset(64)]`
- `float Sharp.Shared.Types.TakeDamageResult.DamageDealt` [L:41]
  - Attributes: `[FieldOffset(32)]`
- `float Sharp.Shared.Types.TakeDamageResult.NewDamageAccumulatorValue` [L:56]
  - Attributes: `[FieldOffset(52)]`
- `float Sharp.Shared.Types.TakeDamageResult.PreModifiedDamage` [L:44]
  - Attributes: `[FieldOffset(36)]`
- `float Sharp.Shared.Types.TakeDamageResult.TotalledDamageDealt` [L:50]
  - Attributes: `[FieldOffset(44)]`
- `float Sharp.Shared.Types.TakeDamageResult.TotalledPreModifiedDamage` [L:53]
  - Attributes: `[FieldOffset(48)]`
- `int Sharp.Shared.Types.TakeDamageResult.HealthBefore` [L:38]
  - Attributes: `[FieldOffset(28)]`
- `int Sharp.Shared.Types.TakeDamageResult.HealthLost` [L:35]
  - Attributes: `[FieldOffset(24)]`
- `int Sharp.Shared.Types.TakeDamageResult.TotalledHealthLost` [L:47]
  - Attributes: `[FieldOffset(40)]`
- `ulong Sharp.Shared.Types.TakeDamageResult.DamageFlags` [L:59]
  - Attributes: `[FieldOffset(56)]`

#### Obsolete Members
- `float Sharp.Shared.Types.TakeDamageResult.m_flTotalledPreModifiedDamage` [L:71] — Use TotalledPreModifiedDamage instead


### record struct TeamRewardInfo : System.ValueType, System.IEquatable<Sharp.Shared.Types.TeamRewardInfo>

- FullName: `Sharp.Shared.Types.TeamRewardInfo`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/TeamRewardInfo.cs:26
- Generated: false
- Attributes: `[StructLayout(2, Pack = 4, Size = 8)]`

Inheritance: object → System.ValueType → **TeamRewardInfo**

#### Fields
- `readonly Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.Types.TeamRewardInfo.Team` [L:29]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Enums.TeamRewardType Sharp.Shared.Types.TeamRewardInfo.Type` [L:32]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(4)]`


### struct TraceResult : System.ValueType

- FullName: `Sharp.Shared.Types.TraceResult`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/TraceResult.cs:27
- Generated: false

Inheritance: object → System.ValueType → **TraceResult**

#### Constructors
- `Sharp.Shared.Types.TraceResult.TraceResult(Sharp.Shared.GameEntities.IBaseEntity? entity, float fraction, Sharp.Shared.Enums.TraceRayType rayType, bool startInSolid, int triangle, Sharp.Shared.Types.Vector startPosition, Sharp.Shared.Types.Vector endPosition, Sharp.Shared.Types.Vector planeNormal, Sharp.Shared.Types.PhysicsSurfaceProperties* surface, Sharp.Shared.Types.HitBoxData* hitBox, void* physicsBody, void* physicsShape, Sharp.Shared.Types.Vector hitPoint, float hitOffset, uint contents, short hitBoxBoneIndex)` [L:46]

#### Properties
- `Sharp.Shared.Enums.HitGroupType Sharp.Shared.Types.TraceResult.HitGroup` [L:91]
  - Modifiers: public, readonly
  - Summary: The HitGroup of the entity (e.g., Head, Chest).
- `Sharp.Shared.Enums.TraceRayType Sharp.Shared.Types.TraceResult.RayType` [L:31]
  - Modifiers: public, readonly
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.Types.TraceResult.HitEntity` [L:29]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.HitBoxData* Sharp.Shared.Types.TraceResult.HitBoxData` [L:38]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.PhysicsSurfaceProperties* Sharp.Shared.Types.TraceResult.SurfaceProp` [L:37]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResult.EndPosition` [L:35]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResult.HitPoint` [L:41]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResult.PlaneNormal` [L:36]
  - Modifiers: public, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResult.StartPosition` [L:34]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Types.TraceResult.StartInSolid` [L:32]
  - Modifiers: public, readonly
- `float Sharp.Shared.Types.TraceResult.Fraction` [L:30]
  - Modifiers: public, readonly
- `float Sharp.Shared.Types.TraceResult.HitOffset` [L:42]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.TraceResult.HitBoxId` [L:97]
  - Modifiers: public, readonly
  - Summary: The HitBox ID of the entity.
- `int Sharp.Shared.Types.TraceResult.Triangle` [L:33]
  - Modifiers: public, readonly
- `short Sharp.Shared.Types.TraceResult.HitBoxBoneIndex` [L:44]
  - Modifiers: public, readonly
- `string Sharp.Shared.Types.TraceResult.HitBoxName` [L:103]
  - Modifiers: public, readonly
  - Summary: The HitBox name of the entity.
- `string Sharp.Shared.Types.TraceResult.SurfaceName` [L:108]
  - Modifiers: public, readonly
  - Summary: The name of the surface material.
- `uint Sharp.Shared.Types.TraceResult.Contents` [L:43]
  - Modifiers: public, readonly
- `void* Sharp.Shared.Types.TraceResult.PhysicsBody` [L:39]
  - Modifiers: public, readonly
- `void* Sharp.Shared.Types.TraceResult.PhysicsShape` [L:40]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Types.TraceResult.DidHit()` [L:84]
  - Modifiers: public, readonly
  - Summary: Did the trace hit anything


### struct TraceResultStruct : System.ValueType

- FullName: `Sharp.Shared.Types.TraceResultStruct`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/TraceResult.cs:112
- Generated: false
- Attributes: `[StructLayout(2, Size = 112)]`

Inheritance: object → System.ValueType → **TraceResultStruct**

#### Fields
- `readonly Sharp.Shared.Enums.TraceRayType Sharp.Shared.Types.TraceResultStruct.RayType` [L:121]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(12)]`
- `readonly Sharp.Shared.Types.HitBoxData* Sharp.Shared.Types.TraceResultStruct.HitBoxData` [L:142]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(64)]`
- `readonly Sharp.Shared.Types.PhysicsSurfaceProperties* Sharp.Shared.Types.TraceResultStruct.SurfaceProp` [L:139]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(56)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResultStruct.EndPosition` [L:133]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(32)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResultStruct.HitPoint` [L:151]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(88)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResultStruct.PlaneNormal` [L:136]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(44)]`
- `readonly Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceResultStruct.StartPosition` [L:130]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(20)]`
- `readonly bool Sharp.Shared.Types.TraceResultStruct.StartInSolid` [L:124]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(13)]`
- `readonly float Sharp.Shared.Types.TraceResultStruct.Fraction` [L:118]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(8)]`
- `readonly float Sharp.Shared.Types.TraceResultStruct.HitOffset` [L:154]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(100)]`
- `readonly int Sharp.Shared.Types.TraceResultStruct.Triangle` [L:127]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(16)]`
- `readonly nint Sharp.Shared.Types.TraceResultStruct.HitEntity` [L:115]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly short Sharp.Shared.Types.TraceResultStruct.HitGroupHitBoxBoneIndex` [L:160]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(108)]`
- `readonly uint Sharp.Shared.Types.TraceResultStruct.Contents` [L:157]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(104)]`
- `readonly void* Sharp.Shared.Types.TraceResultStruct.PhysicsBody` [L:145]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(72)]`
- `readonly void* Sharp.Shared.Types.TraceResultStruct.PhysicsShape` [L:148]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(80)]`


### struct TraceShapeCapsule : System.ValueType

- FullName: `Sharp.Shared.Types.TraceShapeCapsule`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/GameTrace.cs:211
- Generated: false
- Attributes: `[StructLayout(0, Size = 28)]`

Inheritance: object → System.ValueType → **TraceShapeCapsule**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeCapsule.m_vCenter1` [L:213]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeCapsule.m_vCenter2` [L:214]
- `float Sharp.Shared.Types.TraceShapeCapsule.Radius` [L:215]


### struct TraceShapeHull : System.ValueType

- FullName: `Sharp.Shared.Types.TraceShapeHull`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/GameTrace.cs:204
- Generated: false
- Attributes: `[StructLayout(0, Size = 24)]`

Inheritance: object → System.ValueType → **TraceShapeHull**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeHull.Maxs` [L:207]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeHull.Mins` [L:206]


### struct TraceShapeLine : System.ValueType

- FullName: `Sharp.Shared.Types.TraceShapeLine`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/GameTrace.cs:190
- Generated: false
- Attributes: `[StructLayout(0, Size = 16)]`

Inheritance: object → System.ValueType → **TraceShapeLine**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeLine.Start` [L:192]
- `float Sharp.Shared.Types.TraceShapeLine.Radius` [L:193]


### struct TraceShapeRay : System.ValueType

- FullName: `Sharp.Shared.Types.TraceShapeRay`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/GameTrace.cs:147
- Generated: false
- Attributes: `[StructLayout(2, Size = 48)]`

Inheritance: object → System.ValueType → **TraceShapeRay**

#### Constructors
- `Sharp.Shared.Types.TraceShapeRay.TraceShapeRay(Sharp.Shared.Types.TraceShapeCapsule capsule)` [L:182]
- `Sharp.Shared.Types.TraceShapeRay.TraceShapeRay(Sharp.Shared.Types.TraceShapeHull hull)` [L:176]
- `Sharp.Shared.Types.TraceShapeRay.TraceShapeRay(Sharp.Shared.Types.TraceShapeLine line)` [L:164]
- `Sharp.Shared.Types.TraceShapeRay.TraceShapeRay(Sharp.Shared.Types.TraceShapeSphere sphere)` [L:170]

#### Fields
- `readonly Sharp.Shared.Enums.TraceRayType Sharp.Shared.Types.TraceShapeRay.Type` [L:162]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(40)]`
- `readonly Sharp.Shared.Types.TraceShapeCapsule Sharp.Shared.Types.TraceShapeRay.Capsule` [L:159]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Types.TraceShapeHull Sharp.Shared.Types.TraceShapeRay.Hull` [L:156]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Types.TraceShapeLine Sharp.Shared.Types.TraceShapeRay.Line` [L:150]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`
- `readonly Sharp.Shared.Types.TraceShapeSphere Sharp.Shared.Types.TraceShapeRay.Sphere` [L:153]
  - Modifiers: public, readonly
  - Attributes: `[FieldOffset(0)]`


### struct TraceShapeSphere : System.ValueType

- FullName: `Sharp.Shared.Types.TraceShapeSphere`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/GameTrace.cs:197
- Generated: false
- Attributes: `[StructLayout(0, Size = 16)]`

Inheritance: object → System.ValueType → **TraceShapeSphere**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.TraceShapeSphere.Center` [L:199]
- `float Sharp.Shared.Types.TraceShapeSphere.Radius` [L:200]


### struct Vector : System.ValueType, System.IComparable, System.IComparable<Sharp.Shared.Types.Vector>, System.IEquatable<Sharp.Shared.Types.Vector>

- FullName: `Sharp.Shared.Types.Vector`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Vector.cs:28
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **Vector**

#### Constructors
- `Sharp.Shared.Types.Vector.Vector()` [L:78]
- `Sharp.Shared.Types.Vector.Vector(Sharp.Shared.Types.Vector other)` [L:52]
- `Sharp.Shared.Types.Vector.Vector(float x, float y, float z)` [L:45]

#### Properties
- `float Sharp.Shared.Types.Vector.X` [L:33]
  - Summary: X or PITCH (Up / Down)
- `float Sharp.Shared.Types.Vector.Y` [L:38]
  - Summary: Y or YAW (Left / Right)
- `float Sharp.Shared.Types.Vector.Z` [L:43]
  - Summary: Z or ROLL (Fall over)

#### Indexers
- `float Sharp.Shared.Types.Vector.this[int key]` [L:85]

#### Methods
- `CMsgQAngle Sharp.Shared.Types.Vector.ToMsgQAngle()` [L:367]
- `CMsgVector Sharp.Shared.Types.Vector.ToMsgVector()` [L:355]
- `CMsgVector2D Sharp.Shared.Types.Vector.ToMsgVector2D()` [L:364]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.AnglesTo(Sharp.Shared.Types.Vector position)` [L:311]
  - Summary: Calculates the Euler angles required to look at a specific position.
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.AnglesToVectorForward()` [L:150]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.Cross(Sharp.Shared.Types.Vector rhs)` [L:248]
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.DirectionToAngles()` [L:299]
  - Summary: Converts a direction vector into Euler angles.
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.VectorToAngles()` [L:318]
- `Sharp.Shared.Types.Vector2D Sharp.Shared.Types.Vector.AsVector2D()` [L:251]
- `bool Sharp.Shared.Types.Vector.Equals(Sharp.Shared.Types.Vector other)` [L:350]
- `bool Sharp.Shared.Types.Vector.IsValid()` [L:180]
- `bool Sharp.Shared.Types.Vector.IsZero([float tolerance = 0.01])` [L:183]
- `float Sharp.Shared.Types.Vector.DistTo(Sharp.Shared.Types.Vector other)` [L:213]
- `float Sharp.Shared.Types.Vector.DistToSqr(Sharp.Shared.Types.Vector other)` [L:204]
  - Summary: Calculates the squared distance to another vector.
- `float Sharp.Shared.Types.Vector.Dot(Sharp.Shared.Types.Vector other)` [L:186]
- `float Sharp.Shared.Types.Vector.Length()` [L:189]
- `float Sharp.Shared.Types.Vector.Length2D()` [L:195]
- `float Sharp.Shared.Types.Vector.Length2DSqr()` [L:198]
- `float Sharp.Shared.Types.Vector.LengthSqr()` [L:192]
- `int Sharp.Shared.Types.Vector.CompareTo(Sharp.Shared.Types.Vector rhs)` [L:281]
- `int Sharp.Shared.Types.Vector.CompareTo(object? obj)` [L:268]
- `override bool Sharp.Shared.Types.Vector.Equals(object? obj)` [L:59]
  - Modifiers: public, override
- `override int Sharp.Shared.Types.Vector.GetHashCode()` [L:69]
  - Modifiers: public, override
- `override string Sharp.Shared.Types.Vector.ToString()` [L:262]
  - Modifiers: public, override
- `static float Sharp.Shared.Types.Vector.DotProduct(in Sharp.Shared.Types.Vector a, in Sharp.Shared.Types.Vector b)` [L:287]
  - Modifiers: public, static
  - Summary: Calculates the Dot Product.
- `static float Sharp.Shared.Types.Vector.Magnitude(in Sharp.Shared.Types.Vector v)` [L:293]
  - Modifiers: public, static
  - Summary: Calculates the Magnitude (Length).
- `void Sharp.Shared.Types.Vector.AnglesToVector(out Sharp.Shared.Types.Vector forward, out Sharp.Shared.Types.Vector right, out Sharp.Shared.Types.Vector up)` [L:158]
- `void Sharp.Shared.Types.Vector.AnglesToVectorSource2(out Sharp.Shared.Types.Vector forward, out Sharp.Shared.Types.Vector right, out Sharp.Shared.Types.Vector up)` [L:169]
- `void Sharp.Shared.Types.Vector.Negate()` [L:241]
  - Summary: Negates the vector (inverts its direction).
- `void Sharp.Shared.Types.Vector.Normalize()` [L:219]
  - Summary: Normalizes the vector (makes it a unit vector with length 1).

#### Operators
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator *(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:126]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator *(Sharp.Shared.Types.Vector vec, float fl)` [L:123]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator +(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:117]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator +(Sharp.Shared.Types.Vector vec, float fl)` [L:129]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator -(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:120]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator -(Sharp.Shared.Types.Vector vec, float fl)` [L:132]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator /(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:143]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Shared.Types.Vector.operator /(Sharp.Shared.Types.Vector vec, float fl)` [L:135]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Vector.operator !=(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:75]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Vector.operator ==(Sharp.Shared.Types.Vector a, Sharp.Shared.Types.Vector b)` [L:72]
  - Modifiers: public, static


### struct Vector2D : System.ValueType, System.IComparable, System.IComparable<Sharp.Shared.Types.Vector2D>, System.IEquatable<Sharp.Shared.Types.Vector2D>

- FullName: `Sharp.Shared.Types.Vector2D`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Vector.cs:375
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **Vector2D**

#### Constructors
- `Sharp.Shared.Types.Vector2D.Vector2D(Sharp.Shared.Types.Vector other)` [L:386]
- `Sharp.Shared.Types.Vector2D.Vector2D(float x, float y)` [L:380]

#### Properties
- `float Sharp.Shared.Types.Vector2D.X` [L:377]
- `float Sharp.Shared.Types.Vector2D.Y` [L:378]

#### Methods
- `CMsgVector2D Sharp.Shared.Types.Vector2D.ToMsgVector2D()` [L:446]
- `bool Sharp.Shared.Types.Vector2D.Equals(Sharp.Shared.Types.Vector2D other)` [L:442]
- `bool Sharp.Shared.Types.Vector2D.IsValid()` [L:392]
- `float Sharp.Shared.Types.Vector2D.Dot(Sharp.Shared.Types.Vector2D other)` [L:401]
- `float Sharp.Shared.Types.Vector2D.Length()` [L:398]
- `float Sharp.Shared.Types.Vector2D.LengthSqr()` [L:395]
- `int Sharp.Shared.Types.Vector2D.CompareTo(Sharp.Shared.Types.Vector2D rhs)` [L:420]
- `int Sharp.Shared.Types.Vector2D.CompareTo(object? obj)` [L:407]
- `override bool Sharp.Shared.Types.Vector2D.Equals(object? obj)` [L:432]
  - Modifiers: public, override
- `override int Sharp.Shared.Types.Vector2D.GetHashCode()` [L:429]
  - Modifiers: public, override

#### Operators
- `static bool Sharp.Shared.Types.Vector2D.operator !=(Sharp.Shared.Types.Vector2D a, Sharp.Shared.Types.Vector2D b)` [L:426]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Vector2D.operator ==(Sharp.Shared.Types.Vector2D a, Sharp.Shared.Types.Vector2D b)` [L:423]
  - Modifiers: public, static


### struct Vector4D : System.ValueType, System.IEquatable<Sharp.Shared.Types.Vector4D>

- FullName: `Sharp.Shared.Types.Vector4D`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Vector.cs:451
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **Vector4D**

#### Constructors
- `Sharp.Shared.Types.Vector4D.Vector4D(Sharp.Shared.Types.Vector4D other)` [L:466]
- `Sharp.Shared.Types.Vector4D.Vector4D(float x, float y, float z, float w)` [L:458]

#### Properties
- `float Sharp.Shared.Types.Vector4D.W` [L:456]
- `float Sharp.Shared.Types.Vector4D.X` [L:453]
- `float Sharp.Shared.Types.Vector4D.Y` [L:454]
- `float Sharp.Shared.Types.Vector4D.Z` [L:455]

#### Methods
- `CMsgVector Sharp.Shared.Types.Vector4D.ToMsgVector()` [L:514]
- `CMsgVector2D Sharp.Shared.Types.Vector4D.ToMsgVector2D()` [L:523]
- `bool Sharp.Shared.Types.Vector4D.Equals(Sharp.Shared.Types.Vector4D other)` [L:508]
- `bool Sharp.Shared.Types.Vector4D.IsValid()` [L:474]
- `float Sharp.Shared.Types.Vector4D.Dot(Sharp.Shared.Types.Vector4D other)` [L:483]
- `float Sharp.Shared.Types.Vector4D.Length()` [L:480]
- `float Sharp.Shared.Types.Vector4D.LengthSqr()` [L:477]
- `override bool Sharp.Shared.Types.Vector4D.Equals(object? obj)` [L:498]
  - Modifiers: public, override
- `override int Sharp.Shared.Types.Vector4D.GetHashCode()` [L:495]
  - Modifiers: public, override

#### Operators
- `static bool Sharp.Shared.Types.Vector4D.operator !=(Sharp.Shared.Types.Vector4D a, Sharp.Shared.Types.Vector4D b)` [L:492]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Vector4D.operator ==(Sharp.Shared.Types.Vector4D a, Sharp.Shared.Types.Vector4D b)` [L:486]
  - Modifiers: public, static


### record struct VirtualTableInfo : System.ValueType, System.IEquatable<Sharp.Shared.Types.VirtualTableInfo>

- FullName: `Sharp.Shared.Types.VirtualTableInfo`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/VirtualTableInfo.cs:22
- Generated: false

Inheritance: object → System.ValueType → **VirtualTableInfo**

#### Properties
- `nint Sharp.Shared.Types.VirtualTableInfo.Address` [L:39]
  - Summary: Vtable address
- `required string Sharp.Shared.Types.VirtualTableInfo.DemangledName` [L:34]
  - Summary: Demangled vtable name
- `ulong Sharp.Shared.Types.VirtualTableInfo.Offset` [L:50]
  - Summary: Offset to Primary vtable address


