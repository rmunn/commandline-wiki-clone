# Trial.Pass(*TSuccess*, *TMessage*) Method 
 

Wraps a value in a Success.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Pass<TSuccess, TMessage>(
	TSuccess value
)

```

**VB**<br />
``` VB
Public Shared Function Pass(Of TSuccess, TMessage) ( 
	value As TSuccess
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Pass(
	TSuccess value
)
```

**F#**<br />
``` F#
static member Pass : 
        value : 'TSuccess -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *TSuccess*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />