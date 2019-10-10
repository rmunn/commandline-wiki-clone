# SentenceBuilder Properties
 

The <a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder</a> type exposes the following members.


## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_ErrorsHeadingText">ErrorsHeadingText</a></td><td>
Gets a delegate that returns that errors block heading text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_SentenceBuilder_Factory">Factory</a></td><td>
Factory to allow custom SentenceBuilder injection</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_FormatError">FormatError</a></td><td>
Gets a delegate that handles singular error formatting. The delegates must accept an <a href="T_CommandLine_Error">Error</a> and returns a string.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_FormatMutuallyExclusiveSetErrors">FormatMutuallyExclusiveSetErrors</a></td><td>
Gets a delegate that handles mutually exclusive set errors formatting. The delegates must accept a sequence of <a href="T_CommandLine_MutuallyExclusiveSetError">MutuallyExclusiveSetError</a> and returns a string.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_HelpCommandText">HelpCommandText</a></td><td>
Get a delegate that returns the help text of help command. The delegates must accept a boolean that is equal 

#### Field Value
Type: <br />true for options; otherwise 

#### Field Value
Type: <br />false for verbs.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_RequiredWord">RequiredWord</a></td><td>
Gets a delegate that returns the word 'required'.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_UsageHeadingText">UsageHeadingText</a></td><td>
Gets a delegate that returns usage text block heading text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_VersionCommandText">VersionCommandText</a></td><td>
Get a delegate that returns the help text of vesion command. The delegates must accept a boolean that is equal 

#### Field Value
Type: <br />true for options; otherwise 

#### Field Value
Type: <br />false for verbs.</td></tr></table>&nbsp;
<a href="#sentencebuilder-properties">Back to Top</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_SentenceBuilder">SentenceBuilder Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />