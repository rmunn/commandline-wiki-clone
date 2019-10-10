# Trial.Fail(*TSuccess*, *TMessage*) Method 
 

Wraps a message in a Failure.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Fail<TSuccess, TMessage>(
	TMessage message
)

```

**VB**<br />
``` VB
Public Shared Function Fail(Of TSuccess, TMessage) ( 
	message As TMessage
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Fail(
	TMessage message
)
```

**F#**<br />
``` F#
static member Fail : 
        message : 'TMessage -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>message</dt><dd>Type: *TMessage*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />