# ReflectionExtensions.GetSpecifications(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T> GetSpecifications<T>(
	this Type type,
	Func<PropertyInfo, T> selector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function GetSpecifications(Of T) ( 
	type As Type,
	selector As Func(Of PropertyInfo, T)
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<T>^ GetSpecifications(
	Type^ type, 
	Func<PropertyInfo^, T>^ selector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member GetSpecifications : 
        type : Type * 
        selector : Func<PropertyInfo, 'T> -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>selector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.reflection.propertyinfo" target="_blank">PropertyInfo</a>, *T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />