# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $50,000.00 | **Cash:** $50,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

## Open Positions

| Date | Ticker | Side | Shares | Entry | Stop | Target | R:R | Thesis |
|---|---|---|---|---|---|---|---|---|

## Jul 24 — EOD Snapshot (Day 15, Friday)
**Portfolio:** $49,578.40 | **Cash:** $12,521.42 (25.3%) | **Day P&L:** +$4.58 (+0.01%) | **Phase P&L:** -$421.60 (-0.84%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $30.09 | -0.73% | +$664.40 (+11.16%) | $27.51 (10% trail) |
| GDX | 82 | $76.97 | $75.50 | +0.64% | -$120.47 (-1.91%) | $70.19 (10% trail) |
| GLDM | 90 | $82.65 | $80.19 | +0.10% | -$221.56 (-2.98%) | $74.42 (10% trail) |
| IEFA | 56 | $97.18 | $96.33 | +0.60% | -$47.60 (-0.88%) | $87.92 (10% trail) |
| SCHP | 240 | $26.19 | $26.08 | +0.04% | -$26.40 (-0.42%) | $23.57 (10% trail) |
| VWO | 93 | $59.06 | $57.80 | -0.52% | -$117.18 (-2.13%) | $53.68 (10% trail) |

**Notes:** Flat day (+$4.58), no new trades. Six positions carried, all GTC 10% trailing stops in place. DBC is the standout winner (+11.2% unrealized); GDX, GLDM, IEFA, SCHP, VWO are modestly underwater but within normal range, none near their stops. **Data-integrity flag:** this file was last updated Jul 3 (Day 0 baseline) — the mandatory EOD commit/push evidently did not run for 21 days despite live trading (fills on Jul 7, 13, 14, 22 per Alpaca order history: DBC/GLDM/EWY opened Jul 7, EWY round-tripped Jul 13, IEFA/VWO added Jul 14, GDX/SCHP added Jul 22). This snapshot was reconstructed directly from live Alpaca account/positions/orders data. The day-by-day entry/thesis history for Jul 6–23 is not recoverable from this log and needs manual backfill or reconciliation; investigate why prior sessions' Step 6 commits were not landing.

## Jul 28 — EOD Snapshot (Day 17, Tuesday)
**Portfolio:** $49,116.41 | **Cash:** $12,521.42 (25.5%) | **Day P&L:** -$461.99 (-0.93%) | **Phase P&L:** -$883.59 (-1.77%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $28.60 | -1.41% | +$336.60 (+5.65%) | $27.51 (10% trail) |
| GDX | 82 | $76.97 | $74.21 | -2.01% | -$226.25 (-3.59%) | $70.19 (10% trail) |
| GLDM | 90 | $82.65 | $79.61 | -1.44% | -$273.43 (-3.68%) | $74.42 (10% trail) |
| IEFA | 56 | $97.18 | $96.72 | -0.11% | -$25.76 (-0.47%) | $87.92 (10% trail) |
| SCHP | 240 | $26.19 | $26.11 | +0.23% | -$19.20 (-0.31%) | $23.57 (10% trail) |
| VWO | 93 | $59.06 | $57.74 | -0.84% | -$122.76 (-2.24%) | $53.68 (10% trail) |

**Notes:** Broad pullback across the book (-$462, -0.93%), no new trades — still six positions, all unchanged since Jul 24, all GTC 10% trailing stops intact and none near triggering. DBC gave back some of its gain but remains the only winner (+5.65%); GDX and GLDM are the day's biggest laggards (-2% to -3.7% unrealized) but well clear of stops. **Data-integrity note:** no Jul 27 (Monday) EOD entry exists in this log — Alpaca's `last_equity` field (49,473.55) implies a trading day occurred between the Jul 24 and Jul 28 snapshots with no commit landing, echoing the earlier 21-day gap. Day P&L above is computed against the Jul 24 snapshot per protocol (comparison window one day wider); Alpaca-native Day P&L (vs. last_equity) would be -$357.14 (-0.72%). Recommend checking why the Jul 27 run didn't push.

## Aug 03 — EOD Snapshot (Day 21, Monday)
**Portfolio:** $49,554.62 | **Cash:** $12,521.42 (25.3%) | **Day P&L:** +$438.21 (+0.89%) | **Phase P&L:** -$445.38 (-0.89%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $28.90 | -1.87% | +$402.60 (+6.76%) | $27.51 (10% trail) |
| GDX | 82 | $76.97 | $75.99 | +2.55% | -$80.29 (-1.27%) | $70.19 (10% trail) |
| GLDM | 90 | $82.65 | $80.14 | 0.00% | -$226.06 (-3.04%) | $74.42 (10% trail) |
| IEFA | 56 | $97.18 | $98.67 | +0.42% | +$83.16 (+1.53%) | $89.03 (10% trail) |
| SCHP | 240 | $26.19 | $25.89 | -0.77% | -$72.00 (-1.15%) | $23.58 (10% trail) |
| VWO | 93 | $59.06 | $59.06 | +0.53% | $0.00 (0.00%) | $53.68 (10% trail) |

**Notes:** Portfolio bounced +$438 (+0.89%) on a broad rally — GDX led (+2.55%), IEFA and VWO also up; still six positions, unchanged since Jul 24, all GTC 10% trailing stops intact and none near triggering. No new trades; DBC remains the standout winner (+6.76% unrealized), GLDM the biggest laggard (-3.04%) but well clear of its stop. **Data-integrity gap (recurring):** no entries exist in this log for Jul 29, 30, or 31 (Wed–Fri, 3 trading days) — the same missed-commit pattern flagged in the Jul 24 and Jul 28 notes. Positions and stop levels are unchanged from Jul 28 per live Alpaca data, so no trade history was lost, but the day-by-day P&L trail for that window is unrecoverable. Day P&L above is computed against the Jul 28 snapshot per protocol (comparison window 6 days wide instead of 1); Phase P&L is unaffected since it's anchored to the fixed Day 0 baseline. This is the third occurrence of this failure mode — worth a human looking at why Step 6 commits aren't landing on schedule.
