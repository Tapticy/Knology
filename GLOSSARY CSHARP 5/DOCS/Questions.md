# Questions:

What the difference between IDictionary - Dictionary
```c#
IDictionary dic = new Dictionary<string, string>()
{
    dic.Add("This", "That");
}

foreach (DictionaryEntry dis in dic)
{
    Console.WriteLine($"{dis.Key}: {dis.Value}");
}



{1, "Ports for devices outside the case"},
{2, "Provide electricity"},
{3, "Expansion cards"}


{1, "FireWire"},
{2, "eSATA"},
{3, "USB"}


Dictionary<int, string> some = new()
{
    { 1, "Ammeter" },
    { 2, "Anonymous" },
    { 3, "ANSI"}
};

foreach (KeyValuePair<int, string> in some)
{
    Console.WriteLine($"{some.Keys} and {some.Values}");
}
```

# Question: 
Why is the output 172 172
```c#
List<string> glo = ["ATAPI", "ATX", "ATX12V"];
foreach (var ary in glo)
{
    if (ary.StartsWith("ATX"))
    {
        Console.WriteLine(ary[1] + ary[2]);
    }
}
```