# MaybeExtensions.Select(*TSource*, *TResult*) Method 
 

Map operation compatible with Linq.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<TResult> Select<TSource, TResult>(
	this Maybe<TSource> maybe,
	Func<TSource, TResult> selector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Select(Of TSource, TResult) ( 
	maybe As Maybe(Of TSource),
	selector As Func(Of TSource, TResult)
) As Maybe(Of TResult)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSource, typename TResult>
static Maybe<TResult>^ Select(
	Maybe<TSource>^ maybe, 
	Func<TSource, TResult>^ selector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Select : 
        maybe : Maybe<'TSource> * 
        selector : Func<'TSource, 'TResult> -> Maybe<'TResult> 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*TSource*)<br /></dd><dt>selector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TSource*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*TResult*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*TSource*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />