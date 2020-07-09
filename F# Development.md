CommandLineParser provides F# package `CommandLineParser.FSharp` published to [nuget](https://www.nuget.org/packages/CommandLineParser.FSharp/). To install, type the command:

```
PM> Install-Package CommandLineParser.FSharp
```

The package has a dependency on: `FSharp.Core`.

You can use all the features of c# package without limitation.

## F# tutorial step by step:
1- Declare the option class
  use OptionAttribute and ValueAttribute to annotate the properties of the class. Also you can define property as `option`.

```fs

type options = {
  [<Option('r', "read", Required = true, HelpText = "Input files.")>] files : string;
  [<Option(HelpText = "Prints all messages to standard output.")>] verbose : bool;
  [<Option(Default = "english", HelpText = "Content language.")>] language : string;  
  [<Value(0, MetaName="offset", HelpText = "File offset.")>] offset : int option;
}
```
2- handle Parser Success
```fs
let run (o : options)  =
    printfn "Parser success"
    printfn "files= %A verbose= %b language= %s offset= %i" o.files o.verbose o.language o.offset.Value
 ```   
3- Handle Parser Failure
```fs
let fail (e : IEnumerable<Error>)  =
    printfn "fail"
```  
4- Call Parser
```fs    
let main argv =
  printfn "Args= %A" argv
  let result = CommandLine.Parser.Default.ParseArguments<options>(argv)
  match result with
  | :? Parsed<options> as parsed -> run parsed.Value
  | :? NotParsed<options> as notParsed -> fail notParsed.Errors
```

 Complete Example:

  
<details>
  <summary>Click to expand!</summary>

```fs
type options = {
  [<Option('r', "read", Required = true, HelpText = "Input files.")>] files : string;
  [<Option(HelpText = "Prints all messages to standard output.")>] verbose : bool;
  [<Option(Default = "english", HelpText = "Content language.")>] language : string;  
  [<Value(0, MetaName="offset", HelpText = "File offset.")>] offset : int option;
}

let run (o : options)  =
    printfn "Parser success"
    printfn "files= %A verbose= %b language= %s offset= %i" 
      o.files o.verbose o.language o.offset.Value
    

let fail (e : IEnumerable<Error>)  =
    printfn "fail"
  
    
let main argv =
  printfn "Args= %A" argv
  let result = CommandLine.Parser.Default.ParseArguments<options>(argv)
  match result with
  | :? Parsed<options> as parsed -> run parsed.Value
  | :? NotParsed<options> as notParsed -> fail notParsed.Errors  

```

</details>

[<img src="media/tryit.png">](https://dotnetfiddle.net/MEeHMp)

Download a complete [demo](https://github.com/commandlineparser/commandline/blob/master/demo/fsharp-demo.fsx) from the Project Repository.
