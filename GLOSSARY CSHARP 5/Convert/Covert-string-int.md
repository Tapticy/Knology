
# ToString() 
When converting a string to int you use the `ToString()` Method
```c#
string word;
int num = 23;
word = num.ToString();
Console.WriteLine("string " + word);
```

# Casting Truncates
When casting truncates the value will be rounded down or up. 
```c#
int value = (int)1.999m; // casting truncates
Console.WriteLine(value);
// When casting truncates the value will be rounded down 
// or up. 
int value2 = Convert.ToInt32(1.599m);
Console.WriteLine(value2);

string num = "102";
int result = 0;
if (int.TryParse(num, out result)) {
    Console.WriteLine($"Measurement: {result}");
}
else {
    Console.WriteLine("Unable to report measurement");
}
Console.WriteLine($"Measurement (w/ offset): {50 + result}");


```



```c#
int[] drawn = new int[3];
drawn[0] = 3; drawn[1] = 2; drawn[2] = 7;

string[] accommodate = Array.ConvertAll(drawn, ele => ele.ToString());

Console.WriteLine(string.Join(" ", accommodate));
```



# Will Give An Error

```c#
int first = 2;
string second = "4";
int result = first + second;
Console.WriteLine($"{result}");
```

## Conversion Types 
The `ToInt32()` method is apart of the .Net Framework, where `To 
```c#
int first = 2;
string second = "4";
int result = Convert.ToInt32(second);
Console.WriteLine($"{result}{first}");
```


# Don't Lose Information
This term is called Widening Conversion:
`decimal myDecimal = myInt;`
Convert from a data type that holds less like an int, decimal types hold more so you don't loose information
```c#
int myInt = 3;
Console.WriteLine($"int: {myInt}");

decimal myDecimal = myInt;
Console.WriteLine($"decimal: {myDecimal}");
```


# Casting
Casting operator () surrounded data type
```c#
decimal myDecimal = 3.14m;
Console.WriteLine($"decimal: {myDecimal}");

// (int)
int myInt = (int)myDecimal;
Console.WriteLine($"int: {myInt}");
```

This int can be assigned inside the decimal
so the compiler dose the conversion work.
```c#
int drawn = 10;
Console.WriteLine($"{drawn}");


decimal picked = drawn;
Console.WriteLine($"{picked}");

// Perform a Cast
decimal total = 3.4m;
Console.WriteLine($"total: {total}");

// Casting Operator ()
int bingo = (int)total;
Console.WriteLine($"Bingo: {bingo}");
```

# Narrowing Conversion 
Decimal Max 79228162514264337593543950335
The float Max 3.4028235E+38

So here is call narrowing when a data type like decimal can hold more
than float which holds less data 
```c#
decimal num = 1.23495498m;
Console.WriteLine($"Decimal: {num}");

float numbers = (float)num;
Console.WriteLine($"Float:   {numbers}");
```

# Converting a int to a string
```c#
  int first = 5;
  int second = 7;
  string message = first.ToString() + second.ToString();
  Console.WriteLine(message);

  // Converting a string to a int
  string three = "5";
  string four = "7";
  int sum = int.Parse(three) + int.Parse(four);
  Console.WriteLine(sum);

  // Using Convert Class to convert string to Int32
  //using the ToInt32() method 
  //.Net Class Library is ToInt32() and C# is ToInt() 
  string value1 = "5";
  string value2 = "7";
  int result = Convert.ToInt32(value1) * Convert.ToInt32(value2);
  Console.WriteLine(result);
```

```c#
 int value1 = 11;
 decimal value2 = 6.2m;
 float value3 = 4.3f;

 int result1 = (int)value1 / (int)value2;
 decimal result2 = (decimal)value2 / (decimal)value3;
 float result3 = (float)value3 / (float)value1;
 
 // Your code here to set result1
 // Hint: You need to round the result to nearest integer (don't just truncate)
 Console.WriteLine($"Divide value1 by value2, display the result as an int: {result1}");

 // Your code here to set result2
 Console.WriteLine($"Divide value2 by value3, display the result as a decimal: {result2}");

 // Your code here to set result3
 Console.WriteLine($"Divide value3 by value1, display the result as a float: {result3}");
```

Your goal was to use several different techniques to change the data type of a given value.

You used implicit conversion, relying on the C# compiler to perform widening conversions. When the compiler was unable to perform an implicit conversion, you used explicit conversions. You used the ToString() method to explicitly convert a numeric data type into a string.

When you needed to perform narrowing conversions, you used several different techniques. You used the casting operator () when the conversion could be made safely and were willing to accept truncation of values after the decimal. And you used the Convert() method when you wanted to perform a conversion and use common rounding rules when performing a narrowing conversion.

Finally, you used the TryParse() methods when the conversion from a string to a numeric data type could potentially result in a data type conversion exception.

Without this wealth of options, it would be difficult to work in a typed programming language. Fortunately, this well executed system of types, conversion, and casting can be harnessed to build error free applications.

```c#
 string[] values = { "12.3", "45", "ABC", "11", "DEF" };

 decimal total = 0m;
 string message = "";

 foreach (var value in values) {
     decimal number; // stores the TryParse "out" value
     if (decimal.TryParse(value, out number)) {
         total += number;
     }
     else {
         message += value;
     }
 }
```

```c#
```

```c#
```

```c#
```

```c#
```

```c#
```

```c#
```


```c#
```

```c#
```

```c#
```


```c#
```


```c#
```

```c#
```

```c#
```


```c#
```


```c#
```

```c#
```

```c#
```


```c#
```


```c#
```

```c#
```

```c#
```