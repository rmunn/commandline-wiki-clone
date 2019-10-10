# HelpText Constructor (SentenceBuilder, String, String)
 

Initializes a new instance of the <a href="T_CommandLine_Text_HelpText">HelpText</a> class specifying heading and copyright strings.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText(
	SentenceBuilder sentenceBuilder,
	string heading,
	string copyright
)
```

**VB**<br />
``` VB
Public Sub New ( 
	sentenceBuilder As SentenceBuilder,
	heading As String,
	copyright As String
)
```

**C++**<br />
``` C++
public:
HelpText(
	SentenceBuilder^ sentenceBuilder, 
	String^ heading, 
	String^ copyright
)
```

**F#**<br />
``` F#
new : 
        sentenceBuilder : SentenceBuilder * 
        heading : string * 
        copyright : string -> HelpText
```


#### Parameters
&nbsp;<dl><dt>sentenceBuilder</dt><dd>Type: <a href="T_CommandLine_Text_SentenceBuilder">CommandLine.Text.SentenceBuilder</a><br />A <a href="P_CommandLine_Text_HelpText_SentenceBuilder">SentenceBuilder</a> instance.</dd><dt>heading</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />A string with heading or an instance of <a href="T_CommandLine_Text_HeadingInfo">HeadingInfo</a>.</dd><dt>copyright</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />A string with copyright or an instance of <a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo</a>.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown when one or more parameters are null or empty strings.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText__ctor">HelpText Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />