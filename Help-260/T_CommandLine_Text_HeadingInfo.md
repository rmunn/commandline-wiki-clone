# HeadingInfo Class
 

Models the heading part of an help text. You can assign it where you assign any <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.Text.HeadingInfo<br />
**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public class HeadingInfo
```

**VB**<br />
``` VB
Public Class HeadingInfo
```

**C++**<br />
``` C++
public ref class HeadingInfo
```

**F#**<br />
``` F#
type HeadingInfo =  class end
```

The HeadingInfo type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HeadingInfo__ctor">HeadingInfo</a></td><td>
Initializes a new instance of the HeadingInfo class specifying program name and version.</td></tr></table>&nbsp;
<a href="#headinginfo-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_HeadingInfo_Default">Default</a></td><td>
Gets the default heading instance. The title is retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblytitleattribute" target="_blank">AssemblyTitleAttribute</a>, or the assembly short name if its not defined. The version is retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblyinformationalversionattribute" target="_blank">AssemblyInformationalVersionAttribute</a>, or the assembly version if its not defined.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_HeadingInfo_Empty">Empty</a></td><td>
An empty object used for initialization.</td></tr></table>&nbsp;
<a href="#headinginfo-class">Back to Top</a>

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
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HeadingInfo_ToString">ToString</a></td><td>
Returns the heading as a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">Object.ToString()</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HeadingInfo_WriteError">WriteError</a></td><td>
Writes out a string and a new line using the program name specified in the constructor and *message* parameter to standard error stream.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HeadingInfo_WriteMessage">WriteMessage(String)</a></td><td>
Writes out a string and a new line using the program name specified in the constructor and *message* parameter to standard output stream.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HeadingInfo_WriteMessage_1">WriteMessage(String, TextWriter)</a></td><td>
Writes out a string and a new line using the program name specified in the constructor and *message* parameter.</td></tr></table>&nbsp;
<a href="#headinginfo-class">Back to Top</a>

## Operators
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public operator](media/puboperator.gif "Public operator")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HeadingInfo_op_Implicit">Implicit(HeadingInfo to String)</a></td><td>
Converts the heading to a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.</td></tr></table>&nbsp;
<a href="#headinginfo-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#headinginfo-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />