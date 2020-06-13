Verbs help delineate and separate options and values for multiple commands within a single app.  

A common usage of verbs in a sample ftp program could be to provide a specific commands: upload, download, delete, etc.  

A well known example of using verbs is the git version control system with multiple verbs: add, commit, push, pull, merge, etc.

To use verb commands create an option class for each verb decorated with the `[Verb]` attribute:

```csharp
[Verb("add", HelpText = "Add file contents to the index.")]
class AddOptions { //normal options here
}
[Verb("commit", HelpText = "Record changes to the repository.")]
class CommitOptions { //normal options here
}
[Verb("clone", HelpText = "Clone a repository into a new directory.")]
class CloneOptions { //normal options here
}
```

A this point you have to use a proper `ParserArguments<T1, T2...>` overload that accepts more than one type (without using the overload with variadic arguments, the library defines versions with up to 16 type parameters):

```csharp
static int Main(string[] args) {
    var result = Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args);
}
```

In this case the `T Value` property of `ParserResult<T>` will be `object` but will contain the proper instance if parsing succeeds or `NullInstance` if fails.

The only change with normal parsing is the requirement to query the `Parsed<object>.Value` property and invoke the application logic written to handle a specific verb.

A helper extension method is provided to simplify this task:

```csharp
static int Main(string[] args) {
    Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args)
    .WithParsed<AddOptions>(opts => ...)
    .WithParsed<CommitOptions>(opts => ...)
    .WithParsed<CloneOptions>(opts => ...)
    .WithNotParsed(errs => ...)
}
```

Coherently with `ParseArguments<T1, T2, ...>()` overloads used for verbs, you can take advantage also of `MapResult<T1, T2, ...>()`. Like in the sample with a single target instance, here we turn the parsed verb into an exit code:

```csharp
static int Main(string[] args) {
  return Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args)
    .MapResult(
      (AddOptions opts) => RunAddAndReturnExitCode(opts),
      (CommitOptions opts) => RunCommitAndReturnExitCode(opts),
      (CloneOptions opts) => RunCloneAndReturnExitCode(opts),
      errs => 1);
}
```

##Display help for verb##

Example: Display a help screen for all available verbs.

```sh
$ app --help
```
Example: Display the help screen for `clone` verb.

```sh
#the official syntax to call help for a verb: <VerbName> --help
$ app clone --help
```
***Remark***

In case of using one verb, you can use `object' as a second verb (dummy verb) as given below:


```cs
//use object as a dummy verb
Parser.Default.ParseArguments<Options,object> (args)
```
At least two verbs are needed.

**Using Verbs as Array of Types**

You can pass array of verb types to the parser.
 The overload method `ParseArguments` has Type as an array Type[]:

```cs
public ParserResult<object> ParseArguments(IEnumerable<string> args, params Type[] types)
```
This overload method is valuable when implementing the verbs as a plugin.
You collect the verbs using a **plugin** loader or **Ioc container** like Autofac or any DI container.

***Example***

```cs
static void Main1(string[] args)
{
    //Type[] types = { typeof(AddOptions), typeof(CommitOptions), typeof(CloneOptions) };
    //or collect types using reflection /plugins /Ioc container
  var types = LoadVerbs();			

  Parser.Default.ParseArguments(args, types)
        .WithParsed(Run)
        .WithNotParsed(HandleErrors);
}

//load all types using Reflection
private	static Type[] LoadVerbs()
{
  return Assembly.GetExecutingAssembly().GetTypes()
	  .Where(t => t.GetCustomAttribute<VerbAttribute>() != null).ToArray();		 
}

private static void Run(object obj)
{
  switch (obj)
  {
    case CloneOptions c:
          //process CloneOptions
        break;
    case CommitOptions o:
          //process CommitOptions
        break;
    case AddOptions a:
          //process AddOptions
        break;
  }
}

```

[<img src="media/tryit.png">](https://dotnetfiddle.net/stVEDu)

**Remark**

The generic overload method:  ```ParseArguments(string[] args, Type[] types)``` support more than 16 verbs.

The overload method ```ParseArguments<T1,..,T16>(string[] args)``` support only 16 verbs.
