# Diagonal Difference

``` swift
func diagonalDifference(arr: [[Int]]) -> Int {
    var firstDiagonalSum = 0
    var secondDiagonalSum = 0
    
    for index in 0 ..< arr.count {
        firstDiagonalSum += arr[index][index]
        secondDiagonalSum += arr.reversed()[index][index]
    }
    
    return abs(firstDiagonalSum - secondDiagonalSum)
}
```
