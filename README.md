# first_flutter_project

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Note

- the main() function in lib/main.dart . In its current form, it only tells Flutter to run the app defined in MyApp.
- Widgets are the elements from which you build every Flutter app. As you can see, even the app itself is a widget.
- The state class extends `ChangeNotifier`, which means that it can notify others about its own changes. For example, if the current word pair changes, some widgets in the app need to know.
- The state is created and provided to the whole app using a `ChangeNotifierProvider`. This allows any widget in the app to get hold of the state.

* MyHomePage
* Every widget defines a `build()` method that's automatically called every time the widget's circumstances change so that the widget is always up to date.
* `MyHomePage` tracks changes to the app's current state using the `watch` method.
* Every `build` method must return ** a widget** or (more typically) **a nested tree of widgets**. In this case, the top-level widget is `Scaffold`.
* Column is one of the most basic layout widgets in Flutter. It takes any number of children and puts them in a column from top to bottom.

Separate component `MyHomePage` is extracted into a new widget, `GeneratorPage`.

- Navigation: Widget `SafeArea` ensures that its child is not obscured by a hardware notch or a status bar.
- Expanded widget: let you express layouts where some **children take only as much space as they need** (SafeArea, in this case) and other widgets should take **as much of the remaining room as possible** (Expanded, in this case).
- The underscore (\_) at the start of \_MyHomePageState makes that class private and is enforced by the compiler. If you want to know more about privacy in Dart, and other topics
- there is no route in flutter. We see all thing and change all thing With Widget
- `Wrap` is a widget similar to `Row` or `Column` that automatically **wraps children to the next "line"** (called "run") when there isn't enough vertical or horizontal space.

- Flutter works with **logical pixels** as a unit of length. They are also sometimes called **device-independent pixels**. A padding of **8 pixels** is visually the same regardless of whether the app is running on an old low-res phone or a newer ‘retina' device. There are roughly 38 logical pixels per centimeter, or about 96 logical pixels per inch, of the physical display.
- `LayoutBuilder`. It lets you change your widget tree depending on how much available space you have.
  LayoutBuilder's builder callback is called every time the constraints change

### How StateWidgets work:

- **Mutable State**: Unlike stateless widgets that display a fixed UI based on their properties, stateful widgets have mutable state. This state can be updated throughout the widget's lifetime.
- **State Object**: The stateful widget itself doesn't directly manage the state. Instead, it creates a separate State object class. This state object holds the actual data that can be changed.
- **Build Method**: Both the StatefulWidget and its State object have a build method. The StatefulWidget's build method typically creates the state object and defines the overall structure of the widget. The State object's build method, on the other hand, uses the current state data to build the UI.
- **Updating State**: When the state needs to be changed, the State object calls a special method named setState. This tells Flutter that the state has changed, and it triggers a rebuild of the widget using the State object's build method again. This ensures the UI reflects the latest state.

## Questions

- what is widget?
  - Widgets are the elements from which you build every Flutter app. As you can see, even the app itself is a widget. Everything in a Flutter app is a widget
- StatelessWidget versus StatefulWidget?
