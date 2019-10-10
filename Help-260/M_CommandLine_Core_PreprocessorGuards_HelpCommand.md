# PreprocessorGuards.HelpCommand Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Func<IEnumerable<string>, IEnumerable<Error>> HelpCommand(
	StringComparer nameComparer
)
```

**VB**<br />
``` VB
Public Shared Function HelpCommand ( 
	nameComparer As StringComparer
) As Func(Of IEnumerable(Of String), IEnumerable(Of Error))
```

**C++**<br />
``` C++
public:
static Func<IEnumerable<String^>^, IEnumerable<Error^>^>^ HelpCommand(
	StringComparer^ nameComparer
)
```

**F#**<br />
``` F#
static member HelpCommand : 
        nameComparer : StringComparer -> Func<IEnumerable<string>, IEnumerable<Error>> 

```


#### Parameters
&nbsp;<dl><dt>nameComparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>))

## See Also


#### Reference
<a href="T_CommandLine_Core_PreprocessorGuards">PreprocessorGuards Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />