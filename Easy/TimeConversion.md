# Time Conversion

``` swift
func timeConversion(s: String) -> String {
    let dateFormatter = DateFormatter()
    dateFormatter.dateFormat = "hh:mm:ssa"

    let date = dateFormatter.date(from: s)
    dateFormatter.dateFormat = "HH:mm:ss"

    return dateFormatter.string(from: date ?? .now)
}
```
