# TypeConverter.ConvertString Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Object ConvertString(
	string value,
	Type type,
	CultureInfo conversionCulture
)
```

**VB**<br />
``` VB
Private Shared Function ConvertString ( 
	value As String,
	type As Type,
	conversionCulture As CultureInfo
) As Object
```

**C++**<br />
``` C++
private:
static Object^ ConvertString(
	String^ value, 
	Type^ type, 
	CultureInfo^ conversionCulture
)
```

**F#**<br />
``` F#
private static member ConvertString : 
        value : string * 
        type : Type * 
        conversionCulture : CultureInfo -> Object 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>conversionCulture</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo" target="_blank">System.Globalization.CultureInfo</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeConverter">TypeConverter Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />