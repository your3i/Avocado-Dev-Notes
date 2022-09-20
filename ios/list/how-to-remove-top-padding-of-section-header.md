# How to remove top padding of section header

There's top padding on top of the section header from iOS 15.

The way to delete the padding is ...

```swift
if #available(iOS 15.0, *) {
    tableView.sectionHeaderTopPadding = 0.01 // *1
}
```

\*1: don't set the value to 0, because it will change the animation of top header changing.

see: [https://zenn.dev/your3i/articles/947f1df7ef7f91](https://zenn.dev/your3i/articles/947f1df7ef7f91)
