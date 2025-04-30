!!! note
    Background sync is currently only available on Android, and currently excludes Decred  wallets.

Background sync will attempt to sync your wallets in the background at the specified interval. This can help keep your wallet up to date, and avoid the need for syncing lots of blocks when opening them. Background sync currently attemps to sync all Monero wallets. Background sync for Monero only uses the private view key, which avoides keeping the private spend key in memory.

In the `Connection and sync` settings, you can enable or disable background syncing for your Monero wallets. By default this is disabled, and if enabled will background sync all Monero wallets.

There are three background sync options:

* **Daily**: Attempts to background sync approximately every eight-teen (18) hours
* **Hourly**: Attemps to background sync approximately every sixty (60) minutes
* **Aggressive**: Attempts to background sync approximately once every fifteen (15) minutes

Enabling background sync will require enabling `Unrestricted background service` and allowing the app to always run in the background.

Background sync has several additional settings which can be set to control network or device conditions.

## Notifications

You can enable transaction notifications by toggling the `Send notifications about new transactions setting`.

This will send a notification locally containing information about a new received transaction.

The notifications will only send during the background sync period, which will be as frequent as the `Background sync mode` setting.