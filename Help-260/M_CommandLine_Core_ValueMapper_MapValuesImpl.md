# ValueMapper.MapValuesImpl Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<Tuple<SpecificationProperty, Maybe<Error>>> MapValuesImpl(
	IEnumerable<SpecificationProperty> specProps,
	IEnumerable<string> values,
	Func<IEnumerable<string>, Type, bool, Maybe<Object>> converter
)
```

**VB**<br />
``` VB
Private Shared Function MapValuesImpl ( 
	specProps As IEnumerable(Of SpecificationProperty),
	values As IEnumerable(Of String),
	converter As Func(Of IEnumerable(Of String), Type, Boolean, Maybe(Of Object))
) As IEnumerable(Of Tuple(Of SpecificationProperty, Maybe(Of Error)))
```

**C++**<br />
``` C++
private:
static IEnumerable<Tuple<SpecificationProperty^, Maybe<Error^>^>^>^ MapValuesImpl(
	IEnumerable<SpecificationProperty^>^ specProps, 
	IEnumerable<String^>^ values, 
	Func<IEnumerable<String^>^, Type^, bool, Maybe<Object^>^>^ converter
)
```

**F#**<br />
``` F#
private static member MapValuesImpl : 
        specProps : IEnumerable<SpecificationProperty> * 
        values : IEnumerable<string> * 
        converter : Func<IEnumerable<string>, Type, bool, Maybe<Object>> -> IEnumerable<Tuple<SpecificationProperty, Maybe<Error>>> 

```


#### Parameters
&nbsp;<dl><dt>specProps</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>values</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>converter</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-4" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>, <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>))<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>, <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="T_CommandLine_Error">Error</a>)))

## See Also


#### Reference
<a href="T_CommandLine_Core_ValueMapper">ValueMapper Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />