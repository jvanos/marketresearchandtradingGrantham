# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $50,000.00 | **Cash:** $50,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

## ⚠️ Memory gap: 2026-07-03 to 2026-07-22

No routine committed to `memory/` between the Grantham-universe pivot
(2026-07-03) and this entry (2026-07-23 midday scan). Six positions were
opened and logged in Alpaca during that window with no corresponding
TRADE-LOG/RESEARCH-LOG entries — original catalysts/theses for these
entries are not recoverable from this repo. Rows below are reconstructed
from live Alpaca position/order data only (entry price, size, initial 10%
trailing stop). Human should check why prior routines' git push/commit
step wasn't landing (env: GITHUB_TOKEN/GITHUB_REPO) — see 2026-07-23
midday scan note.

## Open Positions

| Date | Ticker | Side | Shares | Entry | Stop | Target | R:R | Thesis |
|---|---|---|---|---|---|---|---|---|
| 2026-07-07 | DBC | BUY | 220 | $27.07 | 10% trailing GTC, HWM $30.485, stop $27.4365 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |
| 2026-07-07 | GLDM | BUY | 90 | $82.65 | 10% trailing GTC, HWM $82.69, stop $74.421 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |
| 2026-07-14 | IEFA | BUY | 56 | $97.18 | 10% trailing GTC, HWM $97.69, stop $87.921 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |
| 2026-07-14 | VWO | BUY | 93 | $59.06 | 10% trailing GTC, HWM $59.64, stop $53.676 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |
| 2026-07-22 | GDX | BUY | 82 | $76.97 | 10% trailing GTC, HWM $77.99, stop $70.191 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |
| 2026-07-22 | SCHP | BUY | 240 | $26.19 | 10% trailing GTC, HWM $26.1884, stop $23.56956 | n/a | n/a | Not recorded — reconstructed from Alpaca history (see memory-gap note above) |

## 2026-07-23 — Midday Scan

**Equity:** $49,631.68 | **Cash:** $12,521.43 (25.2%) | **Deployed:** 74.8%

Reviewed all 6 open positions vs. -7% cut / +15%,+20% tighten rules:

| Ticker | Unrealized P&L | Action |
|---|---|---|
| DBC | +12.6% | Hold — below +15% tighten threshold |
| GDX | -2.3% | Hold — above -7% cut threshold |
| GLDM | -3.0% | Hold — above -7% cut threshold |
| IEFA | -1.3% | Hold — above -7% cut threshold |
| SCHP | -0.4% | Hold — above -7% cut threshold |
| VWO | -1.5% | Hold — above -7% cut threshold |

No cuts, no stop tightening, no thesis breaks flagged (no thesis on file
to check against — see memory-gap note above). All 6 trailing stops
confirmed live and correctly trailing HWM at 10%. No new buys (day-trading
budget not applicable, no signal). Discovered and documented the
2026-07-03→07-22 memory-log gap this run (see note above).
