# Paying Everyday Bills with Bitcoin

Spending Bitcoin at a retail checkout via a linked card is one use case; paying recurring, non-card obligations — rent, utilities, a mortgage, a phone bill — is a different problem, since most billers don't accept card payments at all, let alone Bitcoin directly. Lightning Pay Wallet's bill pay feature is built to bridge that gap.

## How it actually reaches a biller who doesn't accept crypto

The mechanism is straightforward: the wallet converts a chosen BTC or stablecoin amount and routes it to the biller as a standard ACH, wire, or check payment behind the scenes, depending on what the biller accepts. From the user's side, the transaction looks like paying with BTC directly from the wallet; from the biller's side, it arrives as an ordinary payment in their existing system. The [bill pay pillar guide](https://lightningpay.info/pay-bills-with-bitcoin) covers this end-to-end flow and the small (0.1%) fee that applies.

## Common bill categories covered

The wallet supports a range of specific, high-frequency bill types, each with its own dedicated guide covering biller compatibility and typical processing time:

- [Rent](https://lightningpay.info/pay-rent-with-bitcoin) — including guidance on paying a landlord or property manager who has no crypto infrastructure of their own.
- [Utilities](https://lightningpay.info/pay-utilities-with-bitcoin) — electric, water, and gas billers, typically paid via the biller's existing account-number-based payment system.
- [Mortgage payments](https://lightningpay.info/pay-mortgage-with-bitcoin) — larger, less frequent, and generally requiring more lead time given ACH/wire settlement windows.
- [Phone bills](https://lightningpay.info/pay-phone-bill-with-bitcoin) — smaller, high-frequency payments well suited to Lightning's low-fee, fast-settlement design.
- [Credit card payments](https://lightningpay.info/pay-credit-card-with-bitcoin) — paying down an existing card balance directly from a BTC or stablecoin balance rather than routing through a bank account first.

## Timing considerations

Because the underlying settlement to the biller often depends on ACH or wire rails rather than Lightning's instant settlement, bill payments generally need more lead time than a point-of-sale card purchase — the BTC-to-fiat conversion inside the wallet is fast, but the onward payment to a traditional biller inherits that biller's normal processing window. Recurring bills like utilities or a mortgage are usually the ones worth scheduling a few business days ahead rather than on the due date itself.

## Which balance to pay from

As with the [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card), bill payments can draw from BTC, USDC, or USDT. Someone who wants predictable bill amounts without exposure to BTC price swings between scheduling a payment and it clearing can pay directly from a stablecoin balance; someone comfortable with BTC volatility can pay from BTC directly. The [stablecoins overview](https://lightningpay.info/stablecoins) covers this trade-off in more depth.

## Tax implications of paying bills in BTC

Similar to card spending, using BTC to pay a bill is generally treated as a disposal for tax purposes in most jurisdictions — the difference between cost basis and value at the time of payment is a reportable gain or loss. The [Bitcoin tax assistant](https://lightningpay.info/bitcoin-tax-assistant) logs bill payments alongside other disposal events specifically because of this.

## Why this matters beyond convenience

For someone paid partly or fully in Bitcoin, or holding meaningful BTC/stablecoin balances they'd otherwise need to manually off-ramp before paying ordinary bills, an integrated bill-pay feature removes a manual, multi-step process (sell BTC on an exchange, wait for settlement, withdraw to a bank account, then pay the bill) and replaces it with a single action inside the wallet. This is less about ideology and more about reducing the number of steps between holding an asset and using it for a routine obligation.

## Related articles

- [The Lightning Pay Bitcoin Visa Card](the-lightning-pay-bitcoin-visa-card.md)
- [Understanding the Lightning Network](understanding-the-lightning-network.md)
- [Bitcoin Tax Assistant: Cost Basis Tracking](bitcoin-tax-assistant-cost-basis-tracking.md)
- [Stablecoins in Your Wallet: USDC vs USDT](stablecoins-usdc-vs-usdt-in-your-wallet.md)
