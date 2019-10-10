# Parser Constructor (Action(ParserSettings))
 

Initializes a new instance of the <a href="T_CommandLine_Parser">Parser</a> class, configurable with <a href="T_CommandLine_ParserSettings">ParserSettings</a> using a delegate.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public Parser(
	Action<ParserSettings> configuration
)
```

**VB**<br />
``` VB
Public Sub New ( 
	configuration As Action(Of ParserSettings)
)
```

**C++**<br />
``` C++
public:
Parser(
	Action<ParserSettings^>^ configuration
)
```

**F#**<br />
``` F#
new : 
        configuration : Action<ParserSettings> -> Parser
```


#### Parameters
&nbsp;<dl><dt>configuration</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(<a href="T_CommandLine_ParserSettings">ParserSettings</a>)<br />The <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> delegate used to configure aspects and behaviors of the parser.</dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="Overload_CommandLine_Parser__ctor">Parser Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />