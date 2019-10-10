# HelpText&nbsp;Implicit Conversion (HelpText to String)
 

Converts the help instance to a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static implicit operator string (
	HelpText info
)
```

**VB**<br />
``` VB
Public Shared Widening Operator CType ( 
	info As HelpText
) As String
```

**C++**<br />
``` C++
static implicit operator String^ (
	HelpText^ info
)
```

**F#**<br />
``` F#

```


#### Parameters
&nbsp;<dl><dt>info</dt><dd>Type: <a href="T_CommandLine_Text_HelpText">CommandLine.Text.HelpText</a><br />This <a href="T_CommandLine_Text_HelpText">HelpText</a> instance.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a><br />The <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> that contains the help screen.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />