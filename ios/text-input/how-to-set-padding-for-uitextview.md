# How to set padding for UITextView

use [textContainerInset](https://developer.apple.com/documentation/uikit/uitextview/1618619-textcontainerinset)

the default value is UIEdgeInsets(top: 8, left: 0, bottom: 8, right: 0)

so if you set top and bottom smaller than 8, the padding will be kind of unnatural.



```swift
let textView = UITextView()
textView.textContainerInset = UIEdgeInsets(top: 8, left: 8, bottom: 8, right: 8)
```
