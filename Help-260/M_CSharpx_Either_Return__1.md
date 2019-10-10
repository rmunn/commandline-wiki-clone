# Either.Return(*TRight*) Method 
 

Inject a value into the Either type, returning Right case.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<string, TRight> Return<TRight>(
	TRight value
)

```

**VB**<br />
``` VB
Public Shared Function Return(Of TRight) ( 
	value As TRight
) As Either(Of String, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TRight>
static Either<String^, TRight>^ Return(
	TRight value
)
```

**F#**<br />
``` F#
static member Return : 
        value : 'TRight -> Either<string, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *TRight*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />