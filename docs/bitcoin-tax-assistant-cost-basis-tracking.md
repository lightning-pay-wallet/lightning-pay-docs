# Bitcoin Tax Assistant: Cost Basis Tracking

Bitcoin's tax treatment in most jurisdictions requires tracking cost basis on every acquisition and calculating gain or loss on every disposal — a straightforward requirement in theory that becomes genuinely difficult once a wallet has accumulated dozens or hundreds of small transactions. Lightning Pay Wallet's built-in tax assistant is designed to keep that record automatically rather than reconstructing it after the fact.

## What gets logged automatically

Every transaction type that touches the wallet is recorded with the information a tax calculation actually needs:

- **On-ramp buys** — logged with USD cost basis at the second of purchase, sourced from the MoonPay or Strike transaction.
- **Sells and off-ramps** — proceeds and basis calculated against whichever lot-selection method the user has configured.
- **Spends** (via the [Bitcoin Visa card](https://lightningpay.info/bitcoin-visa-card) or [bill pay](https://lightningpay.info/pay-bills-with-bitcoin)) — treated as disposals for tax purposes in most jurisdictions, since spending BTC or a stablecoin is generally a taxable event distinct from spending cash.

The [tax assistant overview](https://lightningpay.info/bitcoin-tax-assistant) covers the full transaction taxonomy the tool tracks.

## Why lot-selection method matters

When a wallet holds Bitcoin purchased at different prices and times (which is the normal outcome of using [Auto-DCA](https://lightningpay.info/auto-dca-bitcoin) or making periodic manual buys), a disposal has to specify which specific lot is being sold — FIFO (first-in-first-out), LIFO (last-in-first-out), or specific-lot identification are the common methods, and the choice can materially change the reported gain or loss in a given year. Jurisdictions differ on which methods are permitted and how consistently a method must be applied year over year, which is a question for a tax professional rather than something this article can answer generally.

## Why this matters more with frequent small transactions

A user who buys BTC once a year has a manageable tax record even without dedicated tooling. A user running weekly Auto-DCA, paying [utilities](https://lightningpay.info/pay-utilities-with-bitcoin) or [rent](https://lightningpay.info/pay-rent-with-bitcoin) in BTC, and swapping between BTC and stablecoins periodically generates a transaction volume that's genuinely impractical to reconstruct by hand at tax time. Automatic logging at the moment each transaction occurs avoids the alternative, which is trying to retroactively determine historical USD prices for transactions that happened months earlier.

## Stablecoin transactions still count

It's a common misconception that swapping BTC for a dollar-pegged stablecoin is a tax-neutral event because "it's still dollars." In most jurisdictions, converting BTC to USDC or USDT is a disposal of BTC at its current market value, which can trigger a reportable gain or loss even though the resulting balance is stable going forward. The [stablecoins overview](https://lightningpay.info/stablecoins) and [Bitcoin-stablecoin bridge guide](https://lightningpay.info/stablecoins/bitcoin-stablecoin-bridge) describe the mechanics of that swap; the tax assistant is what turns the mechanics into a basis record.

## What the tool does not do

The tax assistant produces a transaction-level record with cost basis and proceeds — it is not a substitute for filing software, and it does not itself calculate or file a tax return. Jurisdictional rules on holding periods, allowable methods, and reporting thresholds vary enough that the output is best treated as an input to a tax professional or filing software, not a final answer. This article, and the tool itself, are informational and not tax advice.

## Exporting records

For anyone working with an accountant or tax software, having a clean, exportable transaction history — rather than needing to manually pull dates and prices from a block explorer — is generally the most time-consuming part of crypto tax preparation to avoid doing by hand. The [FAQ](https://lightningpay.info/faq) covers export format and history availability in more detail.

## Related articles

- [Automating Bitcoin Purchases with Auto-DCA](automating-bitcoin-purchases-with-auto-dca.md)
- [Stablecoins in Your Wallet: USDC vs USDT](stablecoins-usdc-vs-usdt-in-your-wallet.md)
- [Paying Everyday Bills with Bitcoin](paying-everyday-bills-with-bitcoin.md)
- [Non-Custodial Security, Explained](non-custodial-security-explained.md)
