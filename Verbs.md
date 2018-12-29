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

In this scenario the parser supplies you an additional `help` verb that allows:

```
C:\> app help clone
```

In this way application users can display specific verb command help screen.

```
C:\> app help
```

Or will display a help screen for available verbs.