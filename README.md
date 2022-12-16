# MyMauiTraining
Lots of .NET Tutorials are going to be in here

# File Structure
- The `Resources` folder contains shared fonts, images, and assets used by all platforms.
- The `MauiProgram.cs` file contains the code that configures the app and specifies that the App class should be used to run the application.
- The `App.xaml.cs` file, the constructor for the App class creates a new instance of the `AppShell class`, which is then displayed in the application window.
- The `AppShell.xaml` file contains the main layout for the application and starting page of `MainPage`.
- The `MainPage.xaml` file contains the layout for the page. This layout includes the XAML code for a button with the caption `Click me`, and an image that displays the `dotnet_bot.png` file. There are two other labels as well.
- The `MainPage.xaml.cs` file contains the application logic for the page. Specifically, the `MainPage` class includes a method named `OnCounterClicked` that runs when the user taps the Click me button.

To recap, a .NET MAUI project initially contains:

The `MauiProgram.cs` file that contains the code for creating and configuring the Application object.

The `App.xaml` and `App.xaml.cs` files that provide UI resources and create the initial window for the application.

The `AppShell.xaml` and `AppShell.xaml.cs` files that specify the initial page for the application and handle the registration of pages for navigation routing.

The `MainPage.xaml` and `MainPage.xaml.cs` files that define the layout and UI logic for the page displayed by default in the initial window.

# Layouts
![layouts](/assets/maui-layout-types.png)
- `VerticalStackLayout` and `HorizontalStackLayout`, optimized stack layouts that lay out controls in a top-to-bottom or left-to-right stack. A `StackLayout` is also available, which has a property named `StackOrientation`, which you can set to `Horizontal` or `Vertical`. On a tablet or phone, modifying this property in your application code enables you to adjust the display if the user rotates the devic
- `AbsoluteLayout`, which lets you set exact coordinates for controls.
- `FlexLayout`, which is similar to `StackLayout` except that it enables you to wrap the child controls it contains if they don't fit in a single row or column. This layout also provides options for alignment and adapting to different screen sizes. For example, a `FlexLayout` control can align its child control to the left, right, or center when arranged vertically. When aligned horizontally, controls can be justified to ensure even spacing. You could use a horizontal `FlexLayout` inside a `ScrollView` to display a horizontally scrollable series of frames (each frame could itself be a vertically arranged `FlexLayout`)
- `Grid`, which lays out its controls according to a column and row location we set. You can define the column and row sizes as well as spans, so grid layouts don't necessarily have a "checkerboard look" to them.
- https://learn.microsoft.com/en-us/training/modules/build-mobile-and-desktop-apps/7-summary
- https://www.youtube.com/watch?v=rMWcd7srbnw
  