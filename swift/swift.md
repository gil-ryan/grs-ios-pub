# Swift Based Applications

## How to build cool apps

* Consider this introductory to developing iOS applications on xcode
* The results will live in your pocket!
* Easy to distribute through AppStore
* Vibrant dev community

## What exactly is in iOS

### What goes into features like...

* Cocoa Touch
* Media
* Core Services
* Core OS

#### Cocoa Touch

UI Aspect

| Core technology | feature |
|:--:|:--:|
| Multi-touch | Alerts |
| Core Motion | Web view|
| View Hierarchy | Map Kit|
| Localization | Image Picker|
| Controls | Camera | 

#### Media

| Core technology | feature |
|:--:|:--:|
| Core audio | JPEG, PNG, TIFF|
| OpenAL | PDF|
| Audio Mixing | Quartz (2D)|
| Audio Recording | Core Animation|
| Video Playback | OpenGL ES

#### Core Services

These are on top of the lower level services below. 

| Core technology | feature |
|:--:|:--:|
| Collections | Core Location|
| Address Book | Net Services|
| Networking | Threading |
| File Access | Preferences |
| SQLite | URL Utilites

#### Core OS

We won't be touching upon these aspects in the repository.

| Core technology | feature |
|:--:|:--:|
| OSX Kernal| Power management | 
|Mach 3.0 | Keychain access|
|BSD | Certificates|
|Sockets | File System|
|Security | Bonjour|

### Platform Components

* Tools
* Language(s)
* Frameworks
* Design strategy

```swift
import UIKit

internal class ViewController : UIViewController {

    override internal func viewDidLoad()

    @IBAction internal func basic_method_init(_ sender: Any)
}
```