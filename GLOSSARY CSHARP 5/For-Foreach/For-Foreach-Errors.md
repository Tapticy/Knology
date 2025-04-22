
# Argument Exception Error 
### This is for Error handling 
System.ArgumentException: 'Offset and length were out of bounds for the array or count is greater than the number of elements from index to the end of the source collection.' `Array.Sort(nine, shorts);`

```c#
  int[] nine = { 01, 07, 08, 17, 23, 37, 44 };
  Int16[] shorts = { 03, 04, 15, 34, 12 };
  Array.Sort(nine, shorts);

  foreach (int n in nine) {
      Console.WriteLine($"{n}\n");
  }

  if (nine.Length > 0) {
      Array.Clear(shorts, 0, nine.Length);
  }

  foreach (int n in nine) {
      Console.Write($"{n}");
  }
```




##### ########################
# Error
Unhandled exception. System.IndexOutOfRangeException: Index was outside the bounds of the array. at Program.<Main>$(String[] args) 
`if ((userNumber == 3) && (userNumber == draw1[i]))` Find out why?

Because this `draw1` array is out of bounds: 
`for (int i = 1; i < draw1.Length; i++)`
# Unhandled exception 
```c#

for (int i = 1; i < 101; i++)
{
    int userNumber = 3;
    if ((userNumber == 3) && (userNumber == draw1[i]))
    {
        Console.WriteLine($"{i} - {userNumber} FizzBuzz");
    }
    else if (i % 3 == 0)
    {
        Console.WriteLine($"{i} i Fizz");
    }
    else if (i % 5 == 0)
    {
        Console.WriteLine($"{i} i Buzz");
    }
    else
    {
        Console.WriteLine($"{i}");
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