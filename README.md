# mobile-boilerplate

Mobile boilerplate project, using [Flutter](https://docs.flutter.dev/) and github actions)

### Requirements

Clone flutter repository from github:
Windows:
`git clone https://github.com/flutter/flutter.git -b stable`
then set the path variable to include the path you cloned to. E.g C:\src\flutter\bin
See [Installation for Windows](https://github.com/flutter/flutterdocs.flutter.dev/get-started/install/windows) for further information.
You will need different installations for Intel and M3 chips. Please refer to the documentation on [Installation for MacOs](https://docs.flutter.dev/get-started/install/macos)

Then run `flutter doctor` to see what else is needed

### Debugging

run `flutter run` at the root of your project. The target can either be a simulator or a connected handset
For iOS refer to [this article](https://medium.com/front-end-weekly/how-to-test-your-flutter-ios-app-on-your-ios-device-75924bfd75a8#:~:text=You%20need%20to%20go%20to,app%20on%20your%20local%20device) to read about connecting your iOS device.

To connect to iOS simulator run the simulator installed with XCode see [Installation for MacOs](https://docs.flutter.dev/get-started/install/macos)
