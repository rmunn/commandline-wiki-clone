# Result Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;RailwaySharp.ErrorHandling.Result<br />
**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class Result
```

**VB**<br />
``` VB
Friend NotInheritable Class Result
```

**C++**<br />
``` C++
internal ref class Result abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
type Result =  class end
```

The Result type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_FailWith__2">FailWith(TSuccess, TMessage)(IEnumerable(TMessage))</a></td><td>
Creates a Failure result with the given messages.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_FailWith__2_1">FailWith(TSuccess, TMessage)(TMessage)</a></td><td>
Creates a Failure result with the given message.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_Succeed__2">Succeed(TSuccess, TMessage)(TSuccess)</a></td><td>
Creates a Success result with the given value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_Succeed__2_1">Succeed(TSuccess, TMessage)(TSuccess, IEnumerable(TMessage))</a></td><td>
Creates a Success result with the given value and the given messages.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_Succeed__2_2">Succeed(TSuccess, TMessage)(TSuccess, TMessage)</a></td><td>
Creates a Success result with the given value and the given message.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_Try__1">Try(TSuccess)</a></td><td>
Executes the given function on a given success or captures the failure.</td></tr></table>&nbsp;
<a href="#result-class">Back to Top</a>

## See Also


#### Reference
<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />