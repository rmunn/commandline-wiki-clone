# StringExtensions.ToStringLocal(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string ToStringLocal<T>(
	this T value
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ToStringLocal(Of T) ( 
	value As T
) As String
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static String^ ToStringLocal(
	T value
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ToStringLocal : 
        value : 'T -> string 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type . When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_StringExtensions">StringExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />