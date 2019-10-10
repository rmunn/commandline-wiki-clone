# Trial Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;RailwaySharp.ErrorHandling.Trial<br />
**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class Trial
```

**VB**<br />
``` VB
Friend NotInheritable Class Trial
```

**C++**<br />
``` C++
internal ref class Trial abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
type Trial =  class end
```

The Trial type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Apply__3">Apply(TValue, TSuccess, TMessage)</a></td><td>
If the wrapped function is a success and the given result is a success the function is applied on the value. Otherwise the exisiting error messages are propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Bind__3">Bind(TValue, TSuccess, TMessage)</a></td><td>
If the result is a Success it executes the given function on the value. Otherwise the exisiting failure is propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Collect__2">Collect(TSuccess, TMessage)</a></td><td>
Collects a sequence of Results and accumulates their values. If the sequence contains an error the error will be propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Either__3">Either(TSuccess, TMessage, TResult)</a></td><td>
Takes a Result and maps it with successFunc if it is a Success otherwise it maps it with failureFunc.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Fail__2">Fail(TSuccess, TMessage)</a></td><td>
Wraps a message in a Failure.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Failed__2">Failed(TSuccess, TMessage)</a></td><td>
Returns true if the result was not successful.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Flatten__2">Flatten(TSuccess, TMessage)</a></td><td>
Flattens a nested result given the Failure types are equal.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Lift__3">Lift(TValue, TSuccess, TMessage)</a></td><td>
Lifts a function into a Result container and applies it on the given result.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Lift2__4">Lift2(TSuccess, TMessage, TSuccess1, TMessage1)</a></td><td>
Promote a function to a monad/applicative, scanning the monadic/applicative arguments from left to right.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_MergeMessages__2">MergeMessages(TSuccess, TMessage)</a></td><td>
Appends the given messages with the messages in the given result.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Ok__2">Ok(TSuccess, TMessage)</a></td><td>
Wraps a value in a Success.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Pass__2">Pass(TSuccess, TMessage)</a></td><td>
Wraps a value in a Success.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_ReturnOrFail__2">ReturnOrFail(TSuccess, TMessage)</a></td><td>
If the given result is a Success the wrapped value will be returned. Otherwise the function throws an exception with Failure message of the result.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Trial_Warn__2">Warn(TSuccess, TMessage)</a></td><td>
Wraps a value in a Success and adds a message.</td></tr></table>&nbsp;
<a href="#trial-class">Back to Top</a>

## See Also


#### Reference
<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />