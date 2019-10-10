# ArgumentsExtensions.Preprocess Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Error> Preprocess(
	this IEnumerable<string> arguments,
	IEnumerable<Func<IEnumerable<string>, IEnumerable<Error>>> preprocessorLookup
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Preprocess ( 
	arguments As IEnumerable(Of String),
	preprocessorLookup As IEnumerable(Of Func(Of IEnumerable(Of String), IEnumerable(Of Error)))
) As IEnumerable(Of Error)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static IEnumerable<Error^>^ Preprocess(
	IEnumerable<String^>^ arguments, 
	IEnumerable<Func<IEnumerable<String^>^, IEnumerable<Error^>^>^>^ preprocessorLookup
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Preprocess : 
        arguments : IEnumerable<string> * 
        preprocessorLookup : IEnumerable<Func<IEnumerable<string>, IEnumerable<Error>>> -> IEnumerable<Error> 

```


#### Parameters
&nbsp;<dl><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>preprocessorLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)))<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ArgumentsExtensions">ArgumentsExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />