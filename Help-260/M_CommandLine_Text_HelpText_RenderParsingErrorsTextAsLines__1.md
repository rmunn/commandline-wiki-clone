# HelpText.RenderParsingErrorsTextAsLines(*T*) Method 
 

Builds a sequence of string that contains a parsing error message.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<string> RenderParsingErrorsTextAsLines<T>(
	ParserResult<T> parserResult,
	Func<Error, string> formatError,
	Func<IEnumerable<MutuallyExclusiveSetError>, string> formatMutuallyExclusiveSetErrors,
	int indent
)

```

**VB**<br />
``` VB
Public Shared Function RenderParsingErrorsTextAsLines(Of T) ( 
	parserResult As ParserResult(Of T),
	formatError As Func(Of Error, String),
	formatMutuallyExclusiveSetErrors As Func(Of IEnumerable(Of MutuallyExclusiveSetError), String),
	indent As Integer
) As IEnumerable(Of String)
```

**C++**<br />
``` C++
public:
generic<typename T>
static IEnumerable<String^>^ RenderParsingErrorsTextAsLines(
	ParserResult<T>^ parserResult, 
	Func<Error^, String^>^ formatError, 
	Func<IEnumerable<MutuallyExclusiveSetError^>^, String^>^ formatMutuallyExclusiveSetErrors, 
	int indent
)
```

**F#**<br />
``` F#
static member RenderParsingErrorsTextAsLines : 
        parserResult : ParserResult<'T> * 
        formatError : Func<Error, string> * 
        formatMutuallyExclusiveSetErrors : Func<IEnumerable<MutuallyExclusiveSetError>, string> * 
        indent : int -> IEnumerable<string> 

```


#### Parameters
&nbsp;<dl><dt>parserResult</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />The <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the instance that collected command line arguments parsed with <a href="T_CommandLine_Parser">Parser</a> class.</dd><dt>formatError</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="T_CommandLine_Error">Error</a>, <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />The error formatting delegate.</dd><dt>formatMutuallyExclusiveSetErrors</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_MutuallyExclusiveSetError">MutuallyExclusiveSetError</a>), <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />The specialized <a href="T_CommandLine_MutuallyExclusiveSetError">MutuallyExclusiveSetError</a> sequence formatting delegate.</dd><dt>indent</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />Number of spaces used to indent text.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />A sequence of <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> that contains the parsing error message.

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />