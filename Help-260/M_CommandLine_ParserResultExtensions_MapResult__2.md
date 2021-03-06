# ParserResultExtensions.MapResult(*T1*, *TResult*) Method (ParserResult(Object), Func(*T1*, *TResult*), Func(IEnumerable(Error), *TResult*))
 

Provides a way to transform result data into another value.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TResult MapResult<T1, TResult>(
	this ParserResult<Object> result,
	Func<T1, TResult> parsedFunc1,
	Func<IEnumerable<Error>, TResult> notParsedFunc
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function MapResult(Of T1, TResult) ( 
	result As ParserResult(Of Object),
	parsedFunc1 As Func(Of T1, TResult),
	notParsedFunc As Func(Of IEnumerable(Of Error), TResult)
) As TResult
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename TResult>
static TResult MapResult(
	ParserResult<Object^>^ result, 
	Func<T1, TResult>^ parsedFunc1, 
	Func<IEnumerable<Error^>^, TResult>^ notParsedFunc
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member MapResult : 
        result : ParserResult<Object> * 
        parsedFunc1 : Func<'T1, 'TResult> * 
        notParsedFunc : Func<IEnumerable<Error>, 'TResult> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br />The result in verb scenario.</dd><dt>parsedFunc1</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T1*, *TResult*)<br />Lambda executed on successful parsing of *T1*.</dd><dt>notParsedFunc</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>), *TResult*)<br />Lambda executed on failed parsing.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd>First verb type.</dd><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*<br />The new value.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_ParserResult_1">ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions Class</a><br /><a href="Overload_CommandLine_ParserResultExtensions_MapResult">MapResult Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />