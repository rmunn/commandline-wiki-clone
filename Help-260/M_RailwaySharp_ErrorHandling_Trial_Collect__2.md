# Trial.Collect(*TSuccess*, *TMessage*) Method 
 

Collects a sequence of Results and accumulates their values. If the sequence contains an error the error will be propagated.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<IEnumerable<TSuccess>, TMessage> Collect<TSuccess, TMessage>(
	IEnumerable<Result<TSuccess, TMessage>> xs
)

```

**VB**<br />
``` VB
Public Shared Function Collect(Of TSuccess, TMessage) ( 
	xs As IEnumerable(Of Result(Of TSuccess, TMessage))
) As Result(Of IEnumerable(Of TSuccess), TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<IEnumerable<TSuccess>^, TMessage>^ Collect(
	IEnumerable<Result<TSuccess, TMessage>^>^ xs
)
```

**F#**<br />
``` F#
static member Collect : 
        xs : IEnumerable<Result<'TSuccess, 'TMessage>> -> Result<IEnumerable<'TSuccess>, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>xs</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*))<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSuccess*), *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />