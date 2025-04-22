
```c#
DisplayCharacter('f'); // Output: A lowercase letter: f
DisplayCharacter('R'); // Output: An uppercase letter: R
DisplayCharacter('8'); // Output: A digit: 8
DisplayCharacter(','); // Output: Not alphanumeric character: ,

void DisplayCharacter(char ch)
{
    if (char.IsUpper(ch))
    {
        Console.WriteLine($"An uppercase letter: {ch}");
    }
    else if (char.IsLower(ch))
    {
        Console.WriteLine($"A lowercase letter: {ch}");
    }
    else if (char.IsDigit(ch))
    {
        Console.WriteLine($"A digit: {ch}");
    }
    else
    {
        Console.WriteLine($"Not alphanumeric character: {ch}");
    }
}
```


```c#

```

# Main Method
Main is where the code is run 
`Replace()` Replacing string `"jack"` with `"fok"`
```c#
using System;

class Program
{
    static void Main(string[] args)
    {
        string jack = "jack";
        jack = jack.Replace("jack", "fok");
        args = new string[] { "This", "That" };
        Console.WriteLine($"Main: {args.Length} or {jack}");
    }
}
```

# For loop Through
```c#
int[] frequencies = { 800, 1000, 1200 };
int[] durations = { 300, 300, 300 };

for (int i = 0; i < frequencies.Length; i++)
{
    Console.WriteLine(frequencies[i] + durations[i]);
}
```
## OR
```c#
int frequency = 1000; // Frequency in Hertz
int duration = 500;   // Duration in milliseconds
Console.Beep(frequency, duration);
```


# ToArray And ToCharArray Methods
These's 2 methods are similar to each other
```c#
string olderDrives = """ 
Most older hard drives, CD drives, and DVD drives use the parallel 
ATA (PATA) interface standard, also called the EIDE (Enhanced Integrated Drive Electronics)
standard, which can accommodate up to four EIDE or IDE devices on one system. 
Newer drives use the serial ATA (SATA) interface standard.
            """;

char[] lookIn = olderDrives.ToArray();
char[] lookUp = olderDrives.ToCharArray();

int countS = 0;

foreach (char l in lookIn)
{
    if (l == 's')
    {
        countS++;
    }
}
string total = new string(lookIn);
Console.WriteLine(total);
Console.WriteLine($"This many: {countS} s");

int countA = 0;
foreach (char see in lookUp)
{
    if (see == 'A' || see == 'a')
    {
        countA++;
    }
}

string tal = new string(lookUp);
Console.WriteLine(tal);
Console.WriteLine($"This Many: {countA} a's");
```


```c#
 string most = """
    The four most popular input/output devices are the mouse, keyboard, printer, 
    and monitor.
    """;

string inside = """ 
    The most important component inside the computer case is the motherboard, 
    also called the main board or system board.
    """;

string[] words = most.Split(" ");
foreach (var w in words)
{
    Console.WriteLine($"{w}");
}

for (int i = 0; i < inside.Length; i++)
{
    Console.WriteLine($"{i}");
}
```


# RegularExpressions And Regex() Method
```c#
using System.Text.RegularExpressions;

class Program : Texts
{
    static void Main(string[] args)
    {
        string text = """
             A computer requires both hardware and software to work. 
             The four basic functions of the microcomputer are input, 
             output, processing, and storage of data. 
             Data and instructions are stored in a computer in binary 
             form, which uses only two states for data on and off, or 1 
             and 0-which are called bits. Eight bits equal one byte. 
            """;
        string word = "microcomputer";

        bool match = Regex.IsMatch(text, word);
        Console.WriteLine(match);

    }
}
```



```c#
```