# Task
Create a console app that can print a right angle triangle using loops and if statements.
e.g.
```
*
**
***
****
*****
```

# Variables
Variables are a way of storing information for later use.
e.g. Storing the output of a function. Storing the input data for a function.
[Click here for more detail](https://www.tutorialspoint.com/csharp/csharp_variables.htm)


# If Statements
An if statement is used to control the flow in a program.
A statement must be true or false. If the statement is true it will execude the code within the if statement. If the statement is false it will skip the statement.

```
if(2 + 2 == 4)
{
    Print("This is true")
}
```

# Else statement
If you want some code that only executes if a statement is false, you can follow an if statement with an else statement
```
var input = Math.Random()
if(input % 2 == 0) // If the random number is even
{
    Print("This number is even")
}
else
{
    Print("This number is odd")
}
```

# Loops
A loop is a piece of code that keeps executing until an if statement reaches true.
There are many types of loops. Most languages have 3:

While
```
var number = 0
while(number < 10)
{
    Print("Still not 10")
    number = number + 1
}
```

Do while
```
var number = 0;
do
{
    Print("Still not 10")
    number = number + 1
} while()
```

For
```
for(var number = 0; number < 10; number++)
{
    Print("Still not 10")
}
```

[More Info](https://www.tutorialspoint.com/csharp/csharp_loops.htm)