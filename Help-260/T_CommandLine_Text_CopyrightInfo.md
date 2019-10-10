# CopyrightInfo Class
 

Models the copyright part of an help text. You can assign it where you assign any <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.Text.CopyrightInfo<br />
**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public class CopyrightInfo
```

**VB**<br />
``` VB
Public Class CopyrightInfo
```

**C++**<br />
``` C++
public ref class CopyrightInfo
```

**F#**<br />
``` F#
type CopyrightInfo =  class end
```

The CopyrightInfo type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_CopyrightInfo__ctor">CopyrightInfo()</a></td><td>
Initializes a new instance of the CopyrightInfo class.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_CopyrightInfo__ctor_2">CopyrightInfo(AssemblyCopyrightAttribute)</a></td><td>
Initializes a new instance of the CopyrightInfo class with an assembly attribute, this overrides all formatting.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_CopyrightInfo__ctor_3">CopyrightInfo(String, Int32)</a></td><td>
Initializes a new instance of the CopyrightInfo class specifying author and year.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_CopyrightInfo__ctor_4">CopyrightInfo(String, Int32[])</a></td><td>
Initializes a new instance of the CopyrightInfo class specifying author and copyrightYears.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_CopyrightInfo__ctor_1">CopyrightInfo(Boolean, String, Int32[])</a></td><td>
Initializes a new instance of the CopyrightInfo class specifying symbol case, author and copyrightYears.</td></tr></table>&nbsp;
<a href="#copyrightinfo-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected property](media/protproperty.gif "Protected property")</td><td><a href="P_CommandLine_Text_CopyrightInfo_CopyrightWord">CopyrightWord</a></td><td>
Gets a different copyright word when overridden in a derived class.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_CopyrightInfo_Default">Default</a></td><td>
Gets the default copyright information. Retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblycopyrightattribute" target="_blank">AssemblyCopyrightAttribute</a>, if it exists, otherwise it uses <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblycompanyattribute" target="_blank">AssemblyCompanyAttribute</a> as copyright holder with the current year. If neither exists it throws an <a href="https://docs.microsoft.com/dotnet/api/system.invalidoperationexception" target="_blank">InvalidOperationException</a>.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_CopyrightInfo_Empty">Empty</a></td><td>
An empty object used for initialization.</td></tr></table>&nbsp;
<a href="#copyrightinfo-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_CopyrightInfo_FormatYears">FormatYears</a></td><td>
When overridden in a derived class, allows to specify a new algorithm to render copyright copyrightYears as a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_CopyrightInfo_ToString">ToString</a></td><td>
Returns the copyright as a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">Object.ToString()</a>.)</td></tr></table>&nbsp;
<a href="#copyrightinfo-class">Back to Top</a>

## Operators
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public operator](media/puboperator.gif "Public operator")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_CopyrightInfo_op_Implicit">Implicit(CopyrightInfo to String)</a></td><td>
Converts the copyright instance to a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.</td></tr></table>&nbsp;
<a href="#copyrightinfo-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#copyrightinfo-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />