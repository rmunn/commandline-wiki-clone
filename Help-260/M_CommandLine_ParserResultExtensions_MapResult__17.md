# ParserResultExtensions.MapResult(*T1*, *T2*, *T3*, *T4*, *T5*, *T6*, *T7*, *T8*, *T9*, *T10*, *T11*, *T12*, *T13*, *T14*, *T15*, *T16*, *TResult*) Method (ParserResult(Object), Func(*T1*, *TResult*), Func(*T2*, *TResult*), Func(*T3*, *TResult*), Func(*T4*, *TResult*), Func(*T5*, *TResult*), Func(*T6*, *TResult*), Func(*T7*, *TResult*), Func(*T8*, *TResult*), Func(*T9*, *TResult*), Func(*T10*, *TResult*), Func(*T11*, *TResult*), Func(*T12*, *TResult*), Func(*T13*, *TResult*), Func(*T14*, *TResult*), Func(*T15*, *TResult*), Func(*T16*, *TResult*), Func(IEnumerable(Error), *TResult*))
 

Provides a way to transform result data into another value.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TResult MapResult<T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13, T14, T15, T16, TResult>(
	this ParserResult<Object> result,
	Func<T1, TResult> parsedFunc1,
	Func<T2, TResult> parsedFunc2,
	Func<T3, TResult> parsedFunc3,
	Func<T4, TResult> parsedFunc4,
	Func<T5, TResult> parsedFunc5,
	Func<T6, TResult> parsedFunc6,
	Func<T7, TResult> parsedFunc7,
	Func<T8, TResult> parsedFunc8,
	Func<T9, TResult> parsedFunc9,
	Func<T10, TResult> parsedFunc10,
	Func<T11, TResult> parsedFunc11,
	Func<T12, TResult> parsedFunc12,
	Func<T13, TResult> parsedFunc13,
	Func<T14, TResult> parsedFunc14,
	Func<T15, TResult> parsedFunc15,
	Func<T16, TResult> parsedFunc16,
	Func<IEnumerable<Error>, TResult> notParsedFunc
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function MapResult(Of T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13, T14, T15, T16, TResult) ( 
	result As ParserResult(Of Object),
	parsedFunc1 As Func(Of T1, TResult),
	parsedFunc2 As Func(Of T2, TResult),
	parsedFunc3 As Func(Of T3, TResult),
	parsedFunc4 As Func(Of T4, TResult),
	parsedFunc5 As Func(Of T5, TResult),
	parsedFunc6 As Func(Of T6, TResult),
	parsedFunc7 As Func(Of T7, TResult),
	parsedFunc8 As Func(Of T8, TResult),
	parsedFunc9 As Func(Of T9, TResult),
	parsedFunc10 As Func(Of T10, TResult),
	parsedFunc11 As Func(Of T11, TResult),
	parsedFunc12 As Func(Of T12, TResult),
	parsedFunc13 As Func(Of T13, TResult),
	parsedFunc14 As Func(Of T14, TResult),
	parsedFunc15 As Func(Of T15, TResult),
	parsedFunc16 As Func(Of T16, TResult),
	notParsedFunc As Func(Of IEnumerable(Of Error), TResult)
) As TResult
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2, typename T3, typename T4, typename T5, typename T6, typename T7, typename T8, typename T9, typename T10, typename T11, typename T12, typename T13, typename T14, typename T15, typename T16, typename TResult>
static TResult MapResult(
	ParserResult<Object^>^ result, 
	Func<T1, TResult>^ parsedFunc1, 
	Func<T2, TResult>^ parsedFunc2, 
	Func<T3, TResult>^ parsedFunc3, 
	Func<T4, TResult>^ parsedFunc4, 
	Func<T5, TResult>^ parsedFunc5, 
	Func<T6, TResult>^ parsedFunc6, 
	Func<T7, TResult>^ parsedFunc7, 
	Func<T8, TResult>^ parsedFunc8, 
	Func<T9, TResult>^ parsedFunc9, 
	Func<T10, TResult>^ parsedFunc10, 
	Func<T11, TResult>^ parsedFunc11, 
	Func<T12, TResult>^ parsedFunc12, 
	Func<T13, TResult>^ parsedFunc13, 
	Func<T14, TResult>^ parsedFunc14, 
	Func<T15, TResult>^ parsedFunc15, 
	Func<T16, TResult>^ parsedFunc16, 
	Func<IEnumerable<Error^>^, TResult>^ notParsedFunc
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member MapResult : 
        result : ParserResult<Object> * 
        parsedFunc1 : Func<'T1, 'TResult> * 
        parsedFunc2 : Func<'T2, 'TResult> * 
        parsedFunc3 : Func<'T3, 'TResult> * 
        parsedFunc4 : Func<'T4, 'TResult> * 
        parsedFunc5 : Func<'T5, 'TResult> * 
        parsedFunc6 : Func<'T6, 'TResult> * 
        parsedFunc7 : Func<'T7, 'TResult> * 
        parsedFunc8 : Func<'T8, 'TResult> * 
        parsedFunc9 : Func<'T9, 'TResult> * 
        parsedFunc10 : Func<'T10, 'TResult> * 
        parsedFunc11 : Func<'T11, 'TResult> * 
        parsedFunc12 : Func<'T12, 'TResult> * 
        parsedFunc13 : Func<'T13, 'TResult> * 
        parsedFunc14 : Func<'T14, 'TResult> * 
        parsedFunc15 : Func<'T15, 'TResult> * 
        parsedFunc16 : Func<'T16, 'TResult> * 
        notParsedFunc : Func<IEnumerable<Error>, 'TResult> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br />The result in verb scenario.</dd><dt>parsedFunc1</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T1*, *TResult*)<br />Lambda executed on successful parsing of *T1*.</dd><dt>parsedFunc2</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T2*, *TResult*)<br />Lambda executed on successful parsing of *T2*.</dd><dt>parsedFunc3</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T3*, *TResult*)<br />Lambda executed on successful parsing of *T3*.</dd><dt>parsedFunc4</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T4*, *TResult*)<br />Lambda executed on successful parsing of *T4*.</dd><dt>parsedFunc5</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T5*, *TResult*)<br />Lambda executed on successful parsing of *T5*.</dd><dt>parsedFunc6</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T6*, *TResult*)<br />Lambda executed on successful parsing of *T6*.</dd><dt>parsedFunc7</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T7*, *TResult*)<br />Lambda executed on successful parsing of *T7*.</dd><dt>parsedFunc8</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T8*, *TResult*)<br />Lambda executed on successful parsing of *T8*.</dd><dt>parsedFunc9</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T9*, *TResult*)<br />Lambda executed on successful parsing of *T9*.</dd><dt>parsedFunc10</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T10*, *TResult*)<br />Lambda executed on successful parsing of *T10*.</dd><dt>parsedFunc11</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T11*, *TResult*)<br />Lambda executed on successful parsing of *T11*.</dd><dt>parsedFunc12</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T12*, *TResult*)<br />Lambda executed on successful parsing of *T12*.</dd><dt>parsedFunc13</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T13*, *TResult*)<br />Lambda executed on successful parsing of *T13*.</dd><dt>parsedFunc14</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T14*, *TResult*)<br />Lambda executed on successful parsing of *T14*.</dd><dt>parsedFunc15</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T15*, *TResult*)<br />Lambda executed on successful parsing of *T15*.</dd><dt>parsedFunc16</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T16*, *TResult*)<br />Lambda executed on successful parsing of *T16*.</dd><dt>notParsedFunc</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>), *TResult*)<br />Lambda executed on failed parsing.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd>First verb type.</dd><dt>T2</dt><dd>Second verb type.</dd><dt>T3</dt><dd>Third verb type.</dd><dt>T4</dt><dd>Fourth verb type.</dd><dt>T5</dt><dd>Fifth verb type.</dd><dt>T6</dt><dd>Sixth verb type.</dd><dt>T7</dt><dd>Seventh verb type.</dd><dt>T8</dt><dd>Eighth verb type.</dd><dt>T9</dt><dd>Ninth verb type.</dd><dt>T10</dt><dd>Tenth verb type.</dd><dt>T11</dt><dd>Eleventh verb type.</dd><dt>T12</dt><dd>Twelfth verb type.</dd><dt>T13</dt><dd>Thirteenth verb type.</dd><dt>T14</dt><dd>Fourteenth verb type.</dd><dt>T15</dt><dd>Fifteenth verb type.</dd><dt>T16</dt><dd>Sixteenth verb type.</dd><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*<br />The new value.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_ParserResult_1">ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions Class</a><br /><a href="Overload_CommandLine_ParserResultExtensions_MapResult">MapResult Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />