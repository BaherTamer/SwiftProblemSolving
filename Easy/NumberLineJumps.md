# Number Line Jumps

``` swift
func kangaroo(x1: Int, v1: Int, x2: Int, v2: Int) -> String {
    // (2 - 1 = 1) % (1 - 2 = -1) = 0
    // (0 - 5 = -5) % (2 - 3 = -1) != 0
    v2 < v1 && ((x1 - x2) % (v1 - v2) == 0 && (v2 < v1)) == true ? "YES" : "NO"
}
```
