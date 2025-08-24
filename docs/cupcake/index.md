# Cupcake: Air-Gapped Wallet

Cupcake is a secure, air-gapped mobile wallet that leverages live QR codes for transaction signing. It is designed with a focus on security by isolating your private keys from your primary, online device.

**Note:** Cupcake is currently in a BETA phase. It is recommended for users who are familiar with air-gapped wallets and are comfortable with self-troubleshooting.

## How It Works

Cupcake operates on a two-device system, similar to a hardware wallet, to provide enhanced security for your crypto assets.

*   **Cupcake App:** This app is installed on a dedicated, offline device. It securely stores your private keys and is used exclusively for signing transactions.
*   **Cake Wallet App:** This is your everyday wallet app, installed on your primary, online device. It holds the view keys, allowing you to monitor your balance, view transaction history, and create new transactions to be signed.

The communication between the two apps is handled entirely through QR codes, ensuring that your private keys never leave the offline device.

## Supported Cryptocurrencies

Currently, Cupcake offers support for Monero (XMR) and Bitcoin (BTC). Support for additional cryptocurrencies is planned for future releases.

## Download and Installation

Cupcake is available for both iOS and Android platforms. You can download the app from the following sources:

*   **App Store:** [Link to App Store](https://apps.apple.com/eg/app/cupcake-by-cake-wallet/id6737430272)
*   **Play Store:** [Link to Play Store](https://play.google.com/store/apps/details?id=com.cakewallet.cupcake)
*   **GitHub Releases:** [Link to GitHub Releases](https://github.com/cake-tech/cupcake/releases)

## Project Structure

The Cupcake project is a Flutter-based application, organized into the following key directories:

| Path | Description |
| :--- | :--- |
| **`.github/`** | Contains GitHub Actions workflows for continuous integration, including building releases and running linters. |
| **`android/`** | Holds the Android-specific project files, including Gradle configurations, manifests, and native code. |
| **`assets/`** | Includes all static assets for the application, such as images, fonts, and icons. |
| **`ios/`** | Contains the iOS-specific project files, including Xcode project configurations and native code. |
| **`lib/`** | The core of the Flutter application, containing all the Dart source code. |
| **`lib/coins/`** | Implements the logic for different cryptocurrencies, with separate modules for Monero and Bitcoin. |
| **`lib/view_model/`** | Contains the view models, which manage the application's state and business logic. |
| **`lib/views/`** | Includes all the UI components of the application, such as screens, widgets, and dialogs. |
| **`macos/`** | Holds the macOS-specific project files. |
| **`.tooling/`** | Contains various scripts and tools used for development and building the application. |

## Building from Source

To build the Cupcake application from the source code, you will need to have the Flutter SDK and the appropriate development environment set up for your target platform (Android or iOS).

### Prerequisites

*   Flutter SDK (version 3.29.3)
*   For Android: Android Studio and the Android SDK
*   For iOS: Xcode and CocoaPods

### Build Steps

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/cake-tech/cupcake.git
    cd cupcake
    ```

2.  **Install dependencies:**
    ```bash
    flutter pub get
    ```

3.  **Prepare for development:**
    ```bash
    make prepare_dev
    ```

4.  **Build the application:**

    *   **Android:**
        ```bash
        make libs_android_build
        make cupcake_android_monero
        ```

    *   **iOS:**
        ```bash
        make libs_ios_build
        make cupcake_ios_monero
        ```

## Contributing

Contributions to the Cupcake project are welcome. To contribute, please follow these steps:

1.  Fork the repository on GitHub.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with clear, descriptive messages.
4.  Push your changes to your forked repository.
5.  Create a pull request to the main Cupcake repository.

Before submitting a pull request, please ensure that your code adheres to the existing code style and that all tests pass.

## License

Cupcake is released under the GNU General Public License v3.0. For more details, see the [LICENSE](https://github.com/cake-tech/cupcake/blob/main/LICENSE) file.
