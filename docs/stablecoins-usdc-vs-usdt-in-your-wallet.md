# Stablecoins in Your Wallet: USDC vs USDT

Lightning Pay Wallet holds Bitcoin and Lightning balances at the same 12-word seed as two dollar-pegged stablecoins, USDC and USDT. This article covers why a Bitcoin-focused wallet includes stablecoins at all, and how the two differ.

## Why hold a stablecoin in a Bitcoin wallet

Bitcoin's price moves. For someone who wants to hold spendable dollar value without leaving the wallet, moving to a bank account, or going through a separate exchange account, a stablecoin balance solves a specific problem: it lets funds sit at a roughly constant dollar value while remaining under the same self-custody model as the BTC balance. The [stablecoins overview](https://lightningpay.info/stablecoins) covers this rationale, along with the [volatility protection guide](https://lightningpay.info/stablecoins/volatility-protection), which walks through when converting BTC to a stablecoin balance temporarily makes sense versus when it doesn't.

## USDC: the regulated option

USDC is issued by Circle, is US-regulated, is structured for compliance with the EU's MiCA framework, and publishes monthly attestations of its reserves audited by Deloitte. In practice, this makes USDC the more conservative default for US and EU users who prioritize regulatory clarity and reserve transparency over anything else.

## USDT: the liquidity leader

USDT (Tether) is issued out of El Salvador and carries roughly two to three times the global trading volume of USDC. It's the default quote pair on most exchanges, and it dominates usage in Asia, the Middle East, and Latin America. For users who move funds frequently across exchanges or need the deepest liquidity in a given market, USDT is often the more practical choice even where USDC's regulatory profile might otherwise be preferred.

The full breakdown, including reserve composition and regional adoption patterns, is in the [USDC vs USDT comparison](https://lightningpay.info/stablecoins/usdc-vs-usdt).

## Bridging between Bitcoin and stablecoins

Because both stablecoins live at the same seed as the Bitcoin balance, converting between BTC and a stablecoin is an in-wallet swap rather than a withdrawal-and-rebuy through a third party. The [Bitcoin-stablecoin bridge guide](https://lightningpay.info/stablecoins/bitcoin-stablecoin-bridge) covers the mechanics of this swap and the fee that applies (0.1% on in-wallet swaps between BTC, USDC, and USDT — the same rate regardless of direction).

## Dedicated wallet views

For users who think in terms of a single asset rather than the whole portfolio, the wallet exposes focused views: the [USDC wallet page](https://lightningpay.info/usdc-wallet) and [USDT wallet page](https://lightningpay.info/usdt-wallet) each cover balance, send/receive, and swap actions scoped to that one asset.

## Where stablecoins intersect with spending

Stablecoin balances aren't just a parking spot — they're directly usable. The [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card) can spend from a USDC or USDT balance exactly as it can from BTC, auto-converting to local fiat at the point of sale with no added FX markup. Similarly, the [bill pay feature](https://lightningpay.info/pay-bills-with-bitcoin) can draw from whichever balance the user prefers.

## Practical guidance, not investment advice

Choosing between USDC and USDT is a practical question about jurisdiction, counterparty comfort, and liquidity needs — not a question with one universally correct answer. Users in the US or EU who want documented reserve backing generally lean USDC; users prioritizing the widest exchange support and deepest liquidity, especially outside the US/EU, often lean USDT. Neither choice is required — a user can hold BTC exclusively and never touch either stablecoin. This isn't financial advice, and anyone uncertain about tax or regulatory treatment of stablecoin holdings in their jurisdiction should consult a qualified professional; the [Bitcoin tax assistant](https://lightningpay.info/bitcoin-tax-assistant) can help track cost basis but doesn't substitute for that guidance.

## Related articles

- [Getting Started with Lightning Pay Wallet](getting-started-with-lightning-pay-wallet.md)
- [The Lightning Pay Bitcoin Visa Card](the-lightning-pay-bitcoin-visa-card.md)
- [Paying Everyday Bills with Bitcoin](paying-everyday-bills-with-bitcoin.md)
- [Bitcoin Tax Assistant: Cost Basis Tracking](bitcoin-tax-assistant-cost-basis-tracking.md)
