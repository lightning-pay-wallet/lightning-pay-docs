# Hardware Wallets and Multi-Wallet Support

Many Bitcoin users don't hold everything in a single wallet — some balance is kept accessible for spending, some in cold storage for long-term holding, and increasingly, some across more than one software wallet for different purposes. Lightning Pay Wallet's multi-wallet support is built around that reality rather than assuming a single-wallet setup.

## What multi-wallet support means here

Rather than requiring one wallet instance per device or per seed phrase, Lightning Pay Wallet lets a user manage multiple distinct wallets — each with its own seed — from a single app instance, switching between them without reinstalling or logging into separate accounts (since there are no accounts to log into in the first place). The [multi-wallet overview](https://lightningpay.info/multi-wallet-bitcoin) covers the interface for adding, naming, and switching between wallets.

## Common reasons to run more than one wallet

- **Separating spending from savings** — a smaller "hot" wallet for daily spending via the [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card) or [bill pay](https://lightningpay.info/pay-bills-with-bitcoin), and a larger balance kept in a wallet that's rarely touched.
- **Business vs personal funds** — keeping transaction histories cleanly separated, which also simplifies the kind of cost-basis tracking covered in the [tax assistant guide](https://lightningpay.info/bitcoin-tax-assistant).
- **Testing or gifting** — a small, disposable wallet for experimenting with a feature or for [gifting Bitcoin](https://lightningpay.info/bitcoin-gift-cards) without exposing a main wallet's balance or address history.

## Hardware wallet integration

For anyone holding a larger balance, keeping the private key entirely off a general-purpose phone or computer is a meaningful security upgrade over software-only storage. Lightning Pay Wallet supports connecting Ledger, Trezor, and BitBox hardware devices, which generate and store keys on dedicated offline hardware and only ever expose signed transactions to the connected app — never the raw private key.

This is a genuinely different security model from the software-based seed-phrase backup covered in the [private keys guide](https://lightningpay.info/security/private-keys-guide): a hardware wallet removes "malware on my computer captured my seed phrase" from the list of realistic attack vectors, at the cost of a small amount of added friction (needing the physical device present to sign a transaction).

## Using a hardware wallet alongside a software wallet

A common pattern is not choosing one or the other, but running both: a software wallet (as covered in the [getting started guide](getting-started-with-lightning-pay-wallet.md)) for day-to-day balances and spending, and a hardware-wallet-backed wallet for a larger, rarely-touched balance. Multi-wallet support is what makes managing both from one interface practical, rather than needing entirely separate apps.

## Watch-only vs full-access wallets

Some users add a hardware wallet in "watch-only" mode — able to see the balance and generate receive addresses without the ability to sign transactions unless the physical device is connected. This is useful for checking a cold-storage balance without needing the hardware device on hand at every check-in.

## Restoring across wallets

Because both software and hardware wallets in this context follow the BIP-39 standard covered in the [seed phrase guide](https://lightningpay.info/security/private-keys-guide), a wallet's balance can, in principle, be restored on different compatible hardware or software as long as the seed phrase and derivation path are preserved — this portability is what makes switching between, or combining, multiple wallets practical rather than being locked into one device or one piece of software indefinitely.

## When multi-wallet support isn't necessary

For a lot of users, a single wallet is entirely sufficient — multi-wallet and hardware integration exist for cases with larger balances, business use, or a specific reason to separate funds, not as a requirement for basic usage. The [FAQ](https://lightningpay.info/faq) covers the simpler single-wallet default setup for anyone not yet sure they need this.

## Related articles

- [Non-Custodial Security, Explained](non-custodial-security-explained.md)
- [Bitcoin Private Keys and Seed Phrases](bitcoin-private-keys-and-seed-phrases.md)
- [Getting Started with Lightning Pay Wallet](getting-started-with-lightning-pay-wallet.md)
- [Bitcoin Gift Cards Guide](bitcoin-gift-cards-guide.md)
