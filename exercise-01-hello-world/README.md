# Setting up your Development Environment

This should help with setting up the development tools and getting used to using them for doing basic things.

## Software
First, make sure you have the following tools installed on your machine:

 - [Git for Windows](https://git-scm.com/download/win)
 - [Dotnet SDK](https://www.microsoft.com/net/download/thank-you/dotnet-sdk-2.1.402-windows-x64-installer)
 - [Visual Studio Code](https://code.visualstudio.com/)

There is no need to change anything away from the default options provided by the installer, except when you install visual code you may want to enable the 'open with code' options.

You can install these programs on your own hardware if you don't have access to install them on your own machine.

After installing the programs above, check that you can use them as expected. We will check that they are installed correctly using the command line.

You can check the install for each program by running the commands below:

`git` - for Git for Windows

`code` - for Visual studio code - this will open Visual studio code

`dotnet` - for the dotnet SDK.

## Code Repository

Follow steps 1 and 2 from this link to create a repository on github:

https://guides.github.com/activities/hello-world/

This will create a repository in your own github account. By default all repositories are public so we will be able to see your repositrory.

Once you have created the repository, get the clone url from github and run the commands below:

```
git clone [clone url] 
cd hello-world
code .
```

This will open Visual Studio Code inside your new repository.

Press `Ctrl+~` to open a console inside visual studio code.

Inside the console, enter these commands:
```
dotnet new console --name HelloWorld
cd HelloWorld
``` 

You should see a folder named HelloWorld appear in vscode's explorer view. There will be a file named Program.cs with the following content:

```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

In CSharp, code is grouped into .cs files. Each .cs file declares a **namespace**. You can declare as many namespaces as you want in a single .cs file, but best practice is to only declare one per file.

Each namespace can hold **classes**. Classes are where we write most of our code.

The line at the top of the file `using System;` imports the System namespace into our program. This means that any class that is defined in the System namespace can be used in our program.

In Program.cs, we declare a single namespace named **HelloWorld**. The HelloWorld namepsace contains a single class called **Program**. Inside the Program class, we have a single method named **Main**. When you run the program, the Main method will be executed. 

The Main method contains a single line:
```csharp
Console.WriteLine("Hello World!");
```

This uses the `Console` class from the `System` namespace. The `.Writeline("Hello World!");` part is called a method call. We can say we are calling the `WriteLine` method on the `Console` class, and passing the string argument `"Hello World!"`. Similarly, the system will call The `Main` method on our `Program` class when we execute our program, and the system will pass the `command line arguments` to our program inside the args variable.

You can run the program inside vscode like this:

```
dotnet run
```

You should see the `Hello World!` appear in the console.

# Reference Material
1. Read [Chapter 2](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository) of Pro Git (About 1 hour)

2. Follow this web-based [tutorial](https://docs.microsoft.com/en-us/dotnet/csharp/quick-starts/hello-world) about CSharp (About 1 hour)

# Challenges

After completing the above reference material you should be able to do this with a little bit of effort:

1. Change the program we created above so that it prints `"Hello <name>"` where name is passed on the command line.
Push your changes to github, and send us a link to your repo on teams so we can run your program.
