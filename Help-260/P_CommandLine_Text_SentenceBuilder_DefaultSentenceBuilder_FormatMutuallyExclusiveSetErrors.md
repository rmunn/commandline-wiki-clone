# SentenceBuilder.DefaultSentenceBuilder.FormatMutuallyExclusiveSetErrors Property 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public override Func<IEnumerable<MutuallyExclusiveSetError>, string> FormatMutuallyExclusiveSetErrors { get; }
```

**VB**<br />
``` VB
Public Overrides ReadOnly Property FormatMutuallyExclusiveSetErrors As Func(Of IEnumerable(Of MutuallyExclusiveSetError), String)
	Get
```

**C++**<br />
``` C++
public:
virtual property Func<IEnumerable<MutuallyExclusiveSetError^>^, String^>^ FormatMutuallyExclusiveSetErrors {
	Func<IEnumerable<MutuallyExclusiveSetError^>^, String^>^ get () override;
}
```

**F#**<br />
``` F#
abstract FormatMutuallyExclusiveSetErrors : Func<IEnumerable<MutuallyExclusiveSetError>, string> with get
override FormatMutuallyExclusiveSetErrors : Func<IEnumerable<MutuallyExclusiveSetError>, string> with get
```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_MutuallyExclusiveSetError">MutuallyExclusiveSetError</a>), <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder_DefaultSentenceBuilder">SentenceBuilder.DefaultSentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />