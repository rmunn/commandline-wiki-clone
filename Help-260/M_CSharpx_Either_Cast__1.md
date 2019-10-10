# Either.Cast(*TRight*) Method 
 

Attempts to cast an object. Stores the cast value in 1Of2 if successful, otherwise stores the exception in 2Of2

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<Exception, TRight> Cast<TRight>(
	Object obj
)

```

**VB**<br />
``` VB
Public Shared Function Cast(Of TRight) ( 
	obj As Object
) As Either(Of Exception, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TRight>
static Either<Exception^, TRight>^ Cast(
	Object^ obj
)
```

**F#**<br />
``` F#
static member Cast : 
        obj : Object -> Either<Exception, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>obj</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(<a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">Exception</a>, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />