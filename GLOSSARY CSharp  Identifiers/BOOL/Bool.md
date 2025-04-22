
# Bool Lean Array
```c#
bool[] check = { true, false };
Console.WriteLine(check[0] ? "Yes" : "No");
Console.WriteLine(check[1] ? "definition" : "No");
```

# Literals True False
### Initialize a bool variable
```c#
bool check = true;
Console.WriteLine(check ? "Yes" : "No");
Console.WriteLine(false ? "Yes" : "No");
```


# Logical Negation
`!` Computes logical negation 
Making a value `!passed` value true, and `!true` value false
```c#
bool passed = false;
Console.WriteLine(!passed);
Console.WriteLine(!true);
```



```c#
bool MatchYahoo()
{
    Console.WriteLine("All Numbers Match Yahoo");
    return true;
}

bool NoMatch()
{
    Console.WriteLine("Sorry no Match\n Numbers Only with 2 digits");
    return false;
}
```


This is checking for equality using built-in method
```c#
 Console.WriteLine("a" == "A");
 Console.WriteLine("v" == "V");
 Console.WriteLine("Enter yes to countinue");
 string? this_value = Console.ReadLine();
 Console.WriteLine(this_value == "yes" ? "yes" : "no");
```


# Contains() Method
```c#
int[] pick_Category = [2, 4, 5, 6, 7, 9, 10];
int[] pick_Numbers = [1, 2, 3, 4, 5, 6, 7, 8,
 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19,
20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30,
31, 32, 33, 34, 35, 36, 37, 38, 39, 40,
41, 42, 43, 44, 45, 46, 47, 49, 50, 51, 
52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 
62, 63, 64, 65, 66, 67, 68, 69, 70];

Console.WriteLine(pick_Category.Contains(3));
Console.WriteLine(pick_Numbers.Contains(70));
// ! is unary negation operator or Not operator
Console.WriteLine(pick_Category.Contains(10) == false);
Console.WriteLine(!pick_Numbers.Contains(16));


```


# Greater than less than
```c#
Console.WriteLine(pick_Category[2] < pick_Numbers[3]);
Console.WriteLine(pick_Category[1] < pick_Numbers[3]);
Console.WriteLine(pick_Category[4] >= pick_Numbers[6]);
Console.WriteLine(pick_Category[1] <= pick_Numbers[1]);
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