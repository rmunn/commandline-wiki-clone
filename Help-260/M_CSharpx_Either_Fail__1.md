# Either.Fail(*TRight*) Method 
 

Fail with a message. Not part of mathematical definition of a monad.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<string, TRight> Fail<TRight>(
	string message
)

```

**VB**<br />
``` VB
Public Shared Function Fail(Of TRight) ( 
	message As String
) As Either(Of String, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TRight>
static Either<String^, TRight>^ Fail(
	String^ message
)
```

**F#**<br />
``` F#
static member Fail : 
        message : string -> Either<string, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>message</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />