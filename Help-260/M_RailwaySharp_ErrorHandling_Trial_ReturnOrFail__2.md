# Trial.ReturnOrFail(*TSuccess*, *TMessage*) Method 
 

If the given result is a Success the wrapped value will be returned. Otherwise the function throws an exception with Failure message of the result.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TSuccess ReturnOrFail<TSuccess, TMessage>(
	Result<TSuccess, TMessage> result
)

```

**VB**<br />
``` VB
Public Shared Function ReturnOrFail(Of TSuccess, TMessage) ( 
	result As Result(Of TSuccess, TMessage)
) As TSuccess
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static TSuccess ReturnOrFail(
	Result<TSuccess, TMessage>^ result
)
```

**F#**<br />
``` F#
static member ReturnOrFail : 
        result : Result<'TSuccess, 'TMessage> -> 'TSuccess 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: *TSuccess*

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />