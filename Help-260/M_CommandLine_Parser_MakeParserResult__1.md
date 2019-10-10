# Parser.MakeParserResult(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static ParserResult<T> MakeParserResult<T>(
	ParserResult<T> parserResult,
	ParserSettings settings
)

```

**VB**<br />
``` VB
Private Shared Function MakeParserResult(Of T) ( 
	parserResult As ParserResult(Of T),
	settings As ParserSettings
) As ParserResult(Of T)
```

**C++**<br />
``` C++
private:
generic<typename T>
static ParserResult<T>^ MakeParserResult(
	ParserResult<T>^ parserResult, 
	ParserSettings^ settings
)
```

**F#**<br />
``` F#
private static member MakeParserResult : 
        parserResult : ParserResult<'T> * 
        settings : ParserSettings -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br /></dd><dt>settings</dt><dd>Type: <a href="T_CommandLine_ParserSettings">CommandLine.ParserSettings</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />