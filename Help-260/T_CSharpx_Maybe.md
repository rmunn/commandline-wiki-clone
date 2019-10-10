# Maybe Class
 

Provides static methods for manipulating Maybe.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.Maybe<br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class Maybe
```

**VB**<br />
``` VB
Friend NotInheritable Class Maybe
```

**C++**<br />
``` C++
internal ref class Maybe abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
type Maybe =  class end
```

The Maybe type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Bind__2">Bind(T1, T2)</a></td><td>
Sequentially compose two actions, passing any value produced by the first as an argument to the second.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Just__1">Just(T)</a></td><td>
Builds the case when Maybe contains a value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Map__2">Map(T1, T2)</a></td><td>
Transforms an maybe value by using a specified mapping function.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Merge__2">Merge(T1, T2)</a></td><td>
If both maybes contain a value, it merges them into a maybe with a tupled value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Nothing__1">Nothing(T)</a></td><td>
Builds the empty case of Maybe.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Maybe_Return__1">Return(T)</a></td><td>
Inject a value into the monadic <a href="T_CSharpx_Maybe_1">Maybe(T)</a> type.</td></tr></table>&nbsp;
<a href="#maybe-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />