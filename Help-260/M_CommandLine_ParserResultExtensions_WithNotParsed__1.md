# ParserResultExtensions.WithNotParsed(*T*) Method 
 

Executes *action* if <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> lacks parsed values and contains errors.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static ParserResult<T> WithNotParsed<T>(
	this ParserResult<T> result,
	Action<IEnumerable<Error>> action
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function WithNotParsed(Of T) ( 
	result As ParserResult(Of T),
	action As Action(Of IEnumerable(Of Error))
) As ParserResult(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static ParserResult<T>^ WithNotParsed(
	ParserResult<T>^ result, 
	Action<IEnumerable<Error^>^>^ action
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member WithNotParsed : 
        result : ParserResult<'T> * 
        action : Action<IEnumerable<Error>> -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />An <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> instance.</dd><dt>action</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>))<br />The <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">Action</a> delegate to execute.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>Type of the target instance built with parsed value.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)<br />The same *result* instance.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />