# Trial.Lift2(*TSuccess*, *TMessage*, *TSuccess1*, *TMessage1*) Method 
 

Promote a function to a monad/applicative, scanning the monadic/applicative arguments from left to right.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess1, TMessage1> Lift2<TSuccess, TMessage, TSuccess1, TMessage1>(
	Func<TSuccess, Func<TMessage, TSuccess1>> func,
	Result<TSuccess, TMessage1> a,
	Result<TMessage, TMessage1> b
)

```

**VB**<br />
``` VB
Public Shared Function Lift2(Of TSuccess, TMessage, TSuccess1, TMessage1) ( 
	func As Func(Of TSuccess, Func(Of TMessage, TSuccess1)),
	a As Result(Of TSuccess, TMessage1),
	b As Result(Of TMessage, TMessage1)
) As Result(Of TSuccess1, TMessage1)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess, typename TMessage, typename TSuccess1, typename TMessage1>
static Result<TSuccess1, TMessage1>^ Lift2(
	Func<TSuccess, Func<TMessage, TSuccess1>^>^ func, 
	Result<TSuccess, TMessage1>^ a, 
	Result<TMessage, TMessage1>^ b
)
```

**F#**<br />
``` F#
static member Lift2 : 
        func : Func<'TSuccess, Func<'TMessage, 'TSuccess1>> * 
        a : Result<'TSuccess, 'TMessage1> * 
        b : Result<'TMessage, 'TMessage1> -> Result<'TSuccess1, 'TMessage1> 

```


#### Parameters
&nbsp;<dl><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TSuccess*, <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(*TMessage*, *TSuccess1*))<br /></dd><dt>a</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage1*)<br /></dd><dt>b</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TMessage*, *TMessage1*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /><dt>TSuccess1</dt><dd /><dt>TMessage1</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess1*, *TMessage1*)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Trial">Trial Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />