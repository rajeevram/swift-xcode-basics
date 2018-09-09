Please refer to [the following guide](https://guides.codepath.com/ios/Swift-Basics) for common Swift functions, data types, classes, syntaxes, etc.

## What elements can I add to a ViewController backend?

- The most common elements are **IBOutlets** and **IBActions**. **Outlets** are uses to associate objects in the view with variables in their associated .swift file.

- **Actions** are event-handlers. That is, they are functions that are triggered whenever the user clicks on, enters, or otherwise interacts with that object in the view.

- It is common to add **static variables** to the backend of ViewControllers. This allows other views and classes to easily pass messages to the view via static, or class, reference.

- The **UserDefaults** class in Swift is used to preserve app data and configurations after it is closed or reset. Each UserDefaults instance operates similarly to a dictionary via storage and retrieval.

- Adding an event-handler through a **Tap Gesture Recognizer** allows you to change the state whenever the safe area of the view is tapped.

## What is a key-value compliant error and how do I fix it?

- This error indicated that you have a disconnected IBOutlet or IBAction. Probably, you deleted a variable or function without explicitly disconnecting it from the ViewController.

- Examine the **Connections Inspector** for each ViewController in the storyboard. Make sure to remove any connections that display a light switch instead of a filled circle.

- Another way to trigger a key-value compliant error is to name an IBOutlet the same as its parent class, i.e., UILabel label, UITextField textField, UIButton button.

## How can I trigger certain actions when the current view appears or disappears?

- There are 5 general methods that you can use to trigger states changes based on the view changing.

- **viewDidLoad()** is triggered when the view appears for the first time in your app, and anytime after you segue to it and it is not already on the navigation stack (e.g., modal segue).

- **viewWillAppear()** is triggered right before the view you are segueing to is about the appear; **viewDidAppear()** is triggered right after the view shows up.

- **viewWillDisappear()** is triggered right before the you are about to exit the current view; **viewDidDisappear()** is triggered right after the view is exited.

## What can I do to segue to a different view and back again?

- One type of segue is a **push** or **show segue**. This is most useful when your views are embedded in a **Navigation Controller**.

- A show segue in a Navigation Controller pushes the old view onto the navigation stack, and subsequently stacks the new view on top with a back button.

- A **modal segue** is usually used to interface among views that hold no relationship with each other; for example a login page would present modally to a home feed after authentication.

- Perform a model segue by giving the segue an **Identifier** in the **Attributes Inspector**. Then make the call **self. performSegue(withIdentifier: "myID", sender: nil)** within an event-handler.

- Embedding a two views within a **Tab Bar Controller** allows you to switch between them by pressing a particular tab at the bottom of the screen.

