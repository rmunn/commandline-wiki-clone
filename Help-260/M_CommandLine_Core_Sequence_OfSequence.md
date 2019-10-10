# Sequence.OfSequence Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<Token> OfSequence(
	this IEnumerable<Token> tokens,
	Token nameToken,
	TypeDescriptor info
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function OfSequence ( 
	tokens As IEnumerable(Of Token),
	nameToken As Token,
	info As TypeDescriptor
) As IEnumerable(Of Token)
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static IEnumerable<Token^>^ OfSequence(
	IEnumerable<Token^>^ tokens, 
	Token^ nameToken, 
	TypeDescriptor info
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member OfSequence : 
        tokens : IEnumerable<Token> * 
        nameToken : Token * 
        info : TypeDescriptor -> IEnumerable<Token> 

```


#### Parameters
&nbsp;<dl><dt>tokens</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)<br /></dd><dt>nameToken</dt><dd>Type: <a href="T_CommandLine_Core_Token">CommandLine.Core.Token</a><br /></dd><dt>info</dt><dd>Type: <a href="T_CommandLine_Core_TypeDescriptor">CommandLine.Core.TypeDescriptor</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_Sequence">Sequence Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />