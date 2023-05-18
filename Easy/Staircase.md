# Staircase

``` swift
func staircase(n: Int) -> Void {
    for i in 1...n {
        print(String(repeating: " ", count: n - i) + String(repeating: "#", count: i))
    }
}
```
