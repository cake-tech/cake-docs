# Migrate from Zashi

Digital cash is meant to be simple to use, secure, and private by default, and yet Zcash wallets have been plagued with bad UX, privacy gotchas, and incomplete features from day one. With Zcash in Cake Wallet, all of that changes; from auto-shielding without a tap, automatically rotating transparent and shielded addresses, and a broad suite of features, we’re doing our part to make Zcash all it has promised since 2016.

We know migrating to a new wallet can be a stressful process, so we’ve worked hard to make this migration as seamless as possible for our users. In the following guide, we’ve broken down the migration process from Zashi wallet → Cake Wallet into an easy-to-follow guide, including screenshots of every step of the process.

## Getting started

Now let’s get you started migrating over! Migrating from Zashi → Cake only requires **three basic steps**, all of which are outlined in detail throughout the guide:

- [Migrate from Zashi](#migrate-from-zashi)
  - [Getting started](#getting-started)
  - [Installing Cake Wallet](#installing-cake-wallet)
  - [*Recommended method:* Sending to a new wallet in Cake](#recommended-method-sending-to-a-new-wallet-in-cake)
    - [Creating a new Zcash wallet on Cake](#creating-a-new-zcash-wallet-on-cake)
    - [Send Zcash balance from Zashi](#send-zcash-balance-from-zashi)
- [Using Cake Wallet](#using-cake-wallet)

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

The easiest path is to simply create a new Zcash wallet in Cake Wallet and transfer your funds over with a simple transaction. Not only does this allow you to skip the lengthy synchronization process of restoring an older Zcash wallet, but it also lets you get all of the benefits of using [one seed for all of your crypto hot wallets](https://blog.cakewallet.com/cake-wallet-introduces-monero-wallet-groups-new-seed-formats-and-more/).

With a new, 12-word seed, you get a fresh start, faster restoration, and the ability to leverage one backup for all of your favorite cryptocurrency wallets in Cake.

!!! warning
    As Zashi has implemented a different approach to change addresses than Cake Wallet and other more established Zcash wallets, restoring a Zashi seed phrase in Cake Wallet will not show all funds available. Please create a new wallet in Cake Wallet by following the guide below instead of attempting to restore your 24-word seed phrase from Zashi in Cake Wallet.

### Creating a new Zcash wallet on Cake

1. Download Cake Wallet [using the links above](#installing-cake-wallet)
2. Open Cake Wallet
3. Tap `Set a PIN` and set a PIN for the app
    1. Note: If you want to use a longer 6-digit PIN, simply tap `Switch to 6-digit PIN`
        
        ![Create a PIN](zashi/pin.png){: style="height:750px"}
        
4. Tap `Create New Wallet`
    
    ![Choose Create Wallet](zashi/create.png){: style="height:750px"}
    
5. Select `Zcash` as the wallet currency and then tap `Next`
    
    ![Select Zcash as the currency](zashi/zcash.png){: style="height:750px"}
    
    !!! note
        If you already have an existing wallet or wallet group in Cake Wallet, you can choose that group here to use an existing 12-word seed.

6. Enter a wallet name (or tap the 🔄 button to create a random name) and then tap `Next`
    
    ![Create your wallet's name](zashi/create_name.png){: style="height:750px"}
    
7. Follow the on-screen warnings about your seed phrase, then tap `Verify`

    a. Store your seed phrase in a safe place where you can import it into Cake Wallet in the next section. We recommend a few options:
    - Storing your seed in an **end-to-end encrypted** password manager like [Bitwarden](https://bitwarden.com/), [Proton Pass](https://proton.me/pass), or iCloud Keychain
    - Writing it down and keeping it in a **secure place**
    
    !!! warning
        Do not share these seed words with anyone or store them via screenshots or in an insecure note app, as anyone with access to your seed words has the ability to steal all of your Zcash!
    
8. Verify your backup by tapping the correct seed words in the order prompted
9. Tap `Receive` on the bottom dock to display a QR code with a Zcash receive address
    1. Note: If necessary, you can easily copy or share the address by tapping the icon next to the address, then sending to yourself via a messaging app, email, etc. 

![Tap Receive](zashi/home_receive.png){: style="height:750px"}
![Copy your address](zashi/receive.png){: style="height:750px"}

### Send Zcash balance from Zashi

1. Open Zashi
    
2. Tap the Send button in the middle of your screen
    
    ![Tap Send](zashi/zashi_home_send.png){: style="height:750px"}
    
3. Scan the QR code in Cake Wallet by tapping the QR code icon in the address box, or double tap or hold on the address field to paste in the address
4. Enter as close to the spendable balance as you can to send the entirety of your Zcash balance to your new Cake Wallet, then tap `Review`
   1. Unfortunately, Zashi does not support "sweeping" or sending your entire balance at once, so you'll have to do some guess work to see the max amount you can send out while leaving enough for the network fee.
    
    ![Enter address and amount](zashi/zashi_review.png){: style="height:750px"}
    
    !!! note
        Feel free to send a smaller, test transaction to Cake Wallet to test if it helps you feel more comfortable before sending your entire wallet balance!

5. Review the details, and then press `Send` when ready

    ![Review](zashi/zashi_send.png){: style="height:750px"}

6. Once you have sent the funds, confirm they show up in your new Zcash wallet in Cake

# Using Cake Wallet

Users get the full modern Zcash experience, shielded-by-default transactions, rotating transparent addresses, in-app swaps, AnyPay support, and real-world spending through [Cake Pay](https://cakepay.com), all wrapped in a polished interface that has been refined since 2018 through open-source development and real-world use.

That combination of deep Zcash integration, thoughtful privacy defaults, and proven longevity is what makes Cake Wallet the most advanced Zcash wallet available today.
