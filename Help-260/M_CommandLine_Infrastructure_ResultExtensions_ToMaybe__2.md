# ResultExtensions.ToMaybe(*TSuccess*, *TMessage*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<TSuccess> ToMaybe<TSuccess, TMessage>(
	this Result<TSuccess, TMessage> result
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ToMaybe(Of TSuccess, TMessage) ( 
	result As Result(Of TSuccess, TMessage)
) As Maybe(Of TSuccess)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSuccess, typename TMessage>
static Maybe<TSuccess>^ ToMaybe(
	Result<TSuccess, TMessage>^ result
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ToMaybe : 
        result : Result<'TSuccess, 'TMessage> -> Maybe<'TSuccess> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd /><dt>TMessage</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*TSuccess*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(*TSuccess*, *TMessage*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_ResultExtensions">ResultExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />