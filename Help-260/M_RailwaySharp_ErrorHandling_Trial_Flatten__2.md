# Trial.Flatten(*TSuccess*, *TMessage*) Method 
 

Flattens a nested result given the Failure types are equal.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Flatten<TSuccess, TMessage>(
	Result<Result<TSuccess, TMessage>, TMessage> result
)

```

**VB**<br />
``` VB
Public Shared Function Flatten(Of TSuccess, TMessage) ( 
	result As Result(Of Result(Of TSuccess, TMessage), TMessage)
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Flatten(
	Result<Result<TSuccess, TMessage>^, TMessage>^ result
)
```

**F#**<br />
``` F#
static member Flatten : 
        result : Result<Result<'TSuccess, 'TMessage>, 'TMessage> -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(<a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*), *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />