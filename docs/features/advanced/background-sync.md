!!! warning
    Background sync is currently only available on Android with Monero wallets. Background sync will also sync regardless of network condition or charging status, with more options to control this coming in the next version.

Background sync will attempt to sync your wallets in the background at the specified interval. This can help keep your wallet up to date, and avoid the need for syncing lots of blocks when opening them. Background sync currently attemps to sync all Monero wallets.

In `Connection and sync` settings, you can enable or disable background syncing for your Monero wallets. By default this is disabled, and if enabled will background sync all Monero wallets.

There are three background sync options:

* **Daily**: Attempts to background sync approximately every eight-teen (18) hours
* **Hourly**: Attemps to background sync approximately every sixty (60) minutes
* **Aggressive**: Attempts to background sync approximately once every fifteen (15) minutes

Enabling background sync will require enabling `Unrestricted background service` and allowing the app to always run in the background.

## Fixing background sync for GrapheneOS

GrapheneOS sets an Android config option that prevents Cake Wallet from being able to run its background sync service, however this flag can be set to false to remedy this issue. We are working to fix this on the Cake Wallet side, but in the meantime you can change this config option to allow background sync to run.

!!! warning
    We will not provide support in regards to fixing background sync compatibility on GrapheneOS, and while the required command is 100% safe to use, we are not responsible for any loss of data or damage caused by modifying your phone over ADB. Please proceed at your own caution. Enabling ADB can open your device to some risk, so we highly recommend turning ADB off after running the command.

### Steps

#### 1. Install the Android platform
Install the Android platform tools on your applicable platform by following the instructions from [XDA](https://www.xda-developers.com/install-adb-windows-macos-linux/).

#### 2. Connect your phone
Connect your phone to your computer and enable ADB either through USB or wireless debugging.

#### 3. Run the command
In your terminal, run `adb shell device_config put activity_manager_native_boot use_freezer false && adb reboot`. This will set the config option, reboot your device, and once rebooted this will prevent Android from freezing the Cake Wallet background process.

### Reverting

Just run `adb shell device_config put activity_manager_native_boot use_freezer true && adb reboot` and this will set the config option back to the default for GrapheneOS.