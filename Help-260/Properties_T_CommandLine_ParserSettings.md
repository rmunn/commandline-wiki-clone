# ParserSettings Properties
 

The <a href="T_CommandLine_ParserSettings">ParserSettings</a> type exposes the following members.


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
<a href="#parsersettings-properties">Back to Top</a>

## See Also


#### Reference
<a href="T_CommandLine_ParserSettings">ParserSettings Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />