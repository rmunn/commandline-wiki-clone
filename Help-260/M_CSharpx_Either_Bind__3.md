# Either.Bind(*TLeft*, *TRight*, *TResult*) Method 
 

Monadic bind.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<TLeft, TResult> Bind<TLeft, TRight, TResult>(
	Either<TLeft, TRight> either,
	Func<TRight, Either<TLeft, TResult>> func
)

```

**VB**<br />
``` VB
Public Shared Function Bind(Of TLeft, TRight, TResult) ( 
	either As Either(Of TLeft, TRight),
	func As Func(Of TRight, Either(Of TLeft, TResult))
) As Either(Of TLeft, TResult)
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight, typename TResult>
static Either<TLeft, TResult>^ Bind(
	Either<TLeft, TRight>^ either, 
	Func<TRight, Either<TLeft, TResult>^>^ func
)
```

**F#**<br />
``` F#
static member Bind : 
        either : Either<'TLeft, 'TRight> * 
        func : Func<'TRight, Either<'TLeft, 'TResult>> -> Either<'TLeft, 'TResult> 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TRight*, <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TResult*))<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TResult*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />