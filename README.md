## Flutter Desktop Application
 
## Requirements
To compile a desktop application, you must build it on the targeted platform: build a Windows application on Windows, a macOS application on macOS, and a Linux application on Linux.

To create a Flutter application with desktop support, you need the following software:
- Flutter SDK. See the <a href = "https://docs.flutter.dev/get-started/install"> Flutter SDK </a>installation instructions.
- Optional: An IDE that supports Flutter. See <a href = "https://docs.flutter.dev/get-started/editor">setting up an editor</a> for more details.

## Additional Platform Specific Requirements
- <a href="https://docs.flutter.dev/development/platform-integration/desktop#additional-windows-requirements"> Additional Windows requirements </a>
- <a href="https://docs.flutter.dev/development/platform-integration/desktop#additional-macos-requirements"> Additional MacOS requirements </a>
- <a href="https://docs.flutter.dev/development/platform-integration/desktop#additional-linux-requirements"> Additional Linux requirements </a>

## Check if set-up is correct
- Check if everything is set-up correctly as described <a href="https://docs.flutter.dev/development/platform-integration/desktop#set-up"> here </a>

## Creating Flutter project with Desktop support
When you create a new Flutter project you can indicate which platforms you want to support, by default chosen only Android and iOS, but you can enable all 6 platforms

<img width="712" alt="Screen Shot 2022-08-07 at 2 14 30 PM" src="https://user-images.githubusercontent.com/30071369/183283933-b41b96de-40c5-4888-bcca-59576a73d9bc.png">

After creating a project, you should run the following commands in a terminal from the root project directory:
- `flutter pub get` (This command gets all the dependencies listed in the pubspec.yaml file in the current working directory, as well as their transitive dependencies)
- Run the Desktop application using the command: `flutter run`

## Enabling Desktop support for existing project
To add desktop support to an existing Flutter project, run the following command in a terminal from the root project directory:
`flutter create --platforms=windows,macos,linux`
This adds the necessary desktop files and directories to your existing Flutter project. To add only specific desktop _platforms_, change the platforms list to include only the platform(s) you want to add.

## Build a release app
To generate a release build, run one of the following commands:
`flutter build windows`
`flutter build macos`
`flutter build linux`
