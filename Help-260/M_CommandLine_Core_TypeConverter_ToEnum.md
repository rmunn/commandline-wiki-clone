# TypeConverter.ToEnum Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Object ToEnum(
	this string value,
	Type conversionType,
	bool ignoreValueCase
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function ToEnum ( 
	value As String,
	conversionType As Type,
	ignoreValueCase As Boolean
) As Object
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static Object^ ToEnum(
	String^ value, 
	Type^ conversionType, 
	bool ignoreValueCase
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member ToEnum : 
        value : string * 
        conversionType : Type * 
        ignoreValueCase : bool -> Object 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>conversionType</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>ignoreValueCase</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeConverter">TypeConverter Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />