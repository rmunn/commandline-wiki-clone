# ParserResultExtensions.WithParsed(*T*) Method (ParserResult(*T*), Action(*T*))
 

Executes *action* if <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> contains parsed values.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static ParserResult<T> WithParsed<T>(
	this ParserResult<T> result,
	Action<T> action
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function WithParsed(Of T) ( 
	result As ParserResult(Of T),
	action As Action(Of T)
) As ParserResult(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static ParserResult<T>^ WithParsed(
	ParserResult<T>^ result, 
	Action<T>^ action
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member WithParsed : 
        result : ParserResult<'T> * 
        action : Action<'T> -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />An <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> instance.</dd><dt>action</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*T*)<br />The <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> to execute.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>Type of the target instance built with parsed value.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)<br />The same *result* instance.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions Class</a><br /><a href="Overload_CommandLine_ParserResultExtensions_WithParsed">WithParsed Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />