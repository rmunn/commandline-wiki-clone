# Parser.DisplayHelp(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static ParserResult<T> DisplayHelp<T>(
	ParserResult<T> parserResult,
	TextWriter helpWriter,
	int maxDisplayWidth
)

```

**VB**<br />
``` VB
Private Shared Function DisplayHelp(Of T) ( 
	parserResult As ParserResult(Of T),
	helpWriter As TextWriter,
	maxDisplayWidth As Integer
) As ParserResult(Of T)
```

**C++**<br />
``` C++
private:
generic<typename T>
static ParserResult<T>^ DisplayHelp(
	ParserResult<T>^ parserResult, 
	TextWriter^ helpWriter, 
	int maxDisplayWidth
)
```

**F#**<br />
``` F#
private static member DisplayHelp : 
        parserResult : ParserResult<'T> * 
        helpWriter : TextWriter * 
        maxDisplayWidth : int -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br /></dd><dt>helpWriter</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">System.IO.TextWriter</a><br /></dd><dt>maxDisplayWidth</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />