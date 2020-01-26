HelpText support localization starting version 2.6+ by adding  public Resource files which include all HelpText of the Option class. You can use VS IDE to build the resource files.

__Note__: The Resource file should be public.

 ## A step by Step tutorial for Help Localization:
 
 - In the design mode of the Visual Studio IDE right-click the Project node in the Solution Explorer tree and select Add >> New Item. Select the Resource File template and give it a name, for example `Resource`. It will be renamed as Resource.resx in the project.
 - Double click Resource.resx in the Solution Explorer tree.
 - Add a new entry for every helptext option in the option classs,e.g, for the next option:
 ```cs
 [Option('n', "lines",  
    //move to the resource file and name it:  HelpTextLines                  
     HelpText = "Lines to be printed from the beginning or end of the file."]) 
  uint? Lines { get; set; }

```
  Add an entry in the resource file:
  name: "HelpTextLines" 
  value: "Lines to be printed from the beginning or end of the file." 

- Repeat the previous step for all Properties of the Option class


- In the Solution Explorer, add a new Resource File and name it using the culture code for French, "Resource.fr-FR.resx".

- Double click "Resource.fr-FR.resx".

- Enter "Lignes à imprimer depuis le début ou la fin du fichier." for the "HelpTextLines" resource name.
- Complete the translation for all the English entries.

 See Sample of resource files  [here](https://github.com/commandlineparser/commandline/blob/master/demo/ReadText.LocalizedDemo/Properties/Resources.resx).
- Modify the option class by filling the property `ResourceType` with the type of the resource you created and HelpText property with the name of string in the resource file as given below:

```cs
//modify the option 
[Option('n', "lines",           
            HelpText = "HelpTextLines",  //name of the resource string in the resource file
            ResourceType = typeof(Properties.Resources))]  // type of the resource class
        uint? Lines { get; set; }

```
- __Optionally__, 
  - To localize the keywords "Required,Default" and the error messages, add the the string expressions of the class `SentenceBuilder` to the resource files.
  - You can add the class `LocalizableSentenceBuilder` to your project. It's localized and located [here](https://github.com/commandlineparser/commandline/blob/master/demo/ReadText.LocalizedDemo/LocalizableSentenceBuilder.cs)  

  - In the `Main` method, Set sentence builder to `LocalizableSentenceBuilder`:

      ```cs
        SentenceBuilder.Factory = () => new LocalizableSentenceBuilder();
      ```

A complete localized demo `ReadText.LocalizedDemo` is located [here](https://github.com/commandlineparser/commandline/tree/master/demo/ReadText.LocalizedDemo)


### Localized Sample output in culture Czech (cs)

<details>
  <summary>Click to expand!</summary>

```
ReadText.Demo 0.0.0.0
Copyright (C) 2020 author
POUZITI:
normální scénár:
  ReadText.LocalizedDemo.exe head file.bin
specifikace poctu byte:
  ReadText.LocalizedDemo.exe head --bytes 100 file.bin
potlacit sumár:
  ReadText.LocalizedDemo.exe head -q file.bin
precíst více rádek:
  ReadText.LocalizedDemo.exe head --lines 10 file.bin
  ReadText.LocalizedDemo.exe head --lines=10 file.bin

  -n, --lines            Povinné. (Default: 5) Pocet rádek zobrazenych od
                         zacátku nebo konce souboru.

  -c, --bytes            Pocet bytu zobrazenych od zacátku nebo konce souboru.

  -q, --quiet            Potlacit sumár.

  --help                 Zobrazit tuto nápovedu.

  --version              Zobrazit informaci o verzi.

  input file (pos. 0)    Povinné. Jméno vstupního souboru.
```

</details>

__Remarks__:

- To enable the culture in the Console Application,e.g cs, add the next lines at the beginning of the Main method:

```cs
  System.Threading.Thread.CurrentThread.CurrentCulture = new CultureInfo("cs", false);
  System.Threading.Thread.CurrentThread.CurrentUICulture = new CultureInfo("cs", false);
```

Resources:

Download a [localized demo example](resources/ReadText.LocalizedDemo.zip).
