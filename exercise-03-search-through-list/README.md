# Task
Create an application that can find the largest number in a list of integers.
Try to do this with both arrays and a more complex collection such as lists or dictionaries.

# Collections
Collections are a way of grouping data that are related and of the same type.

## Arrays
Arrays are the most basic form of collections. They are fixed in size, so you must specify how large the array is when you create it.
In many languages, you can declare an array by adding square brackets to the type

```
int[] numbers = new int[10]; // This is an empty array of integers
```

To select a member of an array, you use the following code:

```
int[] numbers = new int[10];
numbers[0] = 1 // First member of an array is member zero.
numbers[9] = 10 // The last member of an array is the array size - 1
```

You can also use integer variables to access the array
```
int[] die = new int[6] { 1, 2, 3, 4, 5, 6 } // This creates an array and populates it with the elements in the curly brackets
int i = 3;
int thirdElement = die[i];
```

You can also have 2D arrays
```
bool[,] minesweeperGrid = new bool[10,10]; // This is an empty grid for the game mine sweeper
minesweeperGrid[5,5] = true // This is a mine
```

## Lists
Lists are like arrays except they are not fixed length. You can grow and shrink a list to your needs;
```
var products = new List<string>();
products.Add("TVs"); // This will add a new element to the empty list
products.Add("Stereos"); // This will add a new element at the end of the list
products.AddRange(new List<string> { "CDs", "Computers"}) // This will add multiple members to the list

products.Remove("TVs"); // This will remove the matching element
products.RemoveA(0); // This will remove the first element of the list

products.ForEach(m => Console.WriteLine(m)); // This will print the elements left inthe list to console
```

## Dictionaries
A dictionary is a more complex collection that stores data against a key. This is known as a Key-Value pair.

```
var classScores = new Dictionary<string, int>();
classScores.Add("Alice", 83); // You add elements to the dictionary by specifying the key and then the value
classScores.Add("Bob", 78);
		
int bobsScore = classScores["Bob"]; // You access values in the dictionary by specifying the key in square brackets
```