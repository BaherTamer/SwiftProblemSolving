# Apples and Orange

``` swift
func countApplesAndOranges(s: Int, t: Int, a: Int, b: Int, apples: [Int], oranges: [Int]) -> Void {
    print("\(apples.filter {(s...t).contains($0 + a)}.count)\n\(oranges.filter {(s...t).contains($0 + b)}.count)")
}
```
