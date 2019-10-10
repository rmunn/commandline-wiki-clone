# NameLookup.HavingSeparator Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<char> HavingSeparator(
	string name,
	IEnumerable<OptionSpecification> specifications,
	StringComparer comparer
)
```

**VB**<br />
``` VB
Public Shared Function HavingSeparator ( 
	name As String,
	specifications As IEnumerable(Of OptionSpecification),
	comparer As StringComparer
) As Maybe(Of Char)
```

**C++**<br />
``` C++
public:
static Maybe<wchar_t>^ HavingSeparator(
	String^ name, 
	IEnumerable<OptionSpecification^>^ specifications, 
	StringComparer^ comparer
)
```

**F#**<br />
``` F#
static member HavingSeparator : 
        name : string * 
        specifications : IEnumerable<OptionSpecification> * 
        comparer : StringComparer -> Maybe<char> 

```


#### Parameters
&nbsp;<dl><dt>name</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>specifications</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>)<br /></dd><dt>comparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.char" target="_blank">Char</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_NameLookup">NameLookup Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />