# Ok(*TSuccess*, *TMessage*) Class
 

Represents the result of a successful computation.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;<a href="T_RailwaySharp_ErrorHandling_Result_2">RailwaySharp.ErrorHandling.Result</a>(*TSuccess*, *TMessage*)<br />&nbsp;&nbsp;&nbsp;&nbsp;RailwaySharp.ErrorHandling.Ok(TSuccess, TMessage)<br />
**Namespace:**&nbsp;<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal sealed class Ok<TSuccess, TMessage> : Result<TSuccess, TMessage>

```

**VB**<br />
``` VB
Friend NotInheritable Class Ok(Of TSuccess, TMessage)
	Inherits Result(Of TSuccess, TMessage)
```

**C++**<br />
``` C++
generic<typename TSuccess, typename TMessage>
internal ref class Ok sealed : public Result<TSuccess, TMessage>
```

**F#**<br />
``` F#
[<SealedAttribute>]
type Ok<'TSuccess, 'TMessage> =  
    class
        inherit Result<'TSuccess, 'TMessage>
    end
```


#### Type Parameters
&nbsp;<dl><dt>TSuccess</dt><dd>Type that models the result of a successful computation.</dd><dt>TMessage</dt><dd>Type that model a message related to a computation.</dd></dl>&nbsp;
The Ok(TSuccess, TMessage) type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_RailwaySharp_ErrorHandling_Ok_2__ctor">Ok(TSuccess, TMessage)</a></td><td>
Initializes a new instance of the Ok(TSuccess, TMessage) class</td></tr></table>&nbsp;
<a href="#ok(*tsuccess*,-*tmessage*)-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_RailwaySharp_ErrorHandling_Ok_2_Messages">Messages</a></td><td /></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_RailwaySharp_ErrorHandling_Ok_2_Success">Success</a></td><td /></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_RailwaySharp_ErrorHandling_Result_2_Tag">Tag</a></td><td> (Inherited from <a href="T_RailwaySharp_ErrorHandling_Result_2">Result(TSuccess, TMessage)</a>.)</td></tr></table>&nbsp;
<a href="#ok(*tsuccess*,-*tmessage*)-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_RailwaySharp_ErrorHandling_Result_2_ToString">ToString</a></td><td> (Inherited from <a href="T_RailwaySharp_ErrorHandling_Result_2">Result(TSuccess, TMessage)</a>.)</td></tr></table>&nbsp;
<a href="#ok(*tsuccess*,-*tmessage*)-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#ok(*tsuccess*,-*tmessage*)-class">Back to Top</a>

## See Also


#### Reference
<a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />