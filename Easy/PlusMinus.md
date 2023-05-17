# Plus Minus

``` swift
func plusMinus(arr: [Int]) -> Void {
    let positives = Double(arr.filter {$0 > 0}.count)
    let negatives = Double(arr.filter {$0 < 0}.count)
    let zeros = Double(arr.filter {$0 == 0}.count)
    let arrayCount = Double(arr.count)
    
    print("\(positives/arrayCount)\n\(negatives/arrayCount)\n\(zeros/arrayCount)")
}
```
