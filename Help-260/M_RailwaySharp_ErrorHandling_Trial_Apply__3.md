# Trial.Apply(*TValue*, *TSuccess*, *TMessage*) Method 
 

If the wrapped function is a success and the given result is a success the function is applied on the value. Otherwise the exisiting error messages are propagated.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Apply<TValue, TSuccess, TMessage>(
	Result<Func<TValue, TSuccess>, TMessage> wrappedFunction,
	Result<TValue, TMessage> result
)

```

**VB**<br />
``` VB
Public Shared Function Apply(Of TValue, TSuccess, TMessage) ( 
	wrappedFunction As Result(Of Func(Of TValue, TSuccess), TMessage),
	result As Result(Of TValue, TMessage)
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TValue, typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Apply(
	Result<Func<TValue, TSuccess>^, TMessage>^ wrappedFunction, 
	Result<TValue, TMessage>^ result
)
```

**F#**<br />
``` F#
static member Apply : 
        wrappedFunction : Result<Func<'TValue, 'TSuccess>, 'TMessage> * 
        result : Result<'TValue, 'TMessage> -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>wrappedFunction</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(*TValue*, *TSuccess*), *TMessage*)<br /></dd><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TValue*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TValue</dt><dd /><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />