# TypeLookup.FindTypeDescriptorAndSibling Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<TypeDescriptor> FindTypeDescriptorAndSibling(
	string name,
	IEnumerable<OptionSpecification> specifications,
	StringComparer comparer
)
```

**VB**<br />
``` VB
Public Shared Function FindTypeDescriptorAndSibling ( 
	name As String,
	specifications As IEnumerable(Of OptionSpecification),
	comparer As StringComparer
) As Maybe(Of TypeDescriptor)
```

**C++**<br />
``` C++
public:
static Maybe<TypeDescriptor>^ FindTypeDescriptorAndSibling(
	String^ name, 
	IEnumerable<OptionSpecification^>^ specifications, 
	StringComparer^ comparer
)
```

**F#**<br />
``` F#
static member FindTypeDescriptorAndSibling : 
        name : string * 
        specifications : IEnumerable<OptionSpecification> * 
        comparer : StringComparer -> Maybe<TypeDescriptor> 

```


#### Parameters
&nbsp;<dl><dt>name</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>specifications</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>)<br /></dd><dt>comparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeLookup">TypeLookup Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />