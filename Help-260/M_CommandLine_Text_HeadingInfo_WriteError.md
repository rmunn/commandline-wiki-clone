# HeadingInfo.WriteError Method 
 

Writes out a string and a new line using the program name specified in the constructor and *message* parameter to standard error stream.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public void WriteError(
	string message
)
```

**VB**<br />
``` VB
Public Sub WriteError ( 
	message As String
)
```

**C++**<br />
``` C++
public:
void WriteError(
	String^ message
)
```

**F#**<br />
``` F#
member WriteError : 
        message : string -> unit 

```


#### Parameters
&nbsp;<dl><dt>message</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> message to write.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown when parameter *message* is null or empty string.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HeadingInfo">HeadingInfo Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />