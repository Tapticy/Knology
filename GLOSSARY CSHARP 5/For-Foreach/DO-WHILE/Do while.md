```c#
 do {
     Console.WriteLine(counting);
     ++counting;

 } while (counting < 10);
```


```c#
string CLR = "Common Language Runtime";
       
int counting = 1;
 
do {
    counting++;
    Console.WriteLine($"{CLR}");
} while (counting < 1);
Console.WriteLine($"This will run: {counting}");
```

```c#
  string PFA = "Perform File Operations";
  string CLR = "Common Language Runtime";
  int counting = 0;

  while (counting < 10) {
      counting++;
      Console.WriteLine($"{PFA} {counting}");
  }


  do {
      counting += 2;
      Console.WriteLine($"{CLR}");
  } while (counting < 5);
  Console.WriteLine($"This will run: {counting}");
```