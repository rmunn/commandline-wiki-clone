# ResultExtensions.FailedWith(*TSuccess*, *TMessage*) Method 
 

Returns the error messages or fails if the result was a success.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<TMessage> FailedWith<TSuccess, TMessage>(
	this Result<TSuccess, TMessage> result
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function FailedWith(Of TSuccess, TMessage) ( 
	result As Result(Of TSuccess, TMessage)
) As IEnumerable(Of TMessage)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSuccess, typename TMessage>
static IEnumerable<TMessage>^ FailedWith(
	Result<TSuccess, TMessage>^ result
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member FailedWith : 
        result : Result<'TSuccess, 'TMessage> -> IEnumerable<'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TMessage*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />