# UnParserExtensions.SeperatorOrSpace Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static char SeperatorOrSpace(
	this Specification spec
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function SeperatorOrSpace ( 
	spec As Specification
) As Char
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static wchar_t SeperatorOrSpace(
	Specification^ spec
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member SeperatorOrSpace : 
        spec : Specification -> char 

```


#### Parameters
&nbsp;<dl><dt>spec</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.char" target="_blank">Char</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_Specification">Specification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_UnParserExtensions">UnParserExtensions Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />