```c#
const string Greeting = "Hello";
const double MinLimit = -10.0, MaxLimit = -MinLimit;
```

```c#
using System;
namespace DefinitionsSection
{
    class Words
    {
        private string _ammeter;
        private string _ampere;
    }

    struct YourCount
    {
        public int NumberOfWords { get; set; }
    }

    interface IYourInterface
    {
        
    }

    delegate int YourDelegate();

    enum YourEnum
    {
    }

    namespace YourNestedNamespace
    {
        struct YourStruct
        {
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            //Your program starts here...
            Console.WriteLine("Hello world!");
        }
    }
}
```