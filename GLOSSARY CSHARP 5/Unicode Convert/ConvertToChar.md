
# Convert ToChar 
```c#
Random ran = new Random();
string[] order = new string[5];

for (int i = 0; i < order.Length; i++)
{
    int per = ran.Next(65, 70);
    string prefix = Convert.ToChar(per).ToString();
    string fix = ran.Next(1, 100).ToString("000");
    order[i] = prefix + fix;
}

foreach (var s in order)
{
    Console.WriteLine(s);
}
```