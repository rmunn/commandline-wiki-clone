# HelpText.AutoBuild(*T*) Method (ParserResult(*T*), Int32)
 

Creates a new instance of the <a href="T_CommandLine_Text_HelpText">HelpText</a> class, automatically handling verbs or options scenario.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static HelpText AutoBuild<T>(
	ParserResult<T> parserResult,
	int maxDisplayWidth = 80
)

```

**VB**<br />
``` VB
Public Shared Function AutoBuild(Of T) ( 
	parserResult As ParserResult(Of T),
	Optional maxDisplayWidth As Integer = 80
) As HelpText
```

**C++**<br />
``` C++
public:
generic<typename T>
static HelpText^ AutoBuild(
	ParserResult<T>^ parserResult, 
	int maxDisplayWidth = 80
)
```

**F#**<br />
``` F#
static member AutoBuild : 
        parserResult : ParserResult<'T> * 
        ?maxDisplayWidth : int 
(* Defaults:
        let _maxDisplayWidth = defaultArg maxDisplayWidth 80
*)
-> HelpText 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />The <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the instance that collected command line arguments parsed with <a href="T_CommandLine_Parser">Parser</a> class.</dd><dt>maxDisplayWidth (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The maximum width of the display.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a><br />An instance of <a href="T_CommandLine_Text_HelpText">HelpText</a> class.

## Remarks
This feature is meant to be invoked automatically by the parser, setting the HelpWriter property of <a href="T_CommandLine_ParserSettings">ParserSettings</a>.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText_AutoBuild">AutoBuild Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />