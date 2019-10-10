# ReflectionExtensions.GetVerbSpecification Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<VerbAttribute> GetVerbSpecification(
	this Type type
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function GetVerbSpecification ( 
	type As Type
) As Maybe(Of VerbAttribute)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static Maybe<VerbAttribute^>^ GetVerbSpecification(
	Type^ type
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member GetVerbSpecification : 
        type : Type -> Maybe<VerbAttribute> 

```


#### Parameters
&nbsp;<dl><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="T_CommandLine_VerbAttribute">VerbAttribute</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ReflectionExtensions">ReflectionExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />