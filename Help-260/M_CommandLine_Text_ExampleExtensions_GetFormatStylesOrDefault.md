# ExampleExtensions.GetFormatStylesOrDefault Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<UnParserSettings> GetFormatStylesOrDefault(
	this Example example
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function GetFormatStylesOrDefault ( 
	example As Example
) As IEnumerable(Of UnParserSettings)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static IEnumerable<UnParserSettings^>^ GetFormatStylesOrDefault(
	Example^ example
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member GetFormatStylesOrDefault : 
        example : Example -> IEnumerable<UnParserSettings> 

```


#### Parameters
&nbsp;<dl><dt>example</dt><dd>Type: <a href="T_CommandLine_Text_Example">CommandLine.Text.Example</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_UnParserSettings">UnParserSettings</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Text_Example">Example</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Text_ExampleExtensions">ExampleExtensions Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />