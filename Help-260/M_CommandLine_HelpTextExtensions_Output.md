# HelpTextExtensions.Output Method 
 

redirect errs to Console.Error, and to Console.Out for help/version error

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TextWriter Output(
	this IEnumerable<Error> errs
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Output ( 
	errs As IEnumerable(Of Error)
) As TextWriter
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static TextWriter^ Output(
	IEnumerable<Error^>^ errs
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Output : 
        errs : IEnumerable<Error> -> TextWriter 

```


#### Parameters
&nbsp;<dl><dt>errs</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_HelpTextExtensions">HelpTextExtensions Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />