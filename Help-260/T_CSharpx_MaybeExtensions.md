# MaybeExtensions Class
 

Provides convenience extension methods for <a href="T_CSharpx_Maybe">Maybe</a>.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.MaybeExtensions<br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class MaybeExtensions
```

**VB**<br />
``` VB
<ExtensionAttribute>
Friend NotInheritable Class MaybeExtensions
```

**C++**<br />
``` C++
[ExtensionAttribute]
internal ref class MaybeExtensions abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
[<ExtensionAttribute>]
type MaybeExtensions =  class end
```

The MaybeExtensions type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Bind__2">Bind(T1, T2)</a></td><td>
Invokes a function on this maybe value that itself yields a maybe.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Do__1">Do(T)(Maybe(T), Action(T))</a></td><td>
If contans a value executes an <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> delegate over it.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Do__2">Do(T1, T2)(Maybe(Tuple(T1, T2)), Action(T1, T2))</a></td><td>
If contans a value executes an <a href="https://docs.microsoft.com/dotnet/api/system.action-2" target="_blank">Action(T1, T2)</a> delegate over it.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_FromJust__1">FromJust(T)</a></td><td>
Extracts the element out of a <a href="T_CSharpx_Just_1">Just(T)</a> and returns a default value if its argument is <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_FromJustOrFail__1">FromJustOrFail(T)</a></td><td>
Extracts the element out of a <a href="T_CSharpx_Just_1">Just(T)</a> and throws an error if its argument is <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_GetValueOrDefault__1">GetValueOrDefault(T)</a></td><td>
If contains a values returns it, otherwise returns *noneValue*.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_IsJust__1">IsJust(T)</a></td><td>
Returns `true` iffits argument is of the form <a href="T_CSharpx_Just_1">Just(T)</a>.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_IsNothing__1">IsNothing(T)</a></td><td>
Returns `true` iffits argument is of the form <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Map__2">Map(T1, T2)</a></td><td>
Transforms this maybe value by using a specified mapping function.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_MapValueOrDefault__2">MapValueOrDefault(T1, T2)</a></td><td>
If contains a values executes a mapping function over it, otherwise returns *noneValue*.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Match__1">Match(T)(Maybe(T), Action(T), Action)</a></td><td>
Provides pattern matching using <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">Action</a> delegates.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Match__2">Match(T1, T2)(Maybe(Tuple(T1, T2)), Action(T1, T2), Action)</a></td><td>
Provides pattern matching using <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">Action</a> delegates over maybe with tupled wrapped value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_MatchJust__2">MatchJust(T1, T2)</a></td><td>
Matches a value returning `true` and tupled value itself via two output parameters.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_Select__2">Select(TSource, TResult)</a></td><td>
Map operation compatible with Linq.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_SelectMany__3">SelectMany(TSource, TValue, TResult)</a></td><td>
Bind operation compatible with Linq.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_ToEnumerable__1">ToEnumerable(T)</a></td><td>
Returns an empty list when given <a href="T_CSharpx_Nothing_1">Nothing(T)</a> or a singleton list when given a <a href="T_CSharpx_Just_1">Just(T)</a>.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_MaybeExtensions_ToMaybe__1">ToMaybe(T)</a></td><td>
Equivalent to monadic <a href="M_CSharpx_Maybe_Return__1">Return(T)(T)</a> operation. Builds a <a href="T_CSharpx_Just_1">Just(T)</a> value in case *value* is different from its default.</td></tr></table>&nbsp;
<a href="#maybeextensions-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />