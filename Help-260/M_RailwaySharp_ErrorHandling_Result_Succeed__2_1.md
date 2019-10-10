# Result.Succeed(*TSuccess*, *TMessage*) Method (*TSuccess*, IEnumerable(*TMessage*))
 

Creates a Success result with the given value and the given messages.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Succeed<TSuccess, TMessage>(
	TSuccess value,
	IEnumerable<TMessage> messages
)

```

**VB**<br />
``` VB
Public Shared Function Succeed(Of TSuccess, TMessage) ( 
	value As TSuccess,
	messages As IEnumerable(Of TMessage)
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Succeed(
	TSuccess value, 
	IEnumerable<TMessage>^ messages
)
```

**F#**<br />
``` F#
static member Succeed : 
        value : 'TSuccess * 
        messages : IEnumerable<'TMessage> -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *TSuccess*<br /></dd><dt>messages</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Result">Result Class</a><br /><a href="Overload_RailwaySharp_ErrorHandling_Result_Succeed">Succeed Overload</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />