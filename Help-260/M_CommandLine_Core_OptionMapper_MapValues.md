# OptionMapper.MapValues Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<IEnumerable<SpecificationProperty>, Error> MapValues(
	IEnumerable<SpecificationProperty> propertyTuples,
	IEnumerable<KeyValuePair<string, IEnumerable<string>>> options,
	Func<IEnumerable<string>, Type, bool, Maybe<Object>> converter,
	StringComparer comparer
)
```

**VB**<br />
``` VB
Public Shared Function MapValues ( 
	propertyTuples As IEnumerable(Of SpecificationProperty),
	options As IEnumerable(Of KeyValuePair(Of String, IEnumerable(Of String))),
	converter As Func(Of IEnumerable(Of String), Type, Boolean, Maybe(Of Object)),
	comparer As StringComparer
) As Result(Of IEnumerable(Of SpecificationProperty), Error)
```

**C++**<br />
``` C++
public:
static Result<IEnumerable<SpecificationProperty^>^, Error^>^ MapValues(
	IEnumerable<SpecificationProperty^>^ propertyTuples, 
	IEnumerable<KeyValuePair<String^, IEnumerable<String^>^>>^ options, 
	Func<IEnumerable<String^>^, Type^, bool, Maybe<Object^>^>^ converter, 
	StringComparer^ comparer
)
```

**F#**<br />
``` F#
static member MapValues : 
        propertyTuples : IEnumerable<SpecificationProperty> * 
        options : IEnumerable<KeyValuePair<string, IEnumerable<string>>> * 
        converter : Func<IEnumerable<string>, Type, bool, Maybe<Object>> * 
        comparer : StringComparer -> Result<IEnumerable<SpecificationProperty>, Error> 

```


#### Parameters
&nbsp;<dl><dt>propertyTuples</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>options</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)))<br /></dd><dt>converter</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-4" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>, <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>))<br /></dd><dt>comparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>), <a href="T_CommandLine_Error">Error</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_OptionMapper">OptionMapper Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />