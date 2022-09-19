# Make enum conform to Identifiable

```swift
enum Enum: String, Identifiable {
    case menu1
    case menu2

    var id: Self { self } // ? cannot understand
}
```
