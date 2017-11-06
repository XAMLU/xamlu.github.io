# One Day Intro to XAML - Instructor Outline

The purpose of this document is to provide a the details necessary to guide a classroom of students through a step-by-step lab that creates a UWP app that interacts with a GitHub repository.

## Course Outline

The course is broken into a number of sections:

1. Getting started & Basic Navigation
    * Discuss
        * Discuss XAML & UWP
        * Where does Xamarin fit in?
            * Code sharing patterns
    * Module
        * Course Orientation
            * Discuss where to find resources
        * Introduce Shell Page
            * Discuss Windows 10 SDK versions and compatability
        * Add a Navigation View
            * Discuss `NavigationView` vs. `NavViewEx`
            * Discuss `NavProperties` attached properties
            * Discuss `x:Name` Page proerpty and element binding
1. Implementing Authentication
    * Discuss
        * Design - Fluent
        * Adaptive
        * OAuth & Web Auth Broker
        * Services
    * Module
        * App Callback
        * Setup app in GitHub
        * Add some services to App
            * Discuss the source for `GitHubLibrary`
            * Discuss `HttpClient` and show the debug diagnostics
        * Add Authentication UI
            * Discuss Binding vs x:Bind, INPC and Converters
            * Discuss `Visibility` vs Visual States.
        * Add auto-authentication to App
            * Discuss page/control lifecycle events such as Loaded
1. Implementing MVVM, Settings, etc.
    * Discuss
        * MVVM & INPC
            * Talk about MVVMLight. Where does T10 fit in?
    * Module
        * Add MVVMLight
        * Add a ViewModel
            * Walk-through the `HomePageViewModel`
            * Talk about Separation of Concerns
            * Could talk about Command pattern here
        * Implement Repository Search
            * Discuss Converters and implicit conversion
            * Discuss `ListView` and `RelativePanel`
        * Implement Settings
            * Discuss the `SettingsService`
            * Discuss `DesignModeEnabled` & `RelayCommand`
1. Messaging and Commanding
    * Discuss
        * Messaging
        * Commanding
    * Module
        * Implement messaging & commands
1. Issues, Master/Detail, Pivot for Issues
    * Discuss
        * Libraries
        * Microsoft UWP Community Toolkit
        * ObservableCollection
        * Item ViewModels
        * LINQ
        * Styles & Resources
    * Module
        * UWP Toolkit NuGet Package
            * Discuss ObservableCollection
            * Discuss item view-models
            * Discuss LINQ
        * Update Issues Logic
        * Update Issues UI
            * Discuss resources and templates.
1. Data entry and field/form validation
    * Discuss
        * What is validation and why do we need it?
        * What support for validation ships in UWP?
        * JSON, REST and WebClient
            > Show the source for the `GitHubClient`?
        * Global back button & back stack
    * Module
        * Add NavigationService
            * Discuss, why not setup navigation service until now?
        * Add Validation Property Helper
            * Discuss validation property and the problems of validation
        * Add create issue button to global nav bar
            * Discuss navigation view (line 50)
        * Add Create Issue Page
            * Discuss element binding
1. Additional topics
    * Telemetry
    * Deployment
        * Regular Store
        * Business Store
        * Side-loading
        * Beta distribution
    * Inking
    * Composition UI
    * Desktop Bridge
    * Controls
    * Template Studio
