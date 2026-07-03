# Trading Strategy

## Mission
Beat the S&P 500 over the challenge window, trading a Grantham-themed
universe. No options, ever.

## Universe
Eligible:
- Non-US developed and emerging-market equities (regional/country ETFs,
  or individual non-US-domiciled companies)
- Gold, precious metals, and broad commodities (physical/futures-backed
  ETFs, or miners)
- Inflation-protected / TIPS bonds

Excluded, always:
- US-domiciled equities or US total-market/sector funds
- Crypto
- Options or any other derivative

Reference tickers (starting points, NOT exhaustive — anything fitting the
universe above is eligible, use judgment same as any catalyst-driven
pick): VEA, VWO, IEFA, SCHF (intl developed/EM equities) · GLDM, IAU, GDX
(gold/miners) · PDBC, DBC (broad commodities) · SCHP, TIP, VTIP (TIPS)

## Capital & Constraints
- Starting capital: ~$50,000
- Platform: Alpaca (paper trading by default — see env.template)
- Instruments: Stocks/ETFs within the Universe above ONLY

## Core Rules
1. NO OPTIONS — ever (enforced in scripts/alpaca.sh, not just this doc)
2. Grantham universe only — no US-domiciled stocks, no crypto
3. 75-85% deployed
4. Up to 30 positions at a time, max 20% each (position-count and 20% cap
   also enforced in scripts/alpaca.sh)
5. 10% trailing stop on every position as a real GTC order
6. Cut losers at -7% manually
7. Tighten trail: 7% at +15%, 5% at +20%
8. Never within 3% of current price; never move a stop down
9. Max 8 new trades per week (enforced in scripts/alpaca.sh)
10. Follow regional/asset-class momentum (e.g. dollar weakness favoring
    intl equities, real-yield moves favoring TIPS, inflation prints
    favoring commodities)
11. Exit an asset class after 2 consecutive failed trades
12. Patience > activity

## Enforcement note
Rules 1, 4, and 9 above, plus a cost-vs-buying_power check and a
daily-loss circuit breaker, are validated in code inside
`scripts/alpaca.sh` — a BUY order that breaks one of these is rejected
before it reaches Alpaca, regardless of what any prompt or research
output suggests. See CLAUDE.md "Safety Mechanisms" for the full list.
Changing these limits requires a human to edit the wrapper script
directly — they cannot be loosened by editing this file. See
`routines/weekly-review.md` STEP 5.

Rule 2 (Grantham universe) is NOT code-enforced — the wrapper has no
ticker allowlist. Theme fit is a research/judgment call made each
session, the same trust model used for catalyst/entry quality generally.

## Entry Checklist
- Fits the Universe above (non-US equity, gold/metals/commodities, or
  TIPS) — and NOT a US-domiciled stock
- Specific catalyst?
- Asset-class/regional momentum in favor?
- Stop level (7-10% below entry)
- Target (min 2:1 R:R)
