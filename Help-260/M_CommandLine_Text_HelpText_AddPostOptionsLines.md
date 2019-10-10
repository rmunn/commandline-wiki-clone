# HelpText.AddPostOptionsLines Method 
 

Adds text lines at the bottom, after options usage string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText AddPostOptionsLines(
	IEnumerable<string> lines
)
```

**VB**<br />
``` VB
Public Function AddPostOptionsLines ( 
	lines As IEnumerable(Of String)
) As HelpText
```

**C++**<br />
``` C++
public:
HelpText^ AddPostOptionsLines(
	IEnumerable<String^>^ lines
)
```

**F#**<br />
``` F#
member AddPostOptionsLines : 
        lines : IEnumerable<string> -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>lines</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> sequence of line to add.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a><br />Updated <a href="T_CommandLine_Text_HelpText">HelpText</a> instance.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />