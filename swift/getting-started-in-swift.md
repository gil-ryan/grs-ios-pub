# Getting Started

Here are our introductory notes since our _swift.md_ file is more of a table of contents.

## Things to note

One counter-intuitive aspect of Swift, is that every method has arguments that must be called when calling the method.

Every argument has a name you include when calling the function.

```swift
import UIKit

class ViewController: UIViewController {

    @IBAction func touchCard(_ sender: UIButton) {
    }
    
```

Each argument has an 'inside' name and 'caller' name, or outside name. You can add a return to a method, just notice the following:

```swift
import UIKit

class ViewController: UIViewController {

    @IBAction func touchCard(_ sender: UIButton) -> Int{

    }
```

### Xcode tip

Xcode > Behavior > Edit Behavior

You can use the behaviors settings to make xcodes do things. For example, when it generates some output, you can show the debugger. A nice feature.
