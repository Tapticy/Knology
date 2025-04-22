
# Methods 
All these method are built-into c# 
```c# 
Reverse();
ToCharArray();
WriteLine();
Split()
String()
Math() 
Max()
```

# Examples 
This counts any letters in a paragraph 

```c#
string str = "Like millions of other computer users, you have probably used your desktop or notebook computer to play games";
// convert the message into a char array
char[] charMessage = str.ToCharArray();
// Reverse the chars
Array.Reverse(charMessage);
int x = 0;
// count the o's
foreach (char i in charMessage) { if (i == 'o') { x++; } }
// convert it back to a string
string new_message = new String(charMessage);
// print it out
Console.WriteLine(new_message);
Console.WriteLine($"'o' appears {x} times.");
```


# Split() Method 
Only when i use Split(' ') i get 150
Without Split method i get 
```c#
string intro = """
Like millions of other computer users, you have probably used your 
desktop or notebook computer to play games, update your blog, write 
papers, or build spreadsheets. You can use all these applications without 
understanding exactly what goes on inside your computer case or notebook.
But if you are curious to learn more about personal computers, and if you 
want to graduate from simply being the end user of your computer to 
becoming the master of your machine, then this book is for you. 
It is written for anyone who wants to understand what is happening inside
the machine, in order to install new hardware, diagnose and solve hardware
problems, and make purchasing decisions and then install new hardware. 
The only assumption made here is that you are a computer user-that is, 
you can turn on your machine,load a software package, and use that software
to accomplish a task. No experience in electronics is assumed.
""";

// when i use Split(' ') i get 150 
int countWords = intro.Split(' ').Length;
Console.WriteLine(countWords);
```

## With out Split just use intro.Length i get 926 why ??
```c#
int countWords = intro.Length;
Console.WriteLine(countWords);
```


```c#
string intro = """
Like millions of other computer users, you have probably used your 
desktop or notebook computer to play games, update your blog, write 
papers, or build spreadsheets. You can use all these applications without 
understanding exactly what goes on inside your computer case or notebook.
""";

// With out Split just use intro.Length i get 926 why ??
int countWords = intro.Length;
Console.WriteLine(countWords);

foreach (string word in intro.Split())
{
    Console.WriteLine(word);
} 
```

# Math() Max() Method
Concat to method by use the `Math.Max()` together.
```c#
int firstValue = 80;
int secondValue = 6;
int largerValue;
largerValue = Math.Max(firstValue, secondValue);
Console.WriteLine(largerValue);
```

## Methods Type Casting
`Beep()` should here a beep sound.
Integer to a string using the `ToString()` method.
```c#
Console.Beep();
int numbers = 3935;
string text = Convert.ToString(numbers);
Console.WriteLine(text);
```


## Conversion Type Casting
Explicit Conversion `Convert()` and Integer 32 `ToInt32()`
```c#
double myDouble = 5.5;
int b = Convert.ToInt32(myDouble);
Console.WriteLine(b.GetType());
```

## GetType() 
`ToDouble()` Is a method that converts the value of the specified 32-bit signed integer to an equivalent double-precision floating-point number.
`GetType()` Is a method that returns the type of the object
```c#
int c = 349;
double doubleMe = Convert.ToDouble(c);
Console.WriteLine(doubleMe.GetType()); 
```


```c#

```


```c#

```


```c#

```