# HeadingInfo.WriteMessage Method (String, TextWriter)
 

Writes out a string and a new line using the program name specified in the constructor and *message* parameter.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public void WriteMessage(
	string message,
	TextWriter writer
)
```

**VB**<br />
``` VB
Public Sub WriteMessage ( 
	message As String,
	writer As TextWriter
)
```

**C++**<br />
``` C++
public:
void WriteMessage(
	String^ message, 
	TextWriter^ writer
)
```

**F#**<br />
``` F#
member WriteMessage : 
        message : string * 
        writer : TextWriter -> unit 

```


#### Parameters
&nbsp;<dl><dt>message</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> message to write.</dd><dt>writer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">System.IO.TextWriter</a><br />The target <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a> derived type.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown when parameter *message* is null or empty string.</td></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown when parameter *writer* is null.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HeadingInfo">HeadingInfo Class</a><br /><a href="Overload_CommandLine_Text_HeadingInfo_WriteMessage">WriteMessage Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />