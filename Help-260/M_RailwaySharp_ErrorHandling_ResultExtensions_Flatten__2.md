# ResultExtensions.Flatten(*TSuccess*, *TMessage*) Method 
 

Collects a sequence of Results and accumulates their values. If the sequence contains an error the error will be propagated.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<IEnumerable<TSuccess>, TMessage> Flatten<TSuccess, TMessage>(
	this Result<IEnumerable<Result<TSuccess, TMessage>>, TMessage> result
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Flatten(Of TSuccess, TMessage) ( 
	result As Result(Of IEnumerable(Of Result(Of TSuccess, TMessage)), TMessage)
) As Result(Of IEnumerable(Of TSuccess), TMessage)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSuccess, typename TMessage>
static Result<IEnumerable<TSuccess>^, TMessage>^ Flatten(
	Result<IEnumerable<Result<TSuccess, TMessage>^>^, TMessage>^ result
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Flatten : 
        result : Result<IEnumerable<Result<'TSuccess, 'TMessage>>, 'TMessage> -> Result<IEnumerable<'TSuccess>, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)), *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSuccess*), *TMessage*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*)), *TMessage*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />