# OptionSpecification.FromAttribute Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static OptionSpecification FromAttribute(
	OptionAttribute attribute,
	Type conversionType,
	IEnumerable<string> enumValues
)
```

**VB**<br />
``` VB
Public Shared Function FromAttribute ( 
	attribute As OptionAttribute,
	conversionType As Type,
	enumValues As IEnumerable(Of String)
) As OptionSpecification
```

**C++**<br />
``` C++
public:
static OptionSpecification^ FromAttribute(
	OptionAttribute^ attribute, 
	Type^ conversionType, 
	IEnumerable<String^>^ enumValues
)
```

**F#**<br />
``` F#
static member FromAttribute : 
        attribute : OptionAttribute * 
        conversionType : Type * 
        enumValues : IEnumerable<string> -> OptionSpecification 

```


#### Parameters
&nbsp;<dl><dt>attribute</dt><dd>Type: <a href="T_CommandLine_OptionAttribute">CommandLine.OptionAttribute</a><br /></dd><dt>conversionType</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>enumValues</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>

## See Also


#### Reference
<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />