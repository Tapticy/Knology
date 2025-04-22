
# ENUM 
```c#
public enum Abbreviations {
    EPS,
    API,
    AGP,
    CDN,
}
static void Main(string[] args) {
    Abbreviations E = Abbreviations.EPS;
    string[] abb = { "\tEncapsulated PostScript", "\tApplication Programming Interface",
    "\tAccelerated Graphics Port", "\tContent Delivery Network"};

    var total = (Abbreviations.EPS + abb[0]);
    
}
```

