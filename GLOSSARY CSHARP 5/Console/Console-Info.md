
# Console Cancel Event
This can be used to calibrate keyboard keys that are pressed.
```c#
ConsoleKeyInfo cki;
Console.Clear();

Console.CancelKeyPress += new ConsoleCancelEventHandler(myHandler);

while (true) {
    Console.WriteLine("Press any key");
    Console.WriteLine("CLTRL+C to interrupt read operation:");

    // Start a console read operation
    cki = Console.ReadKey(true);

    Console.WriteLine($"  Key pressed: {cki.Key}\n");
    if (cki.Key == ConsoleKey.X) break;
}

protected static void myHandler(object sender, ConsoleCancelEventArgs args)
{
    Console.WriteLine("\nThe read operation has been interrupted");
    Console.WriteLine($" Key pressed: {args.SpecialKey}");
    Console.WriteLine($" Cancel property: {args.Cancel}");

    //
    Console.WriteLine("Setting the Cancel property true");
    args.Cancel = true;

    //
    Console.WriteLine($" Cancel properity: {args.Cancel}");
    Console.WriteLine("The read operation will resume");
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