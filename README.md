# zkEmail Flutter App

This Flutter application demonstrates the use of the [zkEmail Flutter Package via Mopro](https://github.com/zkmopro/zkemail_flutter_package). It provides a simple interface to interact with the zkEmail Noir circuit, showcasing how to integrate zero-knowledge email verification into a mobile app.

## Prerequisites

Before you begin, ensure you have the following installed:

*   **Flutter SDK:** Follow the [official Flutter installation guide](https://docs.flutter.dev/get-started/install). Verify your installation by running `flutter doctor`.
*   **Android Development Environment:**
    *   Android Studio (includes Android SDK and platform-tools).
    *   An Android Emulator or a physical Android device.
*   **iOS Development Environment (for running on iOS or macOS):**
    *   Xcode (install from the Mac App Store).
    *   CocoaPods (`sudo gem install cocoapods`).
    *   **Important:** This project currently targets ARM64 architecture.
        *   It runs on physical iOS devices.
        *   It runs on Macs with Apple Silicon (M1/M2/M3) using the "My Mac (Designed for iPad)" target in Xcode.
        *   It **does not** run on the standard iOS Simulator on Intel-based Macs.

## Getting Started

Follow these steps to set up the project locally:

1.  **Clone the repository (if you haven't already):**
    ```bash
    git clone git@github.com:moven0831/zkemail_flutter_app.git
    cd zkemail_flutter_app
    ```

2.  **Install Flutter dependencies:**
    ```bash
    flutter pub get
    ```

## Running the Application

### Android

1.  **Ensure an Android device/emulator is ready:**
    *   List available emulators: `flutter emulators`
    *   Launch a specific emulator: `flutter emulators --launch <emulator_id>`
    *   Or, connect a physical Android device and enable USB debugging. Verify connection with `flutter devices`.
2.  **Run the app:**
    ```bash
    flutter run
    ```

### iOS / macOS (Apple Silicon)

1.  **Install iOS dependencies:**
    ```bash
    cd ios && pod install
    cd ..
    ```
2.  **Open the Xcode workspace:**
    ```bash
    open ios/Runner.xcworkspace
    ```
3.  **Configure and run in Xcode:**
    *   Select a physical iOS device from the target device list.
    *   **Alternatively, for Apple Silicon Macs:** Select "My Mac (Designed for iPad)" as the target.
    *   Click the **Run** button (▶) to build and launch the app.
