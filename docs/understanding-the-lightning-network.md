# Understanding the Lightning Network

Bitcoin's base layer settles roughly every ten minutes and charges a fee per transaction that fluctuates with network demand — workable for larger transfers, impractical for buying a coffee. The Lightning Network exists specifically to solve that gap, and Lightning Pay Wallet uses both layers side by side at the same seed.

## The core idea

Instead of writing every single payment to the Bitcoin blockchain, Lightning lets two parties open a payment channel backed by an on-chain transaction, then exchange an unlimited number of instant, off-chain balance updates within that channel. Only the opening and closing balances typically need to touch the base chain. Routed correctly across a network of channels, this lets a payment travel from any wallet to any other Lightning-connected wallet in under a second, for a fee usually well under one cent.

The [Bitcoin basics overview](https://lightningpay.info/bitcoin/what-is-bitcoin) covers how the base layer works first, which is useful context before Lightning makes full sense — Lightning is a layer built on top of Bitcoin's settlement guarantees, not a separate currency or a separate trust model.

## Two ways to receive a Lightning payment

Lightning Pay Wallet supports both common formats:

- **BOLT11 invoices** — a single-use, amount-specified string generated for one specific payment, typically shown as a QR code.
- **Lightning Addresses** — a reusable, email-style identifier (`name@domain`) that can receive repeated payments without generating a new invoice each time, similar in spirit to a bank account number.

Both formats settle to the same underlying wallet balance; the difference is just convenience for the sender.

## Why this matters for everyday spending

The [bill pay overview](https://lightningpay.info/pay-bills-with-bitcoin) and related pages — covering [rent](https://lightningpay.info/pay-rent-with-bitcoin), [utilities](https://lightningpay.info/pay-utilities-with-bitcoin), and [mobile bills](https://lightningpay.info/pay-phone-bill-with-bitcoin) — depend on Lightning's speed and low fees to be practical at all. A ten-minute on-chain confirmation with a variable fee doesn't work for routine, recurring payments; sub-second settlement with negligible fees does.

Similarly, the [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card) relies on being able to authorize a point-of-sale transaction in real time, which is only feasible using Lightning-speed settlement underneath the card rails.

## On-chain vs Lightning: when each is used

A well-designed wallet doesn't force a user to choose a layer manually for every transaction. In practice:

- **On-chain** tends to suit larger, infrequent transfers, cold-storage withdrawals, and moving funds to or from an exchange or hardware wallet.
- **Lightning** tends to suit smaller, frequent, time-sensitive payments — the coffee-purchase end of the spectrum, plus card-linked spending and bill pay.

The [wallet overview](https://lightningpay.info/wallet) explains how both balances are presented within a single interface rather than as two disconnected products.

## Fees on the Lightning side

Lightning routing fees are typically a small fraction of a cent per hop and are separate from the wallet's own fee schedule (0.1% on in-wallet swaps, 0.1% on bill pay, 0% monthly). The [fees overview](https://lightningpay.info/fees) and the [comparison against credit card fees](https://lightningpay.info/fees/vs-credit-cards) put these numbers next to traditional payment rails for context.

## A note on liquidity

One Lightning-specific detail worth understanding: channels have finite capacity in each direction, meaning a wallet occasionally needs to manage "inbound" vs "outbound" liquidity behind the scenes to keep payments routing smoothly. This is handled automatically inside Lightning Pay Wallet and doesn't require manual channel management from the user — a meaningful usability difference from earlier, more technical Lightning wallets.

## Related articles

- [Getting Started with Lightning Pay Wallet](getting-started-with-lightning-pay-wallet.md)
- [Paying Everyday Bills with Bitcoin](paying-everyday-bills-with-bitcoin.md)
- [The Lightning Pay Bitcoin Visa Card](the-lightning-pay-bitcoin-visa-card.md)
- [Non-Custodial Security, Explained](non-custodial-security-explained.md)
