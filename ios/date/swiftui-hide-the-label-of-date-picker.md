# \[SwiftUI] Hide the label of Date Picker

* use `.labelsHidden()` to hide labels of Date Picker

```swift
DatePicker("", selection: $fromDate, displayedComponents: [.date])
  .datePickerStyle(.compact)
  .labelsHidden()
```
