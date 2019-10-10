# TypeConverter.ChangeTypeScalar Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Maybe<Object> ChangeTypeScalar(
	string value,
	Type conversionType,
	CultureInfo conversionCulture,
	bool ignoreValueCase
)
```

**VB**<br />
``` VB
Private Shared Function ChangeTypeScalar ( 
	value As String,
	conversionType As Type,
	conversionCulture As CultureInfo,
	ignoreValueCase As Boolean
) As Maybe(Of Object)
```

**C++**<br />
``` C++
private:
static Maybe<Object^>^ ChangeTypeScalar(
	String^ value, 
	Type^ conversionType, 
	CultureInfo^ conversionCulture, 
	bool ignoreValueCase
)
```

**F#**<br />
``` F#
private static member ChangeTypeScalar : 
        value : string * 
        conversionType : Type * 
        conversionCulture : CultureInfo * 
        ignoreValueCase : bool -> Maybe<Object> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>conversionType</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>conversionCulture</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo" target="_blank">System.Globalization.CultureInfo</a><br /></dd><dt>ignoreValueCase</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeConverter">TypeConverter Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />