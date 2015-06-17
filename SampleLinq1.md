## Restriction Operators: Where - Simple 1 ##

This sample uses where to find all elements of an array less than 5.

### Code ###

```
public void Linq1() {
    int[] numbers = { 5, 4, 1, 3, 9, 8, 6, 7, 2, 0 };

    var lowNums =
        from n in numbers
        where n < 5
        select n;

    Console.WriteLine("Numbers < 5:");
    foreach (var x in lowNums) {
        Console.WriteLine(x);
    }
}

```

### Output ###

```
Numbers < 5:
4
1
3
2
0
```