# Parser.HandleUnknownArguments Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<ErrorType> HandleUnknownArguments(
	bool ignoreUnknownArguments
)
```

**VB**<br />
``` VB
Private Shared Function HandleUnknownArguments ( 
	ignoreUnknownArguments As Boolean
) As IEnumerable(Of ErrorType)
```

**C++**<br />
``` C++
private:
static IEnumerable<ErrorType>^ HandleUnknownArguments(
	bool ignoreUnknownArguments
)
```

**F#**<br />
``` F#
private static member HandleUnknownArguments : 
        ignoreUnknownArguments : bool -> IEnumerable<ErrorType> 

```


#### Parameters
&nbsp;<dl><dt>ignoreUnknownArguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_ErrorType">ErrorType</a>)

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />