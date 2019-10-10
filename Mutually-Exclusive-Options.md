You can define options as belonging to a set (group) that is mutually exclusive between groups. It means that you can run commands of one set at a time.
You can't mix commands of more than one set otherwise you get an error.
Mutually Exclusive is available by default. 

> NOTE: Mutually Exclusive Options in V 2.x are  different than V 1.x and the Parser option `MutuallyExclusive` is removed. Also `MutuallyExclusiveSet` property is changed to `SetName`.

Consider an application that can act as either a web or ftp server, but not both at the same time.

Group options in different set by defining the options class as follows:

```csharp

	class OptionsMutuallyExclusive
	{
	  //define commands in set(group) named web
	  [Option(SetName = "web")]
	  public string DocumentRoot { get; set; }
	   [Option(SetName  = "web")]
	  public bool EnableJavaScript { get; set; } 
	  
	  //define other commands in set(group) named ftp
	  [Option(SetName  = "ftp")]
	  public string FtpDirectory { get; set; } 
	  [Option(SetName  = "ftp")]
	  public bool AnonymousLogin { get; set; }
	  
	 
	  //Common: the next option can be used with any set because it's not included in a set
	  [Option('r')]
	  public string UrlAddress { get; set; }
	}
```

[Try it](https://dotnetfiddle.net/MkfPKX)

In this way if you combine an ftp option with a web one, parsing will fail. Options in the SAME set can be combined together, but options cannot be combined across sets. For example, options in the ftp set can be combined, but when options from the web and ftp sets are used together, an incompatible options error is produced.


Follows behavior in the terminal.

      ;; permitted, only commands in setname web is used.
      $ app --enablejavascript --documentroot ~/var/local/website -r http://localhost

     ;; denied; both web and ftp setnam are mixed
     $ app --anonymouslogin --enablejavascript
     ;;Raise ERROR: Option: 'enablejavascript' is not compatible with: 'anonymouslogin'.
    

**Best practice**

1- If you have various sets and each set contains a good number of options, It's better to structure your application with [[Verbs]] Commands.

2- You can distinguish between multiple sets at an interface level.


```csharp

	//define commands in set 'web'
	interface IWebOptions
    {
       
      [Option(SetName = "web")]
      string DocumentRoot { get; set; }
     [Option(SetName  = "web")]
      bool EnableJavaScript { get; set; } 
    }

	//define commands in set 'ftp'
	interface IFtpOptions
    {

	  [Option(SetName  = "ftp")]
	  string FtpDirectory { get; set; } 
	  [Option(SetName  = "ftp")]
	  bool AnonymousLogin { get; set; }
    }

	public class OptionsMutuallyExclusive : IWebOptions, IFtpOptions
	{  
	  //Implement commands in set(group) named web	
	  public string DocumentRoot { get; set; }	  
	  public bool EnableJavaScript { get; set; } 
	  
	  //Implement other commands in set(group) named ftp	
	  public string FtpDirectory { get; set; } 	 
	  public bool AnonymousLogin { get; set; }

	  //Common option, can be used with any set because it's not included in a set
	  [Option('r')]
	  public string UrlAddress { get; set; }
	}
```

[Try it](https://dotnetfiddle.net/OkEgxC)

**Migration of MutuallyExclusive options from v1.9.x guideline**

 A demo in v1.9.71 , like this [demo](https://dotnetfiddle.net/OkEgxC), 
can be  converted to v2.x as given below:

- Remove the Parser configuration `(MutuallyExclusive = true)`, it's not available and Mutually Exclusive Options are available by default.
- Rename `MutuallyExclusiveSet`  property to `SetName`.
- Re-arrange (group) the options in the sets in such a way that every set is complete set.
-  For common options in all sets, remove setname.



