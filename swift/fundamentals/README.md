# Fundamentals

Fundamentals will generally reside here until the topic is developed enough for its own section.

## Type Casting

Swift will never type cast for you and automatically convert and _int_ to a _signed int_ and the likes. You have to create and new thing and initalize that.

uint32 initializer, which is struct

> emoji[card.identifier] = emojiChoices.remove(at: randomIndex)

## Random Number Generator

```swift
let randomIndex = arc4random_uniform(<#T##__upper_bound: UInt32##UInt32#>)
```
    
This will generate a number between _0_ and whatever number you selection for _upper\_bound_, __excluding__ the upper bound selected.