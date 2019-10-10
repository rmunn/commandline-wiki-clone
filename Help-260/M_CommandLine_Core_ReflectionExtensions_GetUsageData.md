# ReflectionExtensions.GetUsageData Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<Tuple<PropertyInfo, UsageAttribute>> GetUsageData(
	this Type type
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function GetUsageData ( 
	type As Type
) As Maybe(Of Tuple(Of PropertyInfo, UsageAttribute))
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static Maybe<Tuple<PropertyInfo^, UsageAttribute^>^>^ GetUsageData(
	Type^ type
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member GetUsageData : 
        type : Type -> Maybe<Tuple<PropertyInfo, UsageAttribute>> 

```


#### Parameters
&nbsp;<dl><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="https://docs.microsoft.com/dotnet/api/system.reflection.propertyinfo" target="_blank">PropertyInfo</a>, <a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a>))

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />