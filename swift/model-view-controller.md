# Model View Contoller

Design paradigm require for iOS. Lets apply it to our concentrator app. Divide objects into three camps.

So the Storyboard is our view,  ViewController is our view, we need the Model.

File > New > New File

* Model
    + What you application is (but not how it is displayed)
* View
    + Your controller's minions
* Controller
    + How your model is presented to the user (UI logic)

## Elaboration

Here is a visual representaion of this.
![single mvc](https://github.com/gil-ryan/grs-ios-pub/blob/master/img/single-mvc.png)

MVC is all about managing the communications between camps. The Model and View should __never__ talk to each other, __ever__. Can the View speak to its Controller? It kind of has to, communication needs to be __blind__ and __structured__. The View sends the action when things happen in the UI. Sometimes the View needs to synchronize with the Controller.

The Controller sets itself as the View's delegate. Delagate methods use terminology like _will_, _should_, or _did_. The delegate is set via a protocol (i.e. it's "blind" to class). 

__Views do not own the data they display__. Why? It makes no sense to have a generic list view that displays a large amount of data. Controllers are almost always that data source (not Model). Controllers interpret/format Model information for the View.

Can the Model talk directly to the Controller? No. The Model is (should be) UI independent. So what if the Model has information to update or something? It uses a 'radio station' - like broadcast mechanism. Controller (or other Model) "tune in" to interesting stuff. These are known as notifications, or 'KVO'. A View might "tune in", but probably not to a Model's "station".

One MVC is generally used to controll one screen on the iPhone. Now combine MVC groups to make complicated programs. Maybe like a sub-MVC but you'd never have more than one iPhone screen using a single MVC.

### Multipl MVCs Working Together

Here is another visual.
![multiple MVC for iOS app](https://github.com/gil-ryan/grs-ios-pub/blob/master/img/multiple-mvc.png)

## Model

### File > New > New File

![Image of template files menu]()

#### Cocoa Touch Class

A subclass for Cocoa Touch UI

#### Swift File

Now __this__ is the blank model file we're looking for. We always name model files after the most important class that is inside the file. 



