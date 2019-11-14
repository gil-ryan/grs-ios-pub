# Model View Contoller

Design paradigm require for iOS. Lets apply it to our concentrator app. Divide objects into three camps.

* Model
    + What you application is (but not how it is displayed)
* View
    + Your controller's minions
* Controller
    + How your model is presented to the user (UI logic)

MVC is all about managing the communications between camps. The Model and View should __never__ talk to each other, __ever__. Can the View speak to its Controller? It kind of has to, communication needs to be __blind__ and __structured__. The View sends the action when things happen in the UI. Sometimes the View needs to synchronize with the Controller.

The Controller sets itself as the View's delegate. Delagate methods use terminology like _will_, _should_, or _did_. The delegate is set via a protocol (i.e. it's "blind" to class). 

__Views do not own the data they display__. Why? It makes no sense to have a generic list view that displays a large amount of data. Controllers are almost always that data source (not Model). Controllers interpret/format Model information for the View.