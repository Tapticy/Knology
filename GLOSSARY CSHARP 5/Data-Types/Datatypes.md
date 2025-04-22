# Sbyte Short Int Long 
Unsigned types will write to the console.
```c#
Console.WriteLine("Signed integral types:");

Console.WriteLine($"sbyte  : {sbyte.MinValue} to {sbyte.MaxValue}");
Console.WriteLine($"short  : {short.MinValue} to {short.MaxValue}");
Console.WriteLine($"int    : {int.MinValue} to {int.MaxValue}");
Console.WriteLine($"long   : {long.MinValue} to {long.MaxValue}");
```
## Display In Terminal
Signed integral types:
sbyte  : -128 to 127
short  : -32768 to 32767
int    : -2147483648 to 2147483647
long   : -9223372036854775808 to 9223372036854775807


## Unsigned Types 
## Hole Numbers
```c#
Console.WriteLine("");
Console.WriteLine("Unsigned integral types:");

Console.WriteLine($"byte   : {byte.MinValue} to {byte.MaxValue}");
Console.WriteLine($"ushort : {ushort.MinValue} to {ushort.MaxValue}");
Console.WriteLine($"uint   : {uint.MinValue} to {uint.MaxValue}");
Console.WriteLine($"ulong  : {ulong.MinValue} to {ulong.MaxValue}");
```
# Displayed
Unsigned integral types:
byte   : 0 to 255
ushort : 0 to 65535
uint   : 0 to 4294967295
ulong  : 0 to 18446744073709551615

## ####################################### ##################

# Floating Point Types
Base 2 format `float` and `double`.
Base 10 format `decimal`.
```c#
Console.WriteLine("");
Console.WriteLine("Floating point types:");
Console.WriteLine($"float  : {float.MinValue} to {float.MaxValue} (with ~6-9 digits of precision)");
Console.WriteLine($"double : {double.MinValue} to {double.MaxValue} (with ~15-17 digits of precision)");
Console.WriteLine($"decimal: {decimal.MinValue} to {decimal.MaxValue} (with 28-29 digits of precision)");

```
# Display
Floating point types:
float  : -3.4028235E+38 to 3.4028235E+38 (with ~6-9 digits of precision)
double : -1.7976931348623157E+308 to 1.7976931348623157E+308 (with ~15-17 digits of precision)
decimal: -79228162514264337593543950335 to 79228162514264337593543950335 (with 28-29 digits of precision)



A value type variable stores its values directly in an area of storage called the stack. The stack is memory allocated to the code that is currently running on the CPU (also known as the stack frame, or activation frame). When the stack frame has finished executing, the values in the stack are removed.

A reference type variable stores its values in a separate memory region called the heap. The heap is a memory area that is shared across many applications running on the operating system at the same time. The .NET Runtime communicates with the operating system to determine what memory addresses are available, and requests an address where it can store the value. The .NET Runtime stores the value, and then returns the memory address to the variable. When your code uses the variable, the .NET Runtime seamlessly looks up the address stored in the variable, and retrieves the value that's stored there.


## Data Types To Stick With
### `int` `decimal` `bool` `string`

`"Hello World!"` Value types are stored in the stack

`data = new data[3];` or `int[] number = new int[3];`
The `new` operator that is a reference type is stored on the Heap memory address.

```c#
int[] data;
data = new data[3];
int[] number = new int[3];

string shortenedString = "Hello World!";
string other = shortenedString;
other = "Changed!";
Console.WriteLine(shortenedString);
Console.WriteLine(other);


int one = 1;
int two = one;
two = 2;

Console.WriteLine("--Value Types--");
Console.WriteLine($"one: {one}");
Console.WriteLine($"two: {two}");

```


```c#


```



```c#


```


```c#


```



```c#


```