# InstanceChooser.MatchVerb Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static ParserResult<Object> MatchVerb(
	Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> tokenizer,
	IEnumerable<Tuple<Verb, Type>> verbs,
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
Private Shared Function MatchVerb ( 
	tokenizer As Func(Of IEnumerable(Of String), IEnumerable(Of OptionSpecification), Result(Of IEnumerable(Of Token), Error)),
	verbs As IEnumerable(Of Tuple(Of Verb, Type)),
	arguments As IEnumerable(Of String),
	nameComparer As StringComparer,
	ignoreValueCase As Boolean,
	parsingCulture As CultureInfo,
	autoHelp As Boolean,
	autoVersion As Boolean,
	nonFatalErrors As IEnumerable(Of ErrorType)
) As ParserResult(Of Object)
```

**C++**<br />
``` C++
private:
static ParserResult<Object^>^ MatchVerb(
	Func<IEnumerable<String^>^, IEnumerable<OptionSpecification^>^, Result<IEnumerable<Token^>^, Error^>^>^ tokenizer, 
	IEnumerable<Tuple<Verb^, Type^>^>^ verbs, 
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
private static member MatchVerb : 
        tokenizer : Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> * 
        verbs : IEnumerable<Tuple<Verb, Type>> * 
        arguments : IEnumerable<string> * 
        nameComparer : StringComparer * 
        ignoreValueCase : bool * 
        parsingCulture : CultureInfo * 
        autoHelp : bool * 
        autoVersion : bool * 
        nonFatalErrors : IEnumerable<ErrorType> -> ParserResult<Object> 

```


#### Parameters
&nbsp;<dl><dt>tokenizer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>), <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>))<br /></dd><dt>verbs</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="T_CommandLine_Core_Verb">Verb</a>, <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>))<br /></dd><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>nameComparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd><dt>ignoreValueCase</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>parsingCulture</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo" target="_blank">System.Globalization.CultureInfo</a><br /></dd><dt>autoHelp</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>autoVersion</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>nonFatalErrors</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_ErrorType">ErrorType</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceChooser">InstanceChooser Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />