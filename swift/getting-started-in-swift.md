# Getting Started

Here are our introductory notes since our _swift.md_ file is more of a table of contents. These notes may be all over the place until I get a better grasp on Swift.

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

## Make a function

```swift
    func flipCard(withEmoji emoji: String, onButton: UIButton){
        
    }
```

It may seem odd at first, but this design is to make calling functions easier.
|: Purpose :|: Name :|
|:-:|:-:|
|: Function name :|: __flipCard__:|
|: External name:|: withEmoji:|
|: Inside argument with type string:|: emoji :| 

* Actions creates a method (function)
* Outlets create an instance variable (property)

```swift
var flipCount: int = 0
```

### Property Observer


### Xcode tips

Xcode > Behavior > Edit Behavior

You can use the behaviors settings to make xcodes do things. For example, when it generates some output, you can show the debugger. A nice feature.

Instance variables are called properties

#### Swift and types

You must be very specific about what types, Swift is a __strongly__ typed language. It will (if it can), decide the type for you.

### Warnings & Error

Red errors won't even compile or run.
Yellowing warnings will compile, but must be rectified, as they are usually are bad indication.

#### Common Warnings

* Initializers
* Variable 'cardNumber' was never mutated; consider changing to 'let' constant

#### Common Errors
