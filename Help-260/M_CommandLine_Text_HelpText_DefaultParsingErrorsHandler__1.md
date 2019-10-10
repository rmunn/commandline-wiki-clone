# HelpText.DefaultParsingErrorsHandler(*T*) Method 
 

Supplies a default parsing error handler implementation.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static HelpText DefaultParsingErrorsHandler<T>(
	ParserResult<T> parserResult,
	HelpText current
)

```

**VB**<br />
``` VB
Public Shared Function DefaultParsingErrorsHandler(Of T) ( 
	parserResult As ParserResult(Of T),
	current As HelpText
) As HelpText
```

**C++**<br />
``` C++
public:
generic<typename T>
static HelpText^ DefaultParsingErrorsHandler(
	ParserResult<T>^ parserResult, 
	HelpText^ current
)
```

**F#**<br />
``` F#
static member DefaultParsingErrorsHandler : 
        parserResult : ParserResult<'T> * 
        current : HelpText -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />The <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the instance that collected command line arguments parsed with <a href="T_CommandLine_Parser">Parser</a> class.</dd><dt>current</dt><dd>Type: <a href="T_CommandLine_Text_HelpText">CommandLine.Text.HelpText</a><br />The <a href="T_CommandLine_Text_HelpText">HelpText</a> instance.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />