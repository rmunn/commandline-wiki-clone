# SpecificationPropertyExtensions.Validate Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Error> Validate(
	this IEnumerable<SpecificationProperty> specProps,
	IEnumerable<Func<IEnumerable<SpecificationProperty>, IEnumerable<Error>>> rules
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Validate ( 
	specProps As IEnumerable(Of SpecificationProperty),
	rules As IEnumerable(Of Func(Of IEnumerable(Of SpecificationProperty), IEnumerable(Of Error)))
) As IEnumerable(Of Error)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static IEnumerable<Error^>^ Validate(
	IEnumerable<SpecificationProperty^>^ specProps, 
	IEnumerable<Func<IEnumerable<SpecificationProperty^>^, IEnumerable<Error^>^>^>^ rules
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Validate : 
        specProps : IEnumerable<SpecificationProperty> * 
        rules : IEnumerable<Func<IEnumerable<SpecificationProperty>, IEnumerable<Error>>> -> IEnumerable<Error> 

```


#### Parameters
&nbsp;<dl><dt>specProps</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>rules</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)))<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationPropertyExtensions">SpecificationPropertyExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />