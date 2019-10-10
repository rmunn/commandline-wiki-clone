# HelpText Constructor (String)
 

Initializes a new instance of the <a href="T_CommandLine_Text_HelpText">HelpText</a> class specifying heading string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText(
	string heading
)
```

**VB**<br />
``` VB
Public Sub New ( 
	heading As String
)
```

**C++**<br />
``` C++
public:
HelpText(
	String^ heading
)
```

**F#**<br />
``` F#
new : 
        heading : string -> HelpText
```


#### Parameters
&nbsp;<dl><dt>heading</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />An heading string or an instance of <a href="T_CommandLine_Text_HeadingInfo">HeadingInfo</a>.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown when parameter *heading* is null or empty string.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText__ctor">HelpText Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />