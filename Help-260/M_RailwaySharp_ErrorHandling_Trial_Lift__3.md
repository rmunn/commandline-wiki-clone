# Trial.Lift(*TValue*, *TSuccess*, *TMessage*) Method 
 

Lifts a function into a Result container and applies it on the given result.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, TMessage> Lift<TValue, TSuccess, TMessage>(
	Func<TValue, TSuccess> func,
	Result<TValue, TMessage> result
)

```

**VB**<br />
``` VB
Public Shared Function Lift(Of TValue, TSuccess, TMessage) ( 
	func As Func(Of TValue, TSuccess),
	result As Result(Of TValue, TMessage)
) As Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
public:
generic<typename TValue, typename TSuccess, typename TMessage>
static Result<TSuccess, TMessage>^ Lift(
	Func<TValue, TSuccess>^ func, 
	Result<TValue, TMessage>^ result
)
```

**F#**<br />
``` F#
static member Lift : 
        func : Func<'TValue, 'TSuccess> * 
        result : Result<'TValue, 'TMessage> -> Result<'TSuccess, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TValue*, *TSuccess*)<br /></dd><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TValue*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TValue</dt><dd /><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />