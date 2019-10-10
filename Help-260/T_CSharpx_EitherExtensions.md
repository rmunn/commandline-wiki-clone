# EitherExtensions Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.EitherExtensions<br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class EitherExtensions
```

**VB**<br />
``` VB
<ExtensionAttribute>
Friend NotInheritable Class EitherExtensions
```

**C++**<br />
``` C++
[ExtensionAttribute]
internal ref class EitherExtensions abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
[<ExtensionAttribute>]
type EitherExtensions =  class end
```

The EitherExtensions type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_Bimap__4">Bimap(TLeft, TRight, TLeft1, TRight1)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_Bind__3">Bind(TLeft, TRight, TResult)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_IsLeft__2">IsLeft(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_IsRight__2">IsRight(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_Map__3">Map(TLeft, TRight, TResult)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_Match__2">Match(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EitherExtensions_ToEither__1">ToEither(TRight)</a></td><td>
Equivalent to monadic <a href="M_CSharpx_Either_Return__1">Return(TRight)(TRight)</a> operation. Builds a <a href="T_CSharpx_Right_2">Right(TLeft, TRight)</a> value in case *value* by default.</td></tr></table>&nbsp;
<a href="#eitherextensions-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />