# \[SwiftUI] Build a segmented control

* use Picker and set pickerStyle to `.segmented`

```swift
enum SegmentedControlType: String, CaseIterable, Identifiable {
    case menu1
    case menu2

    var id: Self { self }
}

struct SegmentedControl: View {

    @Binding var selected: SegmentedControlType
    
    var body: some View {
        Picker("title", selection: $selected) {
            Text("menu1").tag(LotteryType.menu1)
            Text("menu2").tag(LotteryType.menu2)
        }
        .pickerStyle(.segmented)
    }
}
```
