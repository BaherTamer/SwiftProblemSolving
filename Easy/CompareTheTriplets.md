# Compare the Triplets

``` swift
func compareTriplets(a: [Int], b: [Int]) -> [Int] {
    var scores: [Int] = [0, 0]
    
    for index in 0 ..< a.count {
        if a[index] > b[index] {
            scores[0] += 1
        } else if a[index] < b[index] {
            scores[1] += 1
        }
    }
    
    return scores
}
```
