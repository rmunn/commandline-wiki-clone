# MaybeExtensions.MatchJust(*T1*, *T2*) Method 
 

Matches a value returning `true` and tupled value itself via two output parameters.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool MatchJust<T1, T2>(
	this Maybe<Tuple<T1, T2>> maybe,
	out T1 value1,
	out T2 value2
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function MatchJust(Of T1, T2) ( 
	maybe As Maybe(Of Tuple(Of T1, T2)),
	<OutAttribute> ByRef value1 As T1,
	<OutAttribute> ByRef value2 As T2
) As Boolean
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2>
static bool MatchJust(
	Maybe<Tuple<T1, T2>^>^ maybe, 
	[OutAttribute] T1% value1, 
	[OutAttribute] T2% value2
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member MatchJust : 
        maybe : Maybe<Tuple<'T1, 'T2>> * 
        value1 : 'T1 byref * 
        value2 : 'T2 byref -> bool 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(*T1*, *T2*))<br /></dd><dt>value1</dt><dd>Type: *T1*<br /></dd><dt>value2</dt><dd>Type: *T2*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd /><dt>T2</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(*T1*, *T2*)). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />