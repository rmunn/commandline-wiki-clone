# Example Constructor (String, IEnumerable(UnParserSettings), Object)
 

Initializes a new instance of the <a href="T_CommandLine_Text_Example">Example</a> class.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public Example(
	string helpText,
	IEnumerable<UnParserSettings> formatStyles,
	Object sample
)
```

**VB**<br />
``` VB
Public Sub New ( 
	helpText As String,
	formatStyles As IEnumerable(Of UnParserSettings),
	sample As Object
)
```

**C++**<br />
``` C++
public:
Example(
	String^ helpText, 
	IEnumerable<UnParserSettings^>^ formatStyles, 
	Object^ sample
)
```

**F#**<br />
``` F#
new : 
        helpText : string * 
        formatStyles : IEnumerable<UnParserSettings> * 
        sample : Object -> Example
```


#### Parameters
&nbsp;<dl><dt>helpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />Example description.</dd><dt>formatStyles</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_UnParserSettings">UnParserSettings</a>)<br />A <a href="T_CommandLine_UnParserSettings">UnParserSettings</a> instances sequence that defines command line arguments format.</dd><dt>sample</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />A sample instance.</dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Text_Example">Example Class</a><br /><a href="Overload_CommandLine_Text_Example__ctor">Example Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />