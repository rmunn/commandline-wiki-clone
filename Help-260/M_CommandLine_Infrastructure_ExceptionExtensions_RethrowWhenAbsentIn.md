# ExceptionExtensions.RethrowWhenAbsentIn Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void RethrowWhenAbsentIn(
	this Exception exception,
	IEnumerable<Type> validExceptions
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub RethrowWhenAbsentIn ( 
	exception As Exception,
	validExceptions As IEnumerable(Of Type)
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static void RethrowWhenAbsentIn(
	Exception^ exception, 
	IEnumerable<Type^>^ validExceptions
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member RethrowWhenAbsentIn : 
        exception : Exception * 
        validExceptions : IEnumerable<Type> -> unit 

```


#### Parameters
&nbsp;<dl><dt>exception</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">System.Exception</a><br /></dd><dt>validExceptions</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>)<br /></dd></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">Exception</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_ExceptionExtensions">ExceptionExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />