# ResultExtensions.Either(*TSuccess*, *TMessage*, *TResult*) Method 
 

Allows pattern matching on Results.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TResult Either<TSuccess, TMessage, TResult>(
	this Result<TSuccess, TMessage> result,
	Func<TSuccess, IEnumerable<TMessage>, TResult> ifSuccess,
	Func<IEnumerable<TMessage>, TResult> ifFailure
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Either(Of TSuccess, TMessage, TResult) ( 
	result As Result(Of TSuccess, TMessage),
	ifSuccess As Func(Of TSuccess, IEnumerable(Of TMessage), TResult),
	ifFailure As Func(Of IEnumerable(Of TMessage), TResult)
) As TResult
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSuccess, typename TMessage, typename TResult>
static TResult Either(
	Result<TSuccess, TMessage>^ result, 
	Func<TSuccess, IEnumerable<TMessage>^, TResult>^ ifSuccess, 
	Func<IEnumerable<TMessage>^, TResult>^ ifFailure
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Either : 
        result : Result<'TSuccess, 'TMessage> * 
        ifSuccess : Func<'TSuccess, IEnumerable<'TMessage>, 'TResult> * 
        ifFailure : Func<IEnumerable<'TMessage>, 'TResult> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd><dt>ifSuccess</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TSuccess*, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TMessage*), *TResult*)<br /></dd><dt>ifFailure</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TMessage*), *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />