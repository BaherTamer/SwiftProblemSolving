# Mini-Max Sum

``` swift
func miniMaxSum(arr: [Int]) -> Void {
    if arr.allSatisfy({ $0 == arr.first }) {
        let sum = arr.dropFirst().reduce(0, +)
        
        print("\(sum) \(sum)")
    } else {
        var minSum = 0
        var maxSum = 0
        
        arr.forEach { number in
            let sum = arr.filter { $0 != number }.reduce(0, +)
            
            if sum > maxSum { maxSum = sum }
            if sum < minSum || minSum == 0 { minSum = sum }
        }
        
        print("\(minSum) \(maxSum)")
    }
}
```
