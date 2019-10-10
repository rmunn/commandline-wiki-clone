# SentenceBuilder.HelpCommandText Property 
 

Get a delegate that returns the help text of help command. The delegates must accept a boolean that is equal 

#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>, <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />true for options; otherwise 

#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>, <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />false for verbs.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract Func<bool, string> HelpCommandText { get; }
```

**VB**<br />
``` VB
Public MustOverride ReadOnly Property HelpCommandText As Func(Of Boolean, String)
	Get
```

**C++**<br />
``` C++
public:
virtual property Func<bool, String^>^ HelpCommandText {
	Func<bool, String^>^ get () abstract;
}
```

**F#**<br />
``` F#
abstract HelpCommandText : Func<bool, string> with get

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>, <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />