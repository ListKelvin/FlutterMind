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

## Questions

- StatelessWidget versus StatefulWidget?
