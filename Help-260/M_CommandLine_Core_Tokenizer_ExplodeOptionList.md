# Tokenizer.ExplodeOptionList Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<IEnumerable<Token>, Error> ExplodeOptionList(
	Result<IEnumerable<Token>, Error> tokenizerResult,
	Func<string, Maybe<char>> optionSequenceWithSeparatorLookup
)
```

**VB**<br />
``` VB
Public Shared Function ExplodeOptionList ( 
	tokenizerResult As Result(Of IEnumerable(Of Token), Error),
	optionSequenceWithSeparatorLookup As Func(Of String, Maybe(Of Char))
) As Result(Of IEnumerable(Of Token), Error)
```

**C++**<br />
``` C++
public:
static Result<IEnumerable<Token^>^, Error^>^ ExplodeOptionList(
	Result<IEnumerable<Token^>^, Error^>^ tokenizerResult, 
	Func<String^, Maybe<wchar_t>^>^ optionSequenceWithSeparatorLookup
)
```

**F#**<br />
``` F#
static member ExplodeOptionList : 
        tokenizerResult : Result<IEnumerable<Token>, Error> * 
        optionSequenceWithSeparatorLookup : Func<string, Maybe<char>> -> Result<IEnumerable<Token>, Error> 

```


#### Parameters
&nbsp;<dl><dt>tokenizerResult</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>)<br /></dd><dt>optionSequenceWithSeparatorLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.char" target="_blank">Char</a>))<br /></dd></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />