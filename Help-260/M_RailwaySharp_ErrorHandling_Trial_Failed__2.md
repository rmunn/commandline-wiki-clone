# Trial.Failed(*TSuccess*, *TMessage*) Method 
 

Returns true if the result was not successful.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool Failed<TSuccess, TMessage>(
	Result<TSuccess, TMessage> result
)

```

**VB**<br />
``` VB
Public Shared Function Failed(Of TSuccess, TMessage) ( 
	result As Result(Of TSuccess, TMessage)
) As Boolean
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static bool Failed(
	Result<TSuccess, TMessage>^ result
)
```

**F#**<br />
``` F#
static member Failed : 
        result : Result<'TSuccess, 'TMessage> -> bool 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />