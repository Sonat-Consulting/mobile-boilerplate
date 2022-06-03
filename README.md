# mobileboilerplate

Mobile boilerplate project, using [Flutter](https://docs.flutter.dev/) and github actions)

## Requirements

Clone flutter repository from github:
Windows:
`git clone https://github.com/flutter/flutter.git -b stable`
then set the path variable to include the path you cloned to. E.g C:\src\flutter\bin
See [Installation for Windows](https://github.com/flutter/flutterdocs.flutter.dev/get-started/install/windows) for further information.
You will need different installations for Intel and M1 chips. Please refer to the documentation on [Installation for MacOs](https://docs.flutter.dev/get-started/install/macos)

Then run `flutter doctor` to see what else is needed

## Visual Studio code setup

If you are using vscode for development, you should install the two extensions called "Flutter" and "Dart".

Then, if you select the `main.dart` file, and select the "Run and debug" tab in vscode, you can create a new run configuration.

From there, you can now select run target device type in the bottom bar in vscode.

## Debugging

### iOS
run `flutter run` at the root of your project. The target can either be a simulator or a connected handset
For iOS refer to [this article](https://medium.com/front-end-weekly/how-to-test-your-flutter-ios-app-on-your-ios-device-75924bfd75a8#:~:text=You%20need%20to%20go%20to,app%20on%20your%20local%20device) to read about connecting your iOS device.

To connect to iOS simulator run the simulator installed with XCode see [Installation for MacOs](https://docs.flutter.dev/get-started/install/macos)

### Android

In vscode, in the bottom bar, select device type, and select your android emulator (or create a new one).

Then hit the run button in the menu, on the run and debug tab, and it should start building an android debug application.


## Github actions

Github actions is used to run tests and create builds, and eventually create new releases to App store and Google Play.

The ci scripts are located in the `.github/workflows/` folder.

You can use a tool called [`ack`](https://github.com/nektos/act) to run these actions locally.

Docker is used to build and run the actions locally.

1. `brew install ack`
2. `ack -l` to list actions available
3. `ack` to run the default "push" event action (run tests).