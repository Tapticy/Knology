
# Bytes[] Array 
## Convert.ToBase64String() Method
```c#
byte[] bytes = {1, 2, 3, 4, 5, 6, 7};
Console.WriteLine(BitConverter.ToString(bytes));

string s = Convert.ToBase64String(bytes);
Console.WriteLine(s);

byte[] newBytes = Convert.FromBase64String(s);
Console.WriteLine(BitConverter.ToString(newBytes));
```
### Output to terminal
01-02-03-04-05-06-07
AQIDBAUGBw==
01-02-03-04-05-06-07


# GetUpperBound() Method
```c#
int[] arr = new int[5];
int value = 1;
for (int ctr = 0; ctr <= arr.GetUpperBound(0); ctr++)
{
    arr[ctr] = value;
    value = value * 2 + 1;
    Console.WriteLine(value);
    Console.WriteLine(arr[ctr]);
}
```
### Terminal
3
1
7
3
15
7
31
15
63
31