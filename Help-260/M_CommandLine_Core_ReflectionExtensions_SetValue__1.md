# ReflectionExtensions.SetValue(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<Error> SetValue<T>(
	this SpecificationProperty specProp,
	T instance,
	Object value
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function SetValue(Of T) ( 
	specProp As SpecificationProperty,
	instance As T,
	value As Object
) As IEnumerable(Of Error)
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<Error^>^ SetValue(
	SpecificationProperty^ specProp, 
	T instance, 
	Object^ value
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member SetValue : 
        specProp : SpecificationProperty * 
        instance : 'T * 
        value : Object -> IEnumerable<Error> 

```


#### Parameters
&nbsp;<dl><dt>specProp</dt><dd>Type: <a href="T_CommandLine_Core_SpecificationProperty">CommandLine.Core.SpecificationProperty</a><br /></dd><dt>instance</dt><dd>Type: *T*<br /></dd><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />