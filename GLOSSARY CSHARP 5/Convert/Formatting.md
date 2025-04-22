# String Formatting 

# Composite Formatting 
### Use numbered placeholder within a string


Data types and variables of a given data type have built-in "helper methods" to make certain tasks easy.
The literal string "{0} {1}!" forms a template, parts of which are replaced at run time.
The token {0} is replaced by the first argument after the string template, in other words, the value of the variable first.
The token {1} is replaced by the second argument after the string template, in other words, the value of the variable second.
```c#
string first = "replacement";
string second = "instance";

string result = string.Format("{0} {1}", first, second);
Console.WriteLine(result);
```

```c#
string first = "replacement";
string second = "instance";

Console.WriteLine($"{first} {second}");
Console.WriteLine($"{first} {second}");
Console.WriteLine($"{ second} { first}");
```

# String Interpolation
Notice how adding the :C to the tokens inside of the curly braces formats the number as currency regardless of whether you use int or decimal.
```c#
decimal price = 123.45m;
int discount = 50;
Console.WriteLine($"Price: {price:C} (Save {discount:C})");
```


```c#

decimal price = 123.45m;
int discount = 50;
Console.WriteLine($"Price: {price:C} (Save {discount:C})");

 /*
  By default, the N numeric format specifier displays only two digits after the decimal point.

If you want to display more precision, you can do that by adding a number after the specifier. 
The following code will display four digits after the decimal point using the N4 specifier
*/

decimal measurement = 123456.78912m;
Console.WriteLine($"Measurement: {measurement:N} units");

decimal measure = 123456.78912m;
Console.WriteLine($"Measurement: {measure:N4} units");

/*
Formatting percentages
Use the P format specifier to format percentages and rounds 
to 2 decimal places. Add a number afterwards to control the 
number of values displayed after the decimal point.
*/

decimal taxes = .36495m;
Console.WriteLine($"Tax rate: {taxes:P2}");

        /*
         
         */
decimal cost = 67.55m;
decimal salePrice = 59.99m;

string yourDiscount = String.Format("You saved {0:C2} off the regular{1:C2} price. ", (cost - salePrice), cost);

Console.WriteLine(yourDiscount);
```


```c#
class Program
{
    public record Items(string CLR, int number);
    public record Select(string first,  string second);

    static void Main(string[] args) {

        Select sel = new Select("Jack", "Black");
           

        string result = string.Format("{0} {1}", sel.first, sel.second);
        Console.WriteLine(result);
    }
}
```

```c#
  static void Display() {
      decimal tax = .36785m;
      Console.WriteLine($"Tax rate: {tax:P2}");
  }

  static void Combin() {
      decimal price = 67.55m;
      decimal salePrice = 59.99m;

      string yourDiscount = String.Format("You saved {0:C2} off the regular {1:C2} price. ", (price - salePrice), price);

      Console.WriteLine(yourDiscount);
  }

  static void Invoice() {
      int invoiceNumber = 1201;
      decimal productShares = 25.4568m;
      decimal subtotal = 2750.00m;
      decimal taxPercentage = .15825m;
      decimal total = 3185.19m;

      Console.WriteLine($"Invoice Number: {invoiceNumber}");
      Console.WriteLine($"   Shares: {productShares:N3} Product");
      Console.WriteLine($"     Sub Total: {subtotal:C}");
      Console.WriteLine($"           Tax: {taxPercentage:P2}");
      Console.WriteLine($"     Total Billed: {total:C}");
  }
```

```c#
 static void Payee() {
       string paymentId = "769C";
       string payeeName = "Mr. Stephen Ortega";

       var formattedLine = paymentId.PadRight(6);
       formattedLine += payeeName.PadRight(24);

       Console.WriteLine(formattedLine);
   }

 static void Payment() {
       string paymentId = "769C";
       string payeeName = "Mr. Stephen Ortega";
       string paymentAmount = "$5,000.00";

       var formattedLine = paymentId.PadRight(6);
       formattedLine += payeeName.PadRight(24);
       formattedLine += paymentAmount.PadLeft(10);

       Console.WriteLine(formattedLine);
   }

   static void Formatted() {
       string paymentId = "769C";
       string payeeName = "Mr. Stephen Ortega";
       string paymentAmount = "$5,000.00";

       var formattedLine = paymentId.PadRight(6);
       formattedLine += payeeName.PadRight(24);
       formattedLine += paymentAmount.PadLeft(10);

       Console.WriteLine("1234567890123456789012345678901234567890");
       Console.WriteLine(formattedLine);
   }
```