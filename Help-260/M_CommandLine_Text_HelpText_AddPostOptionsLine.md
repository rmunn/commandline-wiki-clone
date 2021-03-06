# HelpText.AddPostOptionsLine Method 
 

Adds a text line at the bottom, after options usage string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText AddPostOptionsLine(
	string value
)
```

**VB**<br />
``` VB
Public Function AddPostOptionsLine ( 
	value As String
) As HelpText
```

**C++**<br />
``` C++
public:
HelpText^ AddPostOptionsLine(
	String^ value
)
```

**F#**<br />
``` F#
member AddPostOptionsLine : 
        value : string -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a><br />Updated <a href="T_CommandLine_Text_HelpText">HelpText</a> instance.

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown when parameter *value* is null or empty string.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />