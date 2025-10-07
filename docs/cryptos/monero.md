---
title: "Monero"
parent: Cryptos
icon: simple/monero
---

# :crypto-monero: Monero

!!! note ""
    Official Website: [getmonero.org](https://www.getmonero.org/){:target="_blank"}

Monero `(XMR)` is the leading cryptocurrency focused on private and censorship-resistant transactions. It is a private, decentralized cryptocurrency that keeps your finances confidential and secure.

The majority of existing cryptocurrencies, including Bitcoin and Ethereum, have transparent blockchains. Transactions can be verified and/or traced by anyone in the world. This means that the sending and receiving addresses of these transactions could potentially be linked to real-world identities.

Monero, on the other hand, uses various technologies to ensure the privacy of its users.

## Seed Format

Cake Wallet uses a the 16-word Polyseed (Default) or the 25-word legacy seed for wallet creation and restoration.

## Syncing

**The most common issue with Monero is an unsynchronized wallet.**

To perform most interactions with your wallet, your wallet must be fully synchronized. There will be a green dot at the top of your home screen.

If you are stuck on the same block while syncing for a while, or it says disconnected, you should [try another node](../../features/advanced/custom-node) or another internet connection.

If your wallet is not fully synced, your wallet balance may be incorrect, and you won't be able to send transactions. You will need to wait until your wallet is fully synced before proceeding. Keep the app open with the screen on to keep syncing.

## Accounts and subaddresses

![Monero addresses](/images/monero-addresses.png)

### Monero subaddresses

A Monero subaddress is a unique, unlinkable address that can be generated on-demand. Coins sent to it will still arrive in your main wallet, but the person sending the coins cannot determine your wallet's main address. Cake Wallet now automatically generates new subaddresses after they are used by default.

If you want to manually manage your subaddresses, you can do so by going to privacy settings and disabling the "Auto generate subaddresses" feature. Then go to your receive screen. To create a new subaddress, tap on `Accounts and subaddresses`, then tap on `Addresses` and create a name for this address, then tap `Create`. Subaddresses always start with `8`. Your main address starts with `4`.

![New address](/images/receive-4.jpg){:width="32%"}
![New address name](/images/receive-5.jpg){:width="32%"}
![Copy address](/images/receive-6.jpg){:width="32%"}

### Monero accounts

Each Monero wallet can have several accounts. We recommend this feature for advanced users only. Within your Monero wallet, click `Receive`, then click `Accounts` or `Accounts and subaddresses`. You may need to also click on `Accounts` to change between your different accounts. You can have unlimited accounts, and each account can have unlimited subaddresses. The first indexed address of each account (besides the main account) starts with an `8`.

Balances and transactions for each Monero account are shown separately. While in one account, you can't see the balance and transactions of another account. You need to switch between accounts to see the balances and transactions of each. The balance of each account appears in the account list.

## View-only wallet

It's possible to create a Monero view-only wallet. You need the following information:

* Main Monero address (`4...`)
* Private view key
* Restore height (recommended, not required)

 Restore from keys following [these steps](../../get-started/setup/restore/). Leave the `Spend key (private)` field blank. Let the blockchain sync fully. After syncing, you should see all incoming transactions (*including* incoming change). View-only wallets usually do not show an accurate balance (they cannot be relied upon for this purpose), and they will not show some types of outgoing transactions.

## Monero fee levels

Cake Wallet follows the standard wallet2 fee levels. We recommend leaving your Cake Wallet fee for Monero as `Automatic`.

| Cake Wallet name | wallet2 priority value | CLI name | GUI Name | Multiplier |
| --- | --- | --- | --- | --- |
| Automatic | 0 | default | Automatic | x1 or x5, depending on network activity |
| Slow | 1 | unimportant | Slow | x1 |
| Medium | 2 | normal | Normal | x5 |
| Fast | 3 | elevated | Fast | x25 |
| Fastest | 4 | priority | Fastest | x1000 |

## Monero save recipient addresses

Monero addresses (unlike Bitcoin) are never stored on the blockchain. When you send Monero to a recipient, the address that you send to is only recorded locally, not on the blockchain. Thus, if you restore a Monero wallet from mnemonic seed or from keys, you will not see the Monero addresses that you sent funds to.

Additionally, Cake Wallet can be configured to discard the Monero recipient address. In settings, untick `Save recipient address`. If you send XMR while this option is disabled, then addresses are no longer retained. The record of which address(es) you send to are lost forever.

Disabling this feature is only recommended for advanced users who know what they're doing. Please leave it enabled if you are unsure.

## Auto generate subaddresses

In privacy settings, you can enable or disable the automatic generation of Monero subaddresses. This feature is enabled by default.

When enabled:

* You can still switch between different accounts.
* For each account, it will display in the receive screen the first **unused** subaddress after the last manually labeled or the last used subaddress.
* Your address book will be collapsed to only show one entry per account, which will be linked to the latest subaddress for the relevant account.

You can disable this feature in settings. Doing so will restore the same functionality as before: you will need to manually label and switch to each subaddress.
