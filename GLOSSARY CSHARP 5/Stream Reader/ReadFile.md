
# IO
Just Writes to a text file 2 line 
```c#
using System.IO;

try
{
    StreamWriter saveText = new StreamWriter("storage.txt");

    saveText.WriteLine("Do this work");
    saveText.WriteLine("Second line of text");
    saveText.Close();
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
finally
{
    Console.WriteLine("End of the line");
}
```



```c#
using System.IO;
using System.Text;

TextReader reader = new StreamReader(File.OpenRead("store.txt"));
Console.WriteLine(reader.ToString());
```







```c#

```



```c#

```



```c#

```



```c#

```