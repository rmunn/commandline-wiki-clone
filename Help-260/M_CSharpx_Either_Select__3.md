# Either.Select(*TLeft*, *TRight*, *TResult*) Method 
 

Map operation compatible with Linq.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<TLeft, TResult> Select<TLeft, TRight, TResult>(
	this Either<TLeft, TRight> either,
	Func<TRight, TResult> selector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Select(Of TLeft, TRight, TResult) ( 
	either As Either(Of TLeft, TRight),
	selector As Func(Of TRight, TResult)
) As Either(Of TLeft, TResult)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TLeft, typename TRight, typename TResult>
static Either<TLeft, TResult>^ Select(
	Either<TLeft, TRight>^ either, 
	Func<TRight, TResult>^ selector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Select : 
        either : Either<'TLeft, 'TRight> * 
        selector : Func<'TRight, 'TResult> -> Either<'TLeft, 'TResult> 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>selector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TRight*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TResult*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />