# Getting Started with Lightning Pay Wallet

Lightning Pay Wallet is a free, non-custodial Bitcoin and Lightning Network wallet with a built-in Bitcoin Visa card. This guide walks through what "non-custodial" actually means for a new user, how installation works, and where to go next once the wallet is running.

## What you're installing

Unlike an exchange account, Lightning Pay Wallet does not create a username and password on a company server. Installing the app generates a fresh private key on your own device, encoded as a 12-word recovery phrase (BIP-39 standard). That phrase — not an email/password pair — is the only thing that controls the funds. The [security overview](https://lightningpay.info/security) and the deeper [non-custodial explainer](https://lightningpay.info/security/non-custodial-explained) cover why this distinction matters in practice: no company can freeze the wallet, and no company can recover it if the phrase is lost.

## Step 1: Get the installer from the right place

The only official distribution point is the [download page](https://lightningpay.info/download), which serves signed builds for Windows 10/11 (.exe), macOS on Apple Silicon and Intel (.dmg), and Linux (Ubuntu, Fedora, Arch, as .zip). Mobile builds for iOS and Android are being rebuilt and are not currently distributed. Platform-specific installers and checksums are listed per OS.

## Step 2: Generate and back up your seed phrase

On first launch, the wallet generates the 12-word phrase client-side using a cryptographically secure random number generator. This is the single step that most new users under-invest in. The [private keys and seed phrase guide](https://lightningpay.info/security/private-keys-guide) is worth reading in full before funding the wallet — it covers writing the phrase down on paper (not a screenshot), keeping two copies in two separate physical locations, and why a phrase stored only digitally defeats the purpose of self-custody.

If you're unsure whether self-custody is the right model for you compared with an exchange account, the [non-custodial vs custodial comparison](https://lightningpay.info/security/vs-custodial) walks through the trade-offs plainly rather than as a sales pitch.

## Step 3: Fund the wallet

New users typically fund the wallet one of two ways:

- **Buy directly in-app**, which routes through the MoonPay on-ramp partner in 160+ countries. The [how-to-buy guide](https://lightningpay.info/bitcoin/how-to-buy) covers payment methods and typical settlement times.
- **Receive BTC or Lightning payments** from an existing wallet or exchange, using either an on-chain address or a Lightning invoice/Lightning Address.

There's no KYC requirement to install or use the wallet itself. KYC only applies where a partner rail (MoonPay for buying, Strike for bank withdrawals) is legally required to collect it in your region.

## Step 4: Understand the three balances you now hold

A single 12-word seed controls three types of balance at once: on-chain BTC, Lightning BTC, and dollar-pegged stablecoins (USDC and USDT). New users are sometimes confused about why a "Bitcoin wallet" also shows stablecoin balances — the short answer is that it's the same underlying key material, just different asset rails. The [stablecoins overview](https://lightningpay.info/stablecoins) explains why this exists (a way to hold dollar-equivalent value without leaving the wallet or the seed).

## Step 5: Know what the wallet can and can't do for you

Because the wallet is non-custodial:

- There is no "forgot password" flow. Losing the seed phrase means losing access permanently.
- There is no customer support line that can reverse a transaction or unfreeze a balance.
- Support requests are limited to app functionality, not fund recovery.

This isn't a limitation specific to Lightning Pay Wallet — it's inherent to any wallet where the user, not a company, holds the keys. The trade-off is that no third party can seize, freeze, or block the funds either.

## Where to go from here

Once the basics are running, a few natural next steps depending on how you plan to use the wallet:

- If you want to spend directly from BTC or stablecoin balances at regular merchants, look at the [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card).
- If you want to automate purchases over time instead of timing the market, see [Auto-DCA](https://lightningpay.info/auto-dca-bitcoin).
- If you use a Ledger, Trezor, or BitBox hardware wallet already, the [multi-wallet support guide](https://lightningpay.info/multi-wallet-bitcoin) explains how those integrate.
- For anything not covered here, the [FAQ](https://lightningpay.info/faq) has direct answers to the most common setup and account questions.

## Related articles

- [Non-Custodial Security, Explained](non-custodial-security-explained.md)
- [Bitcoin Private Keys and Seed Phrases](bitcoin-private-keys-and-seed-phrases.md)
- [Understanding the Lightning Network](understanding-the-lightning-network.md)
- [Hardware Wallets and Multi-Wallet Support](hardware-wallets-and-multi-wallet-support.md)
