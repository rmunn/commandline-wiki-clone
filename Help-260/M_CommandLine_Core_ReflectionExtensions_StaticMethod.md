# ReflectionExtensions.StaticMethod Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Object StaticMethod(
	this Type type,
	string name,
	params Object[] args
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function StaticMethod ( 
	type As Type,
	name As String,
	ParamArray args As Object()
) As Object
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static Object^ StaticMethod(
	Type^ type, 
	String^ name, 
	... array<Object^>^ args
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member StaticMethod : 
        type : Type * 
        name : string * 
        args : Object[] -> Object 

```


#### Parameters
&nbsp;<dl><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>name</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>args</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a>[]<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />