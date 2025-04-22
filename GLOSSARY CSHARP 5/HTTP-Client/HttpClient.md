
# Not complete
```c#
using System;
using System.IO;
using System.Net.Http;
using System.Net.Http.Headers;
using System.Threading.Tasks;


 private static readonly HttpClient _client = new HttpClient();
 static async Task Main() {
     Console.WriteLine("Enter Roll Number Student!");
     string rollNumber = Console.ReadLine();

     Console.WriteLine("Enter Student Name");
     string studentName = Console.ReadLine();

     Console.WriteLine("Enter Age");
     string studentAge = Console.ReadLine();

     Console.WriteLine("Enter path to Birth Certificate PDF");
     string pdfPath = Console.ReadLine();

     if (File.Exists(pdfPath)) {
         await UploadStudentData(rollNumber, studentName, studentAge, pdfPath);
     }
     else {
         Console.WriteLine("File Not found");
     }
 }

 private static async Task UploadStudentData(string rollName, string name, string age, string pdfPath) {
     using (var form = new MultipartFormDataContent()) {
         form.Add(new StringContent(rollName), "rollName");
         form.Add(new StringContent(name), "name");
         form.Add(new StringContent(age), "age");

         var pdfContent = new ByteArrayContent(await File.ReadAllBytesAsync(pdfPath));
         pdfContent.Headers.ContentType = MediaTypeHeaderValue.Parse("application/pdf");
         form.Add(pdfContent, "birthCertificate", Path.GetFileName(pdfPath));

         var respones = await _client.PostAsync("https://patapi.com/upload", form);
         
         if (respones.IsSuccessStatusCode) {
             Console.WriteLine("Student data uploaded");
         }
         else {
             Console.WriteLine($"Failed upload data: {respones.StatusCode}");
         }
     }
 }
```

```c#
```

```c#
```

```c#
```

```c#
```

```c#
```


```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```




```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```




```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```



```c#
```

```c#
```

```c#
```