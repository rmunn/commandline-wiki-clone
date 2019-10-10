# EnumerableExtensions.Cartesian(*TFirst*, *TSecond*, *TResult*) Method 
 

Returns the Cartesian product of two sequences by combining each element of the first set with each in the second and applying the user=define projection to the pair.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<TResult> Cartesian<TFirst, TSecond, TResult>(
	this IEnumerable<TFirst> first,
	IEnumerable<TSecond> second,
	Func<TFirst, TSecond, TResult> resultSelector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Cartesian(Of TFirst, TSecond, TResult) ( 
	first As IEnumerable(Of TFirst),
	second As IEnumerable(Of TSecond),
	resultSelector As Func(Of TFirst, TSecond, TResult)
) As IEnumerable(Of TResult)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TFirst, typename TSecond, typename TResult>
static IEnumerable<TResult>^ Cartesian(
	IEnumerable<TFirst>^ first, 
	IEnumerable<TSecond>^ second, 
	Func<TFirst, TSecond, TResult>^ resultSelector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Cartesian : 
        first : IEnumerable<'TFirst> * 
        second : IEnumerable<'TSecond> * 
        resultSelector : Func<'TFirst, 'TSecond, 'TResult> -> IEnumerable<'TResult> 

```


#### Parameters
&nbsp;<dl><dt>first</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TFirst*)<br /></dd><dt>second</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TSecond*)<br /></dd><dt>resultSelector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TFirst*, *TSecond*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TFirst</dt><dd /><dt>TSecond</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TResult*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TFirst*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />