# Result.Try(*TSuccess*) Method 
 

Executes the given function on a given success or captures the failure.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TSuccess, Exception> Try<TSuccess>(
	Func<TSuccess> func
)

```

**VB**<br />
``` VB
Public Shared Function Try(Of TSuccess) ( 
	func As Func(Of TSuccess)
) As Result(Of TSuccess, Exception)
```

**C++**<br />
``` C++
public:
generic<typename TSuccess>
static Result<TSuccess, Exception^>^ Try(
	Func<TSuccess>^ func
)
```

**F#**<br />
``` F#
static member Try : 
        func : Func<'TSuccess> -> Result<'TSuccess, Exception> 

```


#### Parameters
&nbsp;<dl><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">System.Func</a>(*TSuccess*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, <a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">Exception</a>)

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_Result">Result Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />