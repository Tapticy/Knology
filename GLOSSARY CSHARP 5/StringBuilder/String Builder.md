# String Builder
## Methods:
Insert() Append() Replace() Remove() AppendFormat()
```c#
static void Main(string[] args) {
    StringBuilder CLR = new StringBuilder("Common Language Runtime");
    StringBuilder CTS = new StringBuilder("Common Type System");
    StringBuilder PFA = new StringBuilder("Perform File Operations");
    StringBuilder JIT = new StringBuilder("Just In Time");
    if (args.Length > 0) {
        CLR.Append(args[0]);
    }
    if (args.Length > 1) {
        CTS.Append(args[1]);
    }
    Console.WriteLine(CLR);
    Console.WriteLine(CTS);

    if (args.Length > 2) {
        PFA.Append(args[2]);
    }
    if (args.Length > 3) {
        JIT.Append(args[3]);
    }

    Console.WriteLine(PFA);
    Console.WriteLine(JIT);

    //if (args != null) {
    //    CLR.Replace("Common Language Runtime", "Just In Time");
    //}
    //Console.WriteLine(CLR);
    /*

    */
}
```