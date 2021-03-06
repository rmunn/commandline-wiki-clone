# MaybeExtensions.SelectMany(*TSource*, *TValue*, *TResult*) Method 
 

Bind operation compatible with Linq.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<TResult> SelectMany<TSource, TValue, TResult>(
	this Maybe<TSource> maybe,
	Func<TSource, Maybe<TValue>> valueSelector,
	Func<TSource, TValue, TResult> resultSelector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function SelectMany(Of TSource, TValue, TResult) ( 
	maybe As Maybe(Of TSource),
	valueSelector As Func(Of TSource, Maybe(Of TValue)),
	resultSelector As Func(Of TSource, TValue, TResult)
) As Maybe(Of TResult)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSource, typename TValue, typename TResult>
static Maybe<TResult>^ SelectMany(
	Maybe<TSource>^ maybe, 
	Func<TSource, Maybe<TValue>^>^ valueSelector, 
	Func<TSource, TValue, TResult>^ resultSelector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member SelectMany : 
        maybe : Maybe<'TSource> * 
        valueSelector : Func<'TSource, Maybe<'TValue>> * 
        resultSelector : Func<'TSource, 'TValue, 'TResult> -> Maybe<'TResult> 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*TSource*)<br /></dd><dt>valueSelector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TSource*, <a href="T_CSharpx_Maybe_1">Maybe</a>(*TValue*))<br /></dd><dt>resultSelector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TSource*, *TValue*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /><dt>TValue</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*TResult*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*TSource*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />