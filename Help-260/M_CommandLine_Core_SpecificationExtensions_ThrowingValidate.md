# SpecificationExtensions.ThrowingValidate Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Specification> ThrowingValidate(
	this IEnumerable<Specification> specifications,
	IEnumerable<Tuple<Func<Specification, bool>, string>> guardsLookup
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ThrowingValidate ( 
	specifications As IEnumerable(Of Specification),
	guardsLookup As IEnumerable(Of Tuple(Of Func(Of Specification, Boolean), String))
) As IEnumerable(Of Specification)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static IEnumerable<Specification^>^ ThrowingValidate(
	IEnumerable<Specification^>^ specifications, 
	IEnumerable<Tuple<Func<Specification^, bool>^, String^>^>^ guardsLookup
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ThrowingValidate : 
        specifications : IEnumerable<Specification> * 
        guardsLookup : IEnumerable<Tuple<Func<Specification, bool>, string>> -> IEnumerable<Specification> 

```


#### Parameters
&nbsp;<dl><dt>specifications</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Specification">Specification</a>)<br /></dd><dt>guardsLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="T_CommandLine_Core_Specification">Specification</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>), <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>))<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Specification">Specification</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Specification">Specification</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationExtensions">SpecificationExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />