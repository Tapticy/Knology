
```c#
int[] draw1 = [06, 28, 33, 45, 48];
int[] draw2 = [02, 05, 32, 43, 48];
int[] draw3 = [05, 23, 26, 27, 37];

int[] winNumbers = [10, 16, 29, 37, 40];

// strings
string draw1 = "06, 28, 33, 45, 48";
string draw2 = "02, 05, 32, 43, 48";
string draw3 = "05, 23, 26, 27, 37";

string winNumbers = "10, 16, 29, 37, 40";
```



# For Daily Grand
```c#

int[] pick1 = new int[5];
int[] pick2 = new int[6];

int[] draw1 = [24, 43, 45, 47, 49];
int[] draw2 = [08, 22, 27, 36, 48];
int[] draw3 = [02, 06, 07, 17, 26];

int[] six49 = [10, 13, 24, 35, 38, 45];
int[] encore1 = [4424895];
int[] encore2 = [8079537];
string[] goldBall = ["46910369-01"];


foreach (var item in draw2) { }

foreach (var item in draw3) { }

foreach (var item in six49) { }
```


## Play Around Numbers
Using a `try{}` catch to loop through `draw2` array and 
write the number to a text file using `StreamWriter()`
```c#
int[] draw2 = [08, 22, 27, 36, 48];

try
{
    StreamWriter writer = new StreamWriter("storage.txt");

    foreach (var item in draw2)
    {
        writer.WriteLine(item);
    }
    Console.WriteLine("Item saved")
    writer.Close();
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
finally
{
    Console.WriteLine("End");
}
```


```c#
int[] pick1 = new int[5];
int[] pick2 = new int[6];

int[] draw1 = [24, 43, 45, 47, 49];
int[] draw2 = [08, 22, 27, 36, 48];
int[] draw3 = [02, 06, 07, 17, 26];

int[] six49 = [10, 13, 24, 35, 38, 45];
int[] encore1 = [4424895];
int[] encore2 = [8079537];
string[] goldBall = ["46910369-01"];

var randomRoll = new Random();
randomRoll.Shuffle(draw2);
randomRoll.Shuffle(draw3);
randomRoll.Shuffle(draw1);
```




# Picking Numbers Lotto
```c#
int[] row1 = [1, 8, 15, 22, 29, 36, 43];
int[] row2 = [2, 9, 16, 23, 30, 37, 44];
int[] row3 = [3, 10, 17, 24, 31, 38, 45];
int[] row4 = [4, 11, 18, 25, 32, 39];
int[] row5 = [5, 12, 19, 26, 34, 40];
int[] row6 = [6, 13, 20, 27, 35, 41];
int[] row7 = [7, 14, 21, 28, 36, 42];

int[] encore = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

        
var rand = new Random();
rand.Shuffle(row1);
foreach (int row in row1)
{
    Console.WriteLine(row);
}
```



```c#

int[] draw2 = [08, 22, 27, 36, 48];
for (int i = 0; i < draw2.Length; i++)
{
    if (draw2[i] == 48)
    {
        draw2[i] = 44;
    }
}

foreach (var draw in draw2)
{
    Console.WriteLine("" + draw);
}
```
 

```c#
string[] pick_Category = ["2", "4", "5", "6", "7", "9", "10"];
string[] pick_Numbers = ["1", "2", "3", "4", "5", "6", "7", "8",
 "9", "10", "11", "12", "13", "14", "15", "16", "17", "18", "19",
"20", "21", "22", "23", "24", "25", "26", "27", "28", "29", "30",
"31", "32", "33", "34", "35", "36", "37", "38", "39", "40",
"41", "42", "43", "44", "45", "46", "47", "49", "50", "51", "52",
"53", "54", "55", "56", "57", "58", "59", "60", "61", "62",
"63", "64", "65", "66", "67", "68", "69", "70"];
```

```c#
int[] pick_Category = [2, 4, 5, 6, 7, 9, 10];
int[] pick_Numbers = [1, 2, 3, 4, 5, 6, 7, 8,
 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19,
20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30,
31, 32, 33, 34, 35, 36, 37, 38, 39, 40,
41, 42, 43, 44, 45, 46, 47, 49, 50, 51, 
52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 
62, 63, 64, 65, 66, 67, 68, 69, 70];



foreach (var p in pick_Numbers)
{
    if (p != 4)
    {
        for (int i = 0; i < p; ++i)
        {
            Console.WriteLine($"{i}");
        }
    }
}
```

# Element 
```c#
List<int> ele = new() { 1, 2, 3, 4, 5, 6, 7, 8 };
foreach (int e in ele) {
    Console.WriteLine($"{e}");
}

Span<int> rator = [3, 45, 20, 02];
Span<string> test = ["jack", "peter", "paul"];
foreach (int r in rator) {
    Console.WriteLine(r);
}

foreach (var t in test) {
    Console.WriteLine(t);
}
```


```c#
// Get an array with the values of ConsoleColor enumeration members.
ConsoleColor[] colors = (ConsoleColor[])ConsoleColor.GetValues(typeof(ConsoleColor));

// Save the current background and foreground colors.
ConsoleColor currentBackground = Console.BackgroundColor;
ConsoleColor currentForeground = Console.ForegroundColor;

// Display all foreground colors except the one that matches the background.
Console.WriteLine("All the foreground colors except {0}, the background color:",
     currentBackground);
foreach (var color in colors) {
    if (color == currentBackground) continue;

    Console.ForegroundColor = color;
    Console.WriteLine("   The foreground color is {0}.", color);
}
Console.WriteLine();
// Restore the foreground color.
Console.ForegroundColor = currentForeground;

// Display each background color except the one that matches the current foreground color.
Console.WriteLine("All the background colors except {0}, the foreground color:",
                  currentForeground);
foreach (var color in colors) {
    if (color == currentForeground) continue;

    Console.BackgroundColor = color;
    Console.WriteLine("   The background color is {0}.", color);
}

// Restore the original console colors.
Console.ResetColor();
Console.WriteLine("\nOriginal colors restored...");
```