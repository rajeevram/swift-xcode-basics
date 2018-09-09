## How do I start a new XCode project?

Please read the [following guide](https://guides.codepath.com/ios/New-Project) for extra support.

- Open XCode and click on File > New Project. Click on Single View App: we will be doing exclusively Single View Apps for this class, but you are free to explore other types of apps on your own.

- Fill in all the project details and identifiers (e.g., project name, device, etc.). Make sure to name your project something does not conflict with another class or Swift library.

- Choose whether to initialize a git repository in your project's home folder. Another option is to just place your project's home folder in an existing git repository.

## What are the elements of an XCode project?

Please read the [following guide](https://guides.codepath.com/ios/Project-Basics) for extra support.

- The main UI area is called storyboard and is located within the **Main.storyboard** file. The launch screen for the app is located with the **Launchscreen.storyboard** file. 

- Both the storyboard and launch screen are located with the **Base.lproj** folder.

- The media assets are located in the **Assets.xcassets** folder. The **AppiIcon.appiconset** is where you set the various app icons.

- The **\<ProjectName\>Tests** and **\<ProjectName\>UITests** folders contain all unit tests for the project. We will not be covering Unit Tests in this class, but we encourage you to explore those on your own.

- The **Pods** folder, **Podfile**, and **Podfile.lock** contain all the necessary information for manging external libraries that are incorporated into your project.

- The **Info.plist**, which stands for information property list, is written in XML, and contains metadata that help maintain  persistence and consistency across the app.

- The **\<ProjectName\>.xcodeproj** or **\<ProjectName\>.xcodeworkspace** files are what you use to open up your project workspace in XCode.

## What are the elements in the XCode workspace?

- The left-hand side of the workspace contains the project and navigation hierarchy, i.e., the different project folders and their contained files. This can be toggled in and out of view by clicking the left button in the top-right of the header.

- The center area is the main work area. When .storyboard files are selected, this area displays the app's UI elements and layouts in the center/left, and the document outline in the center/center.

- Click the assistant editor button (two overlapping rings) on the top right of the header to show the accompanying code to the storyboard in the center/right area.

- The right-hand side contains various inspectors (File, Identity, Attributes, Size, etc.) on top and the Object Library on the bottom. This utilities area can be toggled in and out of view by clicking the right button in the top-right of the header.

- The bottom of the workspace contains the output console and the debugging terminal. This area can be toggled in and out of view by clicking the bottom button in the top-right of the header.

- There are three buttons in the top-left area of the header: to build and run the current project, to stop the current run, and to choose the simulator.

## When creating a new class, what type of file should I choose?

- Every UI element in your storyboard should be created as a **CocoaTouchClass**. This includes ViewControllers, TableViews, TableViewCells, CollectionViews, CollectionViewCells, etc.

- The model and API elements should be created as a **Swift File**. These do not rely on user interactions, but instead serve to mediate data among the various UI and storyboard elements.

- If you accidentally delete your storyboard or launch screen, you can create a new **Storyboard** or **Launch Screen** file.

- For Unit Tests, create a **UI Test Case Class** or **Unit Test Case** class.

- Create a new **Group** to group similar files together (e.g., views, models, managers, etc). Generally, files in one group are publicly visible to all other files in different groups, so there is not need to worry about package access as you would in another framework.
