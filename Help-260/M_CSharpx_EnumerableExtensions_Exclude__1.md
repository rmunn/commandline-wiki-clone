# EnumerableExtensions.Exclude(*T*) Method 
 

Excludes *count* elements from a sequence starting at a given index

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T> Exclude<T>(
	this IEnumerable<T> sequence,
	int startIndex,
	int count
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Exclude(Of T) ( 
	sequence As IEnumerable(Of T),
	startIndex As Integer,
	count As Integer
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<T>^ Exclude(
	IEnumerable<T>^ sequence, 
	int startIndex, 
	int count
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Exclude : 
        sequence : IEnumerable<'T> * 
        startIndex : int * 
        count : int -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>sequence</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>startIndex</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>count</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>The type of the elements of the sequence</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />