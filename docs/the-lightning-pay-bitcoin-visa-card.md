# The Lightning Pay Bitcoin Visa Card

Holding Bitcoin and spending it at ordinary merchants have historically been two separate steps — sell to fiat, wait for settlement, then spend. The Lightning Pay Bitcoin Visa card collapses that into a single tap, drawing directly from a wallet balance at the moment of purchase.

## How it works at the point of sale

The card is linked to the same wallet holding BTC, USDC, and USDT. When a purchase is authorized, the wallet converts the chosen balance to the merchant's local fiat currency in real time and settles the transaction over standard Visa rails — meaning it works anywhere among the more than 80 million merchants globally that already accept Visa, with no special merchant integration required.

The [card overview](https://lightningpay.info/bitcoin-visa-card) covers the authorization flow in more detail, including why settlement is fast enough for ordinary point-of-sale use rather than requiring a pre-load-and-wait step.

## Cost structure

The card's economics are straightforward and worth stating precisely rather than in vague marketing language:

- No monthly fee
- No annual fee
- 0% FX markup on foreign currency transactions
- No minimum balance requirement to hold or use the card

The [fees overview](https://lightningpay.info/fees) lists this alongside the wallet's other fees (0.1% on in-wallet swaps, 0.5% on fiat on/off-ramp, 0.1% on bill pay), and the [comparison against traditional credit card fees](https://lightningpay.info/fees/vs-credit-cards) puts the FX markup figure specifically next to what many card networks and banks charge on international purchases.

## ATM access

Beyond point-of-sale purchases, the card supports ATM withdrawal in over 200 countries. Ordinary ATM operator fees still apply, since those are set by the ATM operator rather than the card issuer — this is consistent with how most debit and credit cards work internationally.

## Which balance gets spent

Because the card sits on top of a multi-asset wallet, a purchase can draw from BTC, USDC, or USDT depending on which balance the user selects (or a default balance, if configured). This matters practically: someone holding a stablecoin balance specifically to avoid Bitcoin's price volatility can spend from that balance directly, while someone comfortable spending BTC directly can do that instead. The [stablecoins guide](https://lightningpay.info/stablecoins) covers the reasoning behind holding a dollar-pegged balance alongside BTC.

## How this differs from custodial card products

Cash-back or rewards debit cards tied to custodial exchange accounts (Cash App and similar products fall in this category) spend from a balance the platform itself holds and controls. The Lightning Pay card spends from a non-custodial balance — the funds sit at addresses controlled by the user's own seed phrase until the moment of a transaction. The [comparison with Cash App](https://lightningpay.info/compare/lightning-pay-vs-cash-app) and [comparison with Strike](https://lightningpay.info/compare/lightning-pay-vs-strike) go into this distinction directly, since both of those are custodial-first products.

## Everyday use cases beyond retail purchases

The same underlying settlement speed that makes the card work at checkout also underpins the wallet's [bill pay feature](https://lightningpay.info/pay-bills-with-bitcoin), letting BTC or stablecoin balances cover recurring obligations like [rent](https://lightningpay.info/pay-rent-with-bitcoin), [utilities](https://lightningpay.info/pay-utilities-with-bitcoin), and [credit card payments](https://lightningpay.info/pay-credit-card-with-bitcoin) without a separate off-ramp step.

## Getting a card

Card issuance is tied to the wallet install; the [download page](https://lightningpay.info/download) and [getting started guide](getting-started-with-lightning-pay-wallet.md) cover the installation prerequisites. Specific card ordering and activation steps, along with regional availability, are covered in the [FAQ](https://lightningpay.info/faq).

## Related articles

- [Stablecoins in Your Wallet: USDC vs USDT](stablecoins-usdc-vs-usdt-in-your-wallet.md)
- [Paying Everyday Bills with Bitcoin](paying-everyday-bills-with-bitcoin.md)
- [Understanding the Lightning Network](understanding-the-lightning-network.md)
- [Comparing Lightning Pay to Other Wallets](comparing-lightning-pay-to-other-wallets.md)
