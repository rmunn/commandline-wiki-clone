# SentenceBuilder.RequiredWord Property 
 

Gets a delegate that returns the word 'required'.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract Func<string> RequiredWord { get; }
```

**VB**<br />
``` VB
Public MustOverride ReadOnly Property RequiredWord As Func(Of String)
	Get
```

**C++**<br />
``` C++
public:
virtual property Func<String^>^ RequiredWord {
	Func<String^>^ get () abstract;
}
```

**F#**<br />
``` F#
abstract RequiredWord : Func<string> with get

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />