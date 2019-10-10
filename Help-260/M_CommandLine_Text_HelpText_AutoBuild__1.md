# HelpText.AutoBuild(*T*) Method (ParserResult(*T*), Func(HelpText, HelpText), Func(Example, Example), Boolean, Int32)
 

Creates a new instance of the <a href="T_CommandLine_Text_HelpText">HelpText</a> class using common defaults.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static HelpText AutoBuild<T>(
	ParserResult<T> parserResult,
	Func<HelpText, HelpText> onError,
	Func<Example, Example> onExample,
	bool verbsIndex = false,
	int maxDisplayWidth = 80
)

```

**VB**<br />
``` VB
Public Shared Function AutoBuild(Of T) ( 
	parserResult As ParserResult(Of T),
	onError As Func(Of HelpText, HelpText),
	onExample As Func(Of Example, Example),
	Optional verbsIndex As Boolean = false,
	Optional maxDisplayWidth As Integer = 80
) As HelpText
```

**C++**<br />
``` C++
public:
generic<typename T>
static HelpText^ AutoBuild(
	ParserResult<T>^ parserResult, 
	Func<HelpText^, HelpText^>^ onError, 
	Func<Example^, Example^>^ onExample, 
	bool verbsIndex = false, 
	int maxDisplayWidth = 80
)
```

**F#**<br />
``` F#
static member AutoBuild : 
        parserResult : ParserResult<'T> * 
        onError : Func<HelpText, HelpText> * 
        onExample : Func<Example, Example> * 
        ?verbsIndex : bool * 
        ?maxDisplayWidth : int 
(* Defaults:
        let _verbsIndex = defaultArg verbsIndex false
        let _maxDisplayWidth = defaultArg maxDisplayWidth 80
*)
-> HelpText 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />The <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the instance that collected command line arguments parsed with <a href="T_CommandLine_Parser">Parser</a> class.</dd><dt>onError</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="T_CommandLine_Text_HelpText">HelpText</a>, <a href="T_CommandLine_Text_HelpText">HelpText</a>)<br />A delegate used to customize the text block of reporting parsing errors text block.</dd><dt>onExample</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="T_CommandLine_Text_Example">Example</a>, <a href="T_CommandLine_Text_Example">Example</a>)<br />A delegate used to customize <a href="T_CommandLine_Text_Example">Example</a> model used to render text block of usage examples.</dd><dt>verbsIndex (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br />If true the output style is consistent with verb commands (no dashes), otherwise it outputs options.</dd><dt>maxDisplayWidth (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The maximum width of the display.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a><br />An instance of <a href="T_CommandLine_Text_HelpText">HelpText</a> class.

## Remarks
The parameter *verbsIndex* is not ontly a metter of formatting, it controls whether to handle verbs or options.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText_AutoBuild">AutoBuild Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />