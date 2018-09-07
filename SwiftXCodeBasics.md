# CodePath/FastTrack iOS Development Program
# University of Arizona – Fall 2018

## The Basics of Swift + XCode

Please check out the [CodePath iOS Guides](https://guides.codepath.com/ios/) for plenty of amazing resources on how to use XCode and Swift. Please also refer to [Apple documentation](https://developer.apple.com/swift/resources/) for the Swift programming language. They have done a really good job.

## How do I start a new XCode project?

Please read the [following guide](https://guides.codepath.com/ios/New-Project) for extra support.

- Open XCode  and click on File > New Project. Click on Single View App: we will be doing exclusively Single View Apps for this class, but you are free to explore other types of apps on your own.

- Fill in all the project details and identifiers (e.g., project name, device, etc.). Make sure to name your project something does not conflict with another class or Swift library.

- Choose whether to initialize a git repository in your project's home folder. Another option is to just place your project's home folder in an existing git repository.

## What are the different elements of an XCode project?

- The main UI area is called storyboard and is located within the **Main.storyboard** file. The launch screen for the app is located with the **Launchscreen.storyboard** file. 

- Both the storyboard and launch screen are located with the **Base.lproj** folder.

- The media assets are located in the **Assets.xcassets** folder. The **AppiIcon.appiconset** is where you set the various app icons.

- The **<Project Name>Tests** and **<Project Name>UITests** folders contain all unit tests for the project. We will not be covering Unit Tests in this class, but we encourage you to explore those on your own.

- The **Pods** folder, **Podfile**, and **Podfile.lock** contain all the necessary information for manging external libraries that are incorporated into your project.

- The **Info.plist**, which stands for information property list, is written in XML, and contains metadata that help maintain  persistence and consistency across the app.

- The **<ProjectName>.xcodeproj** or **<ProjectName>.xcodeworkspace** are what you use to open up your project workspace in XCode.

## When creating a new class, what type of file should I choose?

– Every UI element in your storyboard should be created as a **CocoaTouchClass**. This includes ViewControllers, TableViews, TableViewCells, CollectionViews, CollectionViewCells, etc.

– The model and API elements should be created as a **Swift File**. These do not rely on user interactions, but instead serve to mediate data among the various UI and storyboard elements.

– If you accidentally delete your storyboard or launch screen, you can create a new **Storyboard** or **Launch Screen** file.

– For Unit Tests, create a **UI Test Case Class** or **Unit Test Case** class.
