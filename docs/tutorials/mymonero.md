# Migrate from MyMonero

We know migrating to a new wallet can be a stressful process, so we’ve worked hard to make this migration as seamless as possible for our users. In the following guide, we’ve broken down the migration process from MyMonero wallet → Cake Wallet into an easy-to-follow guide, including screenshots of every step of the process.

## Getting started

Now let’s get you started migrating over! Migrating from MyMonero → Cake only requires **three basic steps**, all of which are outlined in detail throughout the guide:

1. [Install Cake Wallet](#installing-cake-wallet)
2. [Create a new Monero wallet](#recommended-method-sending-to-a-new-wallet-in-cake)
3. [Send all of your Monero in MyMonero wallet to the newly created Monero wallet in Cake](#send-monero-balance-from-mymonero-mobile)

Now for those who specifically want to keep their transaction history or have another reason to re-use their existing MyMonero 25-word Monero seed, feel free to jump down to the relevant section:

[*Advanced method:* Exporting an existing wallet to Cake](#advanced-method-exporting-an-existing-wallet-to-cake)

Not so daunting now, is it? **Let’s get started.**

!!! note ""
    💁

    **We’re here to help!**

    If at any point you get nervous or need help, please don’t hesitate to reach out to our team in-app or via support@cakewallet.com, where our incredible support staff are waiting to help ease the migration process for you.

## Installing Cake Wallet

Cake Wallet is available on Android, iOS, macOS, Linux, and Windows.

For the best compatibility and easiest setup we recommend using the mobile version of Cake Wallet to get started, and then explore our desktop apps down the line.

Please choose one of the options below to get started:

[:simple-android: Android](/get-started/android/){ .md-button }
[:simple-apple: iOS / macOS](/get-started/app-store){ .md-button }
[:simple-linux: Linux](/get-started/linux/){ .md-button }
[:material-microsoft-windows: Windows](/get-started/windows){ .md-button }

## *Recommended method:* Sending to a new wallet in Cake

The easiest path is to simply create a new Monero wallet in Cake Wallet and transfer your funds over with a simple transaction. Not only does this allow you to skip the lengthy synchronization process of restoring an older Monero wallet, but it also lets you get all of the benefits of a new seed format in Monero called “Polyseed.”

This newer seed format is easier to backup and restore (only 16 words, instead of 25), encodes the restore height directly into the seed phrase, and has several other security features that ensure your Monero stays safer than ever.

!!! note ""
    Alternatively, you can create a new Monero wallet using a 12-word BIP 39 seed, which enables you to use one seed for all of your crypto wallets in Cake. In the future this will be the default seed format for Monero wallets in Cake due to the simplicity it brings to seed backups.

### Creating a new Monero wallet on Cake

1. Download Cake Wallet [using the links above](#installing-cake-wallet)
2. Open Cake Wallet
3. Tap `Set a PIN` and set a PIN for the app
    1. Note: If you want to use a longer 6-digit PIN, simply tap `Switch to 6-digit PIN`
        
        ![Create a PIN](mymonero/pin.png){: style="height:750px"}
        
4. Tap `Create New Wallet`
    
    ![Choose Create Wallet](mymonero/create.png){: style="height:750px"}
    
5. Select `Monero` as the wallet currency and then tap `Next`
    
    ![Select Monero as the currency](mymonero/monero.png){: style="height:750px"}
    
6. Enter a wallet name (or tap the 🔄 button to create a random name) and then tap `Next`
    
    ![Create your wallet's name](mymonero/create_name.png){: style="height:750px"}
    
7. Follow the on-screen warnings about your seed phrase, then tap `Verify`

    a. Store your seed phrase in a safe place where you can import it into Cake Wallet in the next section. We recommend a few options:
    - Storing your seed in an **end-to-end encrypted** password manager like [Bitwarden](https://bitwarden.com/), [Proton Pass](https://proton.me/pass), or iCloud Keychain
    - Writing it down and keeping it in a **secure place**
    
!!! warning
    Do not share these seed words with anyone or store them via screenshots or in an insecure note app, as anyone with access to your seed words has the ability to steal all of your Monero!
    
1. Verify your backup by tapping the correct seed words in the order prompted
2. Tap `Receive` on the bottom dock to display a QR code with a Monero receive address
    1. Note: If necessary, you can easily copy or share the address by tapping the icon next to the address, then sending to yourself via a messaging app, email, etc. 

![Tap Receive](mymonero/home_receive.png){: style="height:750px"}

![Copy your address](mymonero/receive.png){: style="height:750px"}

### Send Monero balance from MyMonero Mobile

1. On the home page of MyMonero, select the wallet you want to migrate over to Cake
    
    ![Choose your wallet in MyMonero](mymonero/mm_choose_wallet.png){: style="height:750px"}
    
2. Tap the Send button at the top right
    
    ![Tap Send](mymonero/mm_home_send.jpeg){: style="height:750px"}
    
3. Scan the QR code in Cake Wallet by tapping `Use Camera`, or tap the address field to paste in the address
4. Tap `Max` to send the entirety of your Monero balance to your new Cake Wallet, then tap `Send`
    
    ![Enter address and tap Max](mymonero/mm_send.jpeg){: style="height:750px"}
    ![Tap Send at the top right](mymonero/mm_send_tap.jpg){: style="height:750px"}
    
!!! note
    Feel free to send a smaller, test transaction to Cake Wallet to test if it helps you feel more comfortable before sending your entire wallet balance!

5. Enter your wallet password, and tap `Next` to send the transaction
6. Once you have sent the funds, confirm they show up in your new Monero wallet in Cake

## *Advanced method:* Exporting an existing wallet to Cake

For those who want to preserve their transaction history or have a specific reason to keep using their existing MyMonero seed phrase, you can easily export it and restore in Cake Wallet.

!!! note
    When using this method, you'll notice the main difference between MyMonero and Cake Wallet. MyMonero relies on sending a view key to a remote server, something that reduces your privacy but forgoes the need to sync your wallet at all. Cake Wallet takes a different approach, where you do all wallet sync on-device for maximum privacy. This sync process can take some time when restoring older wallets, but can be drastically improved by performing initial sync on a good network or enabling [background sync on Android](/features/advanced/background-sync/).

### Backing up your Monero from MyMonero

1. On the home page of MyMonero, select the wallet you want to migrate over to Cake

    ![Choose your wallet in MyMonero](mymonero/mm_choose_wallet.png){: style="height:750px"}

2. Expand the toggle/drop-down by Address

    ![Expand the secrets dropdown](mymonero/mm_home_dropdown.jpeg){: style="height:750px"}

3. Confirm that you’re in a safe place and are OK to display your private keys on-screen

!!! warning
    Do not share these seed words with anyone or store them via screenshots or in an insecure note app, as anyone with access to your seed words has the ability to steal all of your Monero!

5. Either tap the copy button, or write down your 25-word seed phrase (in the box labeled `Secret Mnemonic`) in a safe place where you can import it into Cake Wallet in the next section. We recommend a few options:
    - Storing your seed in an **end-to-end encrypted** password manage like Bitwarden, Proton Pass, or iCloud Keychain
    - Writing it down and keeping it in a **secure place**

    ![Copy your Secret Mnemonic](mymonero/mm_copy_seed.jpg){: style="height:750px"}

### Restoring your wallet in Cake Wallet

1. Tap `Set a PIN` and set a PIN for the app
    
    ![Create a PIN](mymonero/pin.png){: style="height:750px"}
    
2. Tap `Restore Existing Wallet`
    
    ![Choose Restore Wallet](mymonero/restore.png){: style="height:750px"}
    
3. Tap `Restore from seed/keys`
    
    ![Choose Restore from Seed/Keys](mymonero/restore_seed.png){: style="height:750px"}
    
4. Select `Monero` as wallet currency and then tap `Next`
    
    ![Select Monero as the currency](mymonero/monero.png){: style="height:750px"}
    
5. Choose a name for the wallet
6. Paste or type in the seed phrase from MyMonero wallet that you backed up earlier
    
    ![Enter your 25-word seed phrase from MyMonero](mymonero/restore_seed_poly.png){: style="height:750px"}
    
7. Tap the `Polyseed (16 words)` option and change to `Legacy (25 words)`

    ![Change to Legacy seed type](mymonero/restore_legacy.png){: style="height:750px"}
    
8. Tap `Restore`
9.  Once restored, you will see a synchronization status bar at the top of the balance screen as Cake Wallet checks the Monero blockchain for your wallet history and balance
10. When Cake Wallet finishes the synchronization process and the top bar says `SYNCHRONIZED`, you will see your full balance and transaction history

# Using Cake Wallet

Cake Wallet is the user-friendly, multi-asset cryptocurrency wallet that prioritizes financial privacy and autonomy. With seamless swaps, strong privacy tools, and a focus on accessibility, Cake Wallet empowers you to manage, swap, and spend your digital assets securely and confidently. Cake Wallet is also 100% open-source, ensuring that every bit of code is able to be verified and independently reviewed, keeping your crypto safer than ever from attacks or mistakes.

Cake Wallet also enables you to easily swap between cryptocurrencies without leaving the app, buy and sell directly from fiat, and even use your crypto to buy every day items and treat yourself with [Cake Pay](https://cakepay.com). It’s your freedom money, and Cake helps free you up to use it in more ways than ever.
