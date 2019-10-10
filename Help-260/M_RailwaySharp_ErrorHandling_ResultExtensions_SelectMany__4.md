# ResultExtensions.SelectMany(*TSuccess*, *TMessage*, *TValue*, *TResult*) Method (Result(*TSuccess*, *TMessage*), Func(*TSuccess*, Result(*TValue*, *TMessage*)), Func(*TSuccess*, *TValue*, *TResult*))
 

If the result is a Success it executes the given Func on the value. If the result of the Func is a Success it maps it using the given Func. Otherwise the exisiting failure is propagated.

**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<TResult, TMessage> SelectMany<TSuccess, TMessage, TValue, TResult>(
	this Result<TSuccess, TMessage> result,
	Func<TSuccess, Result<TValue, TMessage>> func,
	Func<TSuccess, TValue, TResult> mapperFunc
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function SelectMany(Of TSuccess, TMessage, TValue, TResult) ( 
	result As Result(Of TSuccess, TMessage),
	func As Func(Of TSuccess, Result(Of TValue, TMessage)),
	mapperFunc As Func(Of TSuccess, TValue, TResult)
) As Result(Of TResult, TMessage)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSuccess, typename TMessage, typename TValue, typename TResult>
static Result<TResult, TMessage>^ SelectMany(
	Result<TSuccess, TMessage>^ result, 
	Func<TSuccess, Result<TValue, TMessage>^>^ func, 
	Func<TSuccess, TValue, TResult>^ mapperFunc
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member SelectMany : 
        result : Result<'TSuccess, 'TMessage> * 
        func : Func<'TSuccess, Result<'TValue, 'TMessage>> * 
        mapperFunc : Func<'TSuccess, 'TValue, 'TResult> -> Result<'TResult, 'TMessage> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TSuccess*, <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TValue*, *TMessage*))<br /></dd><dt>mapperFunc</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TSuccess*, *TValue*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /><dt>TValue</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TResult*, *TMessage*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="Overload_RailwaySharp_ErrorHandling_ResultExtensions_SelectMany">SelectMany Overload</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />