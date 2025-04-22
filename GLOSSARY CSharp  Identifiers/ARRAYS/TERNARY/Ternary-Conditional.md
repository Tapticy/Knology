```c#
string item(double tem) => tem > 20.0 ? "Warm" : "Hot";

void One(double tem) {
    if (tem < 20.0) {
        Console.WriteLine("Cold");
    }
    else {
        Console.WriteLine("Hot");
        Console.WriteLine(item(30.00));
    }
}
One(40);
```