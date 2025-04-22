
```c#
 string customerName = "Ms. Barros";

 string currentProduct = "Magic Yield";
 int currentShares = 2975000;
 decimal currentReturn = 0.1275m;
 decimal currentProfit = 55000000.0m;

 string newProduct = "Glorious Future";
 decimal newReturn = 0.13125m;
 decimal newProfit = 63000000.0m;

 Console.WriteLine($"Dear {customerName},");
 Console.WriteLine($"As a customer of our {currentProduct} offering we are excited to tell you about a new financial product that would dramatically increase your return.\n");
 Console.WriteLine($"Currently, you own {currentShares:N} shares at a return of {currentReturn:P}.\n");
 Console.WriteLine($"Our new product, {newProduct} offers a return of {newReturn:P}.  Given your current volume, your potential profit would be {newProfit:C}.\n");

 Console.WriteLine("Here's a quick comparison:\n");

 string comparisonMessage = "";

 comparisonMessage = currentProduct.PadRight(20);
 comparisonMessage += String.Format("{0:P}", currentReturn).PadRight(10);
 comparisonMessage += String.Format("{0:C}", currentProfit).PadRight(20);

 comparisonMessage += "\n";
 comparisonMessage += newProduct.PadRight(20);
 comparisonMessage += String.Format("{0:P}", newReturn).PadRight(10);
 comparisonMessage += String.Format("{0:C}", newProfit).PadRight(20);

 Console.WriteLine(comparisonMessage);
```

#####
```c#
     void Clear() {
         string[] pallets = ["B14", "A11", "B12", "A13"];
         Console.WriteLine("");

         Array.Clear(pallets, 0, 2);
         Console.WriteLine($"Clearing 2 ... count: {pallets.Length}");
         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
         }
     }

     string[] pall = ["B14", "A11", "B12", "A13"];
     void Resize() {

         Console.WriteLine($"{pall[0]}");
         Array.Clear(pall, 1, 2);
         Console.WriteLine($" {pall[1]}");


     }
     
     void Remove() {
         string[] pallets = ["B14", "A11", "B12", "A13"];
         Console.WriteLine("");

         Array.Clear(pallets, 0, 2);
         Console.WriteLine($"Clearing 2 ... count: {pallets.Length}");
         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
         }

         Console.WriteLine("");
         Array.Resize(ref pallets, 6);
         Console.WriteLine($"Resizing 6 ... count: {pallets.Length}");

         pallets[4] = "C01";
         pallets[5] = "C02";

         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
         }
     }

     void Redo() {
         string[] pallets = ["B14", "A11", "B12", "A13"];
         Console.WriteLine("");

         Array.Clear(pallets, 0, 2);
         Console.WriteLine($"Clearing 2 ... count: {pallets.Length}");
         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
         }

         Console.WriteLine("");
         Array.Resize(ref pallets, 6);
         Console.WriteLine($"Resizing 6 ... count: {pallets.Length}");

         pallets[4] = "C01";
         pallets[5] = "C02";

         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
         }

         Console.WriteLine("");
         Array.Resize(ref pallets, 3);
         Console.WriteLine($"Resizing 3 ... count: {pallets.Length}");

         foreach (var pallet in pallets) {
             Console.WriteLine($"-- {pallet}");
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