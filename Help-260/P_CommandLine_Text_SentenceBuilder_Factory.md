# SentenceBuilder.Factory Property 
 

Factory to allow custom SentenceBuilder injection

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Func<SentenceBuilder> Factory { get; set; }
```

**VB**<br />
``` VB
Public Shared Property Factory As Func(Of SentenceBuilder)
	Get
	Set
```

**C++**<br />
``` C++
public:
static property Func<SentenceBuilder^>^ Factory {
	Func<SentenceBuilder^>^ get ();
	void set (Func<SentenceBuilder^>^ value);
}
```

**F#**<br />
``` F#
static member Factory : Func<SentenceBuilder> with get, set

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">Func</a>(<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder</a>)

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />