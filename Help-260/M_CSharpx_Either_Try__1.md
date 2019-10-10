# Either.Try(*TRight*) Method 
 

Wraps a function, encapsulates any exception thrown within to a Either.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<Exception, TRight> Try<TRight>(
	Func<TRight> func
)

```

**VB**<br />
``` VB
Public Shared Function Try(Of TRight) ( 
	func As Func(Of TRight)
) As Either(Of Exception, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TRight>
static Either<Exception^, TRight>^ Try(
	Func<TRight>^ func
)
```

**F#**<br />
``` F#
static member Try : 
        func : Func<'TRight> -> Either<Exception, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">System.Func</a>(*TRight*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(<a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">Exception</a>, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />