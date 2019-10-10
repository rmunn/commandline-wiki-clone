# InstanceBuilder.Build(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static ParserResult<T> Build<T>(
	Maybe<Func<T>> factory,
	Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> tokenizer,
	IEnumerable<string> arguments,
	StringComparer nameComparer,
	bool ignoreValueCase,
	CultureInfo parsingCulture,
	bool autoHelp,
	bool autoVersion,
	IEnumerable<ErrorType> nonFatalErrors
)

```

**VB**<br />
``` VB
Public Shared Function Build(Of T) ( 
	factory As Maybe(Of Func(Of T)),
	tokenizer As Func(Of IEnumerable(Of String), IEnumerable(Of OptionSpecification), Result(Of IEnumerable(Of Token), Error)),
	arguments As IEnumerable(Of String),
	nameComparer As StringComparer,
	ignoreValueCase As Boolean,
	parsingCulture As CultureInfo,
	autoHelp As Boolean,
	autoVersion As Boolean,
	nonFatalErrors As IEnumerable(Of ErrorType)
) As ParserResult(Of T)
```

**C++**<br />
``` C++
public:
generic<typename T>
static ParserResult<T>^ Build(
	Maybe<Func<T>^>^ factory, 
	Func<IEnumerable<String^>^, IEnumerable<OptionSpecification^>^, Result<IEnumerable<Token^>^, Error^>^>^ tokenizer, 
	IEnumerable<String^>^ arguments, 
	StringComparer^ nameComparer, 
	bool ignoreValueCase, 
	CultureInfo^ parsingCulture, 
	bool autoHelp, 
	bool autoVersion, 
	IEnumerable<ErrorType>^ nonFatalErrors
)
```

**F#**<br />
``` F#
static member Build : 
        factory : Maybe<Func<'T>> * 
        tokenizer : Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> * 
        arguments : IEnumerable<string> * 
        nameComparer : StringComparer * 
        ignoreValueCase : bool * 
        parsingCulture : CultureInfo * 
        autoHelp : bool * 
        autoVersion : bool * 
        nonFatalErrors : IEnumerable<ErrorType> -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>factory</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">Func</a>(*T*))<br /></dd><dt>tokenizer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>), <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>))<br /></dd><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>nameComparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd><dt>ignoreValueCase</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>parsingCulture</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo" target="_blank">System.Globalization.CultureInfo</a><br /></dd><dt>autoHelp</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>autoVersion</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>nonFatalErrors</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_ErrorType">ErrorType</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceBuilder">InstanceBuilder Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />