# SentenceBuilder.FormatError Property 
 

Gets a delegate that handles singular error formatting. The delegates must accept an <a href="T_CommandLine_Error">Error</a> and returns a string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract Func<Error, string> FormatError { get; }
```

**VB**<br />
``` VB
Public MustOverride ReadOnly Property FormatError As Func(Of Error, String)
	Get
```

**C++**<br />
``` C++
public:
virtual property Func<Error^, String^>^ FormatError {
	Func<Error^, String^>^ get () abstract;
}
```

**F#**<br />
``` F#
abstract FormatError : Func<Error, string> with get

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="T_CommandLine_Error">Error</a>, <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />