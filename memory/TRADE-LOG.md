# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $50,000.00 | **Cash:** $50,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

## Reconciliation note — 2026-07-22
This log was reset to the Day 0 baseline by the "Pivot strategy" commit
and never backfilled, even though the live account already held 4
positions opened before the pivot. Backfilling below from live Alpaca
data (positions + order history) so the log matches reality. Entry dates
are approximate (inferred from stop-order creation timestamps, since
exact fill dates weren't logged at the time).

## Open Positions

| Date | Ticker | Side | Shares | Entry | Stop | Target | R:R | Thesis |
|---|---|---|---|---|---|---|---|---|
| ~2026-07-07 (backfilled) | DBC | buy | 220 | $27.07 | $26.874 (10% trail, hwm $29.86) | — | — | Broad commodities exposure (backfilled, pre-dates this log entry) |
| ~2026-07-07 (backfilled) | GLDM | buy | 90 | $82.6518 | $74.421 (10% trail, hwm $82.69) | — | — | Gold exposure (backfilled, pre-dates this log entry) |
| ~2026-07-14 (backfilled) | IEFA | buy | 56 | $97.18 | $87.921 (10% trail, hwm $97.69) | — | — | Non-US developed equity exposure (backfilled, pre-dates this log entry) |
| ~2026-07-14 (backfilled) | VWO | buy | 93 | $59.06 | $53.676 (10% trail, hwm $59.64) | — | — | EM equity exposure (backfilled, pre-dates this log entry) |
| 2026-07-22 | SCHP | buy | 240 | $26.19 | $23.5621 (10% trail) | $29.85 | 2:1 | TIPS — oil-driven (Mideast supply fears, WTI ~$84-88/Brent ~$91) inflation-breakeven risk; portfolio had zero TIPS exposure despite it being a core universe bucket |
| 2026-07-22 | GDX | buy | 82 | $76.9691 | $69.30 (10% trail) | $92.14 | 2:1 | Gold miners — momentum continuation on gold strength (~$4,116/oz, +10.2% YTD), miner equity beta as a second vehicle alongside the flat GLDM bullion position |
