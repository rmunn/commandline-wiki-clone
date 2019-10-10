# NameInfo Class
 

Models name information, used in <a href="T_CommandLine_Error">Error</a> instances.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.NameInfo<br />
**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public sealed class NameInfo : IEquatable<NameInfo>
```

**VB**<br />
``` VB
Public NotInheritable Class NameInfo
	Implements IEquatable(Of NameInfo)
```

**C++**<br />
``` C++
public ref class NameInfo sealed : IEquatable<NameInfo^>
```

**F#**<br />
``` F#
[<SealedAttribute>]
type NameInfo =  
    class
        interface IEquatable<NameInfo>
    end
```

The NameInfo type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_NameInfo__cctor">NameInfo</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_NameInfo__ctor">NameInfo</a></td><td>
Initializes a new instance of the NameInfo class</td></tr></table>&nbsp;
<a href="#nameinfo-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_NameInfo_LongName">LongName</a></td><td>
Gets the long name of the name information.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_NameInfo_NameText">NameText</a></td><td>
Gets a formatted text with unified name information.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_NameInfo_ShortName">ShortName</a></td><td>
Gets the short name of the name information.</td></tr></table>&nbsp;
<a href="#nameinfo-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NameInfo_Equals_1">Equals(Object)</a></td><td>
Determines whether the specified <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a> is equal to the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Object.Equals(Object)</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NameInfo_Equals">Equals(NameInfo)</a></td><td>
Returns a value that indicates whether the current instance and a specified NameInfo have the same value.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NameInfo_GetHashCode">GetHashCode</a></td><td>
Serves as a hash function for a particular type.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">Object.GetHashCode()</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#nameinfo-class">Back to Top</a>

## Fields
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public field](media/pubfield.gif "Public field")![Static member](media/static.gif "Static member")</td><td><a href="F_CommandLine_NameInfo_EmptyName">EmptyName</a></td><td>
Represents an empty name information. Used when <a href="T_CommandLine_Error">Error</a> are tied to values, rather than options.</td></tr></table>&nbsp;
<a href="#nameinfo-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#nameinfo-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine">CommandLine Namespace</a><br />