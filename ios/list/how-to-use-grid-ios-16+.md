# How to use Grid (iOS 16+)

```swift
let rowCount =  count / rowSize + (count % rowSize == 0 ? 0 : 1)

Grid {
    ForEach(0..<rowCount, id: \.self) { row in
        GridRow {
            ForEach(0..<rowSize, id: \.self) { col in
                let n = row * rowSize + col
                if n < count {
                    Text(String(n))
                }
            }
        }
    }
}
```
