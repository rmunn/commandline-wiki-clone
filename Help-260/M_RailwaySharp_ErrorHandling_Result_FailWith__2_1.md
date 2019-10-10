# Result.FailWith(*TSuccess*, *TMessage*) Method (*TMessage*)
 

Creates a Failure result with the given message.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> FailWith<TSuccess, TMessage>(
	TMessage message
)

```

**VB**<br />
``` VB
Public Shared Function FailWith(Of TSuccess, TMessage) ( 
	message As TMessage
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ FailWith(
	TMessage message
)
```

**F#**<br />
``` F#
static member FailWith : 
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
<a href="T_RailwaySharp_ErrorHandling_Result">Result Class</a><br /><a href="Overload_RailwaySharp_ErrorHandling_Result_FailWith">FailWith Overload</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />