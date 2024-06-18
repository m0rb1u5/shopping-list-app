# Flutter: Shopping List App

## Pre-requirements

1. [Install Git 2.27 or major](https://git-scm.com/downloads).
2. [Install the Visual Studio Code 1.77 or major](https://code.visualstudio.com/).
3. Install some extensions in Visual Studio Code<sup>*</sup>:
   - [Flutter](https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter) (required).
   - [Dart](https://marketplace.visualstudio.com/items?itemName=Dart-Code.dart-code) (required).
   - [Pub Manager](https://marketplace.visualstudio.com/items?itemName=qlevar.pub-manager) (required).
   - [Json to Dart Model](https://marketplace.visualstudio.com/items?itemName=hirantha.json-to-dart) (required).
   - [Flutter Riverpod Snippets](https://marketplace.visualstudio.com/items?itemName=robert-brunhage.flutter-riverpod-snippets) (required).
   - [Postman](https://marketplace.visualstudio.com/items?itemName=Postman.postman-for-vscode) (required).
   - [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) (required).
   - [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens) (required).
   - [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) (required).
   - [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) (required).
   - [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) (optional).
   - [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) (optional).
4. [Install Rosetta 2](https://support.apple.com/en-us/102527) (just to macOS with Apple silicon): `sudo softwareupdate --install-rosetta --agree-to-license`
5. [Install Xcode 15](https://developer.apple.com/xcode/) (just to macOS).
6. [Install CocoaPods 1.15 or major](https://cocoapods.org/) (just to macOS).
7. [Install Android Studio](https://developer.android.com/studio).

   During the install process or if installed, install the next components::
   - Android SDK Platform, API 34.0.0.
   - Android SDK Command-line Tools.
   - Android SDK Build-Tools.
   - Android SDK Platform-Tools.
   - Android Emulator.
8. Install some plugins in Android Studio:
   - [Flutter](https://plugins.jetbrains.com/plugin/9212-flutter).
   - [Genymotion](https://plugins.jetbrains.com/plugin/7269-genymotion).
9. [Install Genymotion Desktop](https://www.genymotion.com/product-desktop/download/).
10. Install Flutter SDK. For this step, you can follow the next options (the first one is recommended):

    - [Use VS Code to install Flutter](https://docs.flutter.dev/get-started/install/windows/mobile?tab=vscode#use-vs-code-to-install-flutter).
    - [Download then install Flutter](https://docs.flutter.dev/get-started/install/windows/mobile?tab=download#download-then-install-flutter).

Comments:

*: The repository will automatically install and configure required extensions when opened in VS Code. It is also recommended to create a Flutter configuration [profile in VS Code](https://code.visualstudio.com/docs/editor/profiles).

## Configuration

1. Configurate a Android device:
   - [Set up a Android emulator: Using Genymotion](https://docs.genymotion.com/desktop/Get_started/014_Basic_steps/) (recommended option):
     - [Install Open GApps](https://support.genymotion.com/hc/en-us/articles/4414586104977-How-to-install-Google-Play-Store-and-other-Google-Apps-in-Genymotion).
   - [Set up a Android emulator: Using Androd Studio](https://docs.flutter.dev/get-started/install/windows/mobile?tab=virtual#set-up-the-android-emulator).
   - [Set up a real Android device](https://docs.flutter.dev/get-started/install/windows/mobile?tab=physical#set-up-your-target-android-device).
2. Configurate a iOS device (just to macOS):
   - [Set up a iOS simulator](https://docs.flutter.dev/get-started/install/macos/mobile-ios?tab=virtual#configure-your-target-ios-device).
   - [Set up a real iOS device](https://docs.flutter.dev/get-started/install/macos/mobile-ios?tab=physical#configure-your-target-ios-device).
3. To verify if all components of a complete Flutter development environment were installed, run the following command: `flutter doctor`. The result of your command should resemble:

   ```bash
   Doctor summary (to see all details, run flutter doctor -v):
   [✓] Flutter (Channel stable, 3.22.1, on macOS 14.4.1 23E224 darwin-arm64, locale pt-BR)
   [✓] Android toolchain - develop for Android devices (Android SDK version 34.0.0)
   [✓] Xcode - develop for iOS and macOS (Xcode 15.0)
   [✓] Chrome - develop for the web
   [✓] Android Studio (version 2023.2)
   [✓] VS Code (version 1.89.1)
   [✓] Connected device (3 available)
   [✓] Network resources

   • No issues found!
   ```

4. [Install dependencies](https://docs.flutter.dev/packages-and-plugins/using-packages#adding-a-package-dependency-to-an-app). For this step, run the following command on the root project: `flutter pub get`.
5. Open the project on the IDE. You can use Visual Studio Code or Android Studio (the first one is recommended).

## Run and Debug

Before run into the IDE, run the virtual/physical device.

### In Visual Studio Code

1. Open the "Flutter" panel and select a mobile device or select using the command palette "Flutter: Select Device".
2. Open the "Run and Debug" panel.
3. Select a mode: Debug, Profile or Release.
4. Run by clicking on the green button.
5. After running is possible to open the DevTools on the "Flutter" panel.
