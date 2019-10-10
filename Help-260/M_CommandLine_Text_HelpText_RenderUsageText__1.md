# HelpText.RenderUsageText(*T*) Method (ParserResult(*T*))
 

Builds a string with usage text block created using <a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a> data and metadata.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string RenderUsageText<T>(
	ParserResult<T> parserResult
)

```

**VB**<br />
``` VB
Public Shared Function RenderUsageText(Of T) ( 
	parserResult As ParserResult(Of T)
) As String
```

**C++**<br />
``` C++
public:
generic<typename T>
static String^ RenderUsageText(
	ParserResult<T>^ parserResult
)
```

**F#**<br />
``` F#
static member RenderUsageText : 
        parserResult : ParserResult<'T> -> string 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />A parsing computation result.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>Type of parsing computation result.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a><br />Resulting formatted text.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText_RenderUsageText">RenderUsageText Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />