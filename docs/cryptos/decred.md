---
title: "Decred"
parent: Cryptos
# icon: simple/decred
---

<!-- # :crypto-litecoin: Litecoin -->

!!! note ""
    Official Website: [decred.org](https://decred.org/){:target="_blank"}

!!! warning
    Due to how much data the Decred wallet requires, it will make your Cake wallet backup very large, and in some cases can cause the backup creation to fail.

Decred `(DCR)` is a blockchain-based cryptocurrency with a strong focus on community input, open governance, and sustainable funding for development. It utilizes a hybrid Proof-of-Work (PoW) and Proof-of-Stake (PoS) mining system to ensure that a small group cannot dominate the flow of transactions or make changes to Decred without the input of the community. A unit of the currency is called a decred (DCR).

Stakeholders make and enforce the blockchain’s consensus rules, set a course for future development, and decide how the project’s treasury is used to fund it. Decred’s blockchain is similar to Bitcoin’s, but with major aspects of governance baked into the protocol.

To align incentives, block rewards are split between Proof-of-Work (PoW) miners, stakeholders and the Decred Treasury, which funds the project.

## Seed Format

Cake Wallet uses a 15-word seed format for Decred wallets. When creating or restoring a wallet, you'll need to use this 15-word seed phrase.

## Addresses

Cake automatically generates a new Decred address after each use for better privacy. Previous addresses continue to work.

## SPV Sync

The Decred wallet in Cake uses SPV (Simply Payment Verification) which maximizes privacy and data usage. It allows the wallet to only download blocks which it has transactions in.

SPV sync will require more data usage and time to sync than Bitcoin, but less than other coins like Monero. This also has much higher privacy assurances than using a light wallet implementation where the nodes check for your transactions.

!!! warning
    SPV sync requires much more data than a light wallet, and will require an initial synchronization on wallet creation. This may use lots of data, so make sure you are not on a metered network before starting.

For more detailed info on how SPV sync works, please refer to the official [Decred documentation](https://docs.decred.org/wallets/spv/).

