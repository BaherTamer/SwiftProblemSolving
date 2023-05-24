# Birthday Cake Candles

``` swift
func birthdayCakeCandles(candles: [Int]) -> Int {
    let max = candles.max()
    return candles.filter{ $0 == max }.count
}
```
