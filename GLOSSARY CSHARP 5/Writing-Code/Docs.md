
 
# Array 
```c#
//01, 03, 04, 05, 15, 17, 21
 // 01, 07, 08, 17, 23, 37, 44
 int[] a = [01, 07, 08, 17, 23, 37, 44];
 Int32[] b = [01, 03, 04, 05, 15, 17, 21];
 Array.Sort(a, b);
 foreach (Int32 i in a) {
     Console.WriteLine(i);
 }
```


# IF Statement
```c#
string an = "PFA";
string[] arr = an.Split('-');
   
string JIT = "";
string PFA = "";
string CTS = "";
string CLR = "";

     

if (arr[0] == "JIT") {
    JIT = "Just In Time";
}
else if (arr[0] == "PFA") {
    PFA = "Perform File Operations";
}
else if (arr[0] == "CTS") {
    CTS = "Common Type System";
}
else if (arr[0] == "CLR") {
    CLR = "Common Language Runtime";
}
else {
    Console.WriteLine("Invalid");
}
Console.WriteLine($"{JIT}");
Console.WriteLine($"{PFA}");
Console.WriteLine($"{CTS}");
Console.WriteLine($"{CLR}");
```

## System.IndexOutOfRangeException:
 'Index was outside the bounds of the array
```c#
 string Abb = "";
 string[] letter = Abb.Split('-');

 string JIT; string PFA; string CTS; string CLR;

 if (letter[0] == "JIT") {
     JIT = "Just In Time";
 }
 //
 else if (letter[1] == "PFA") {
     PFA = "Perform File Operations";
 }
 else if (letter[2] == "CTS") {
     CTS = "Common Type System";
 }
 else {
     Console.WriteLine("Just Invalid");
 }
```


# Abbreviations

    CLR: Common Language Runtime
    CTS: Common Type System 
    PFA: Perform File Operations
    JIT: Just In Time


## Hardware and software terms
    EPS or .eps Encapsulated PostScript
    Encapsulated PostScript in digital marketing, which is a Vector Graphic this is made up of 
    curves and lines that joints together to create different geometric shapes. 
    
    API Application Programming Interface
    An API Application Programming Interface is a set of 
    protocols and tools that allow different software applications 
    to communicate with each other.



## Emojis
:smile: :100: :smiley: :blush:

