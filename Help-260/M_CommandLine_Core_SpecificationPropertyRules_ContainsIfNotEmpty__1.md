# SpecificationPropertyRules.ContainsIfNotEmpty(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static bool ContainsIfNotEmpty<T>(
	this IEnumerable<T> sequence,
	T value
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function ContainsIfNotEmpty(Of T) ( 
	sequence As IEnumerable(Of T),
	value As T
) As Boolean
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
generic<typename T>
static bool ContainsIfNotEmpty(
	IEnumerable<T>^ sequence, 
	T value
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member ContainsIfNotEmpty : 
        sequence : IEnumerable<'T> * 
        value : 'T -> bool 

```


#### Parameters
&nbsp;<dl><dt>sequence</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>value</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationPropertyRules">SpecificationPropertyRules Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />