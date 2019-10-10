# ReflectionExtensions.SetProperties(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Error> SetProperties<T>(
	this T instance,
	IEnumerable<SpecificationProperty> specProps,
	Func<SpecificationProperty, bool> predicate,
	Func<SpecificationProperty, Object> selector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function SetProperties(Of T) ( 
	instance As T,
	specProps As IEnumerable(Of SpecificationProperty),
	predicate As Func(Of SpecificationProperty, Boolean),
	selector As Func(Of SpecificationProperty, Object)
) As IEnumerable(Of Error)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<Error^>^ SetProperties(
	T instance, 
	IEnumerable<SpecificationProperty^>^ specProps, 
	Func<SpecificationProperty^, bool>^ predicate, 
	Func<SpecificationProperty^, Object^>^ selector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member SetProperties : 
        instance : 'T * 
        specProps : IEnumerable<SpecificationProperty> * 
        predicate : Func<SpecificationProperty, bool> * 
        selector : Func<SpecificationProperty, Object> -> IEnumerable<Error> 

```


#### Parameters
&nbsp;<dl><dt>instance</dt><dd>Type: *T*<br /></dd><dt>specProps</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>predicate</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>)<br /></dd><dt>selector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>, <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type . When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />