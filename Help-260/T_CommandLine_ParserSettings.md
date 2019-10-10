# ParserSettings Class
 

Provides settings for <a href="T_CommandLine_Parser">Parser</a>. Once consumed cannot be reused.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.ParserSettings<br />
**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public class ParserSettings : IDisposable
```

**VB**<br />
``` VB
Public Class ParserSettings
	Implements IDisposable
```

**C++**<br />
``` C++
public ref class ParserSettings : IDisposable
```

**F#**<br />
``` F#
type ParserSettings =  
    class
        interface IDisposable
    end
```

The ParserSettings type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_ParserSettings__ctor">ParserSettings</a></td><td>
Initializes a new instance of the ParserSettings class.</td></tr></table>&nbsp;
<a href="#parsersettings-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_AutoHelp">AutoHelp</a></td><td>
Gets or sets a value indicating whether implicit option or verb 'help' should be supported.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_AutoVersion">AutoVersion</a></td><td>
Gets or sets a value indicating whether implicit option or verb 'version' should be supported.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_CaseInsensitiveEnumValues">CaseInsensitiveEnumValues</a></td><td>
Gets or sets a value indicating whether perform case sensitive comparisons of <i>values</i>. Note that case insensitivity only applies to <i>values</i>, not the parameters.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_CaseSensitive">CaseSensitive</a></td><td>
Gets or sets a value indicating whether perform case sensitive comparisons. Note that case insensitivity only applies to <i>parameters</i>, not the values assigned to them (for example, enum parsing).</td></tr><tr><td>![Protected property](media/protproperty.gif "Protected property")</td><td><a href="P_CommandLine_ParserSettings_Consumed">Consumed</a></td><td /></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_EnableDashDash">EnableDashDash</a></td><td>
Gets or sets a value indicating whether enable double dash '--' syntax, that forces parsing of all subsequent tokens as values.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_HelpWriter">HelpWriter</a></td><td>
Gets or sets the <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a> used for help method output. Setting this property to null, will disable help screen.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_IgnoreUnknownArguments">IgnoreUnknownArguments</a></td><td>
Gets or sets a value indicating whether the parser shall move on to the next argument and ignore the given argument if it encounter an unknown arguments</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_MaximumDisplayWidth">MaximumDisplayWidth</a></td><td>
Gets or sets the maximum width of the display. This determines word wrap when displaying the text.</td></tr><tr><td>![Protected property](media/protproperty.gif "Protected property")</td><td><a href="P_CommandLine_ParserSettings_NameComparer">NameComparer</a></td><td /></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserSettings_ParsingCulture">ParsingCulture</a></td><td>
Gets or sets the culture used when parsing arguments to typed properties.</td></tr></table>&nbsp;
<a href="#parsersettings-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_ParserSettings_Dispose">Dispose()</a></td><td>
Frees resources owned by the instance.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_ParserSettings_Dispose_1">Dispose(Boolean)</a></td><td>
Releases the unmanaged resources used by the ParserSettings and optionally releases the managed resources</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_ParserSettings_Finalize">Finalize</a></td><td>
Finalizes an instance of the ParserSettings class.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Object.Finalize()</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#parsersettings-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#parsersettings-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine">CommandLine Namespace</a><br />