# Trial.Either(*TSuccess*, *TMessage*, *TResult*) Method 
 

Takes a Result and maps it with successFunc if it is a Success otherwise it maps it with failureFunc.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TResult Either<TSuccess, TMessage, TResult>(
	Func<TSuccess, IEnumerable<TMessage>, TResult> successFunc,
	Func<IEnumerable<TMessage>, TResult> failureFunc,
	Result<TSuccess, TMessage> trialResult
)

```

**VB**<br />
``` VB
Public Shared Function Either(Of TSuccess, TMessage, TResult) ( 
	successFunc As Func(Of TSuccess, IEnumerable(Of TMessage), TResult),
	failureFunc As Func(Of IEnumerable(Of TMessage), TResult),
	trialResult As Result(Of TSuccess, TMessage)
) As TResult
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage, typename TResult>
static TResult Either(
	Func<TSuccess, IEnumerable<TMessage>^, TResult>^ successFunc, 
	Func<IEnumerable<TMessage>^, TResult>^ failureFunc, 
	Result<TSuccess, TMessage>^ trialResult
)
```

**F#**<br />
``` F#
static member Either : 
        successFunc : Func<'TSuccess, IEnumerable<'TMessage>, 'TResult> * 
        failureFunc : Func<IEnumerable<'TMessage>, 'TResult> * 
        trialResult : Result<'TSuccess, 'TMessage> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>successFunc</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TSuccess*, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TMessage*), *TResult*)<br /></dd><dt>failureFunc</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TMessage*), *TResult*)<br /></dd><dt>trialResult</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />