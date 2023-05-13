# Simple Array Sum

``` swift
func simpleArraySum(ar: [Int]) -> Int {
    (ar.count > 0 && ar.count <= 1000) ? ar.reduce(0, +) : 0
}
```
