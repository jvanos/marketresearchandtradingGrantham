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

## Jul 30 — EOD Snapshot (Day 19, Thursday)
**Portfolio:** $49,777.50 | **Cash:** $12,521.42 (25.2%) | **Day P&L:** +$661.09 (+1.35%) | **Phase P&L:** -$222.50 (-0.45%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $29.30 | -0.41% | +$490.71 (+8.24%) | $27.51 (10% trail) |
| GDX | 82 | $76.97 | $76.35 | +3.77% | -$51.18 (-0.81%) | $70.19 (10% trail) |
| GLDM | 90 | $82.65 | $81.37 | +1.68% | -$115.81 (-1.56%) | $74.42 (10% trail) |
| IEFA | 56 | $97.18 | $98.86 | +2.73% | +$94.08 (+1.73%) | $89.03 (10% trail) |
| SCHP | 240 | $26.19 | $26.13 | -0.04% | -$14.40 (-0.23%) | $23.58 (10% trail) |
| VWO | 93 | $59.06 | $58.27 | +2.36% | -$73.94 (-1.35%) | $53.68 (10% trail) |

**Notes:** Strong rebound day (+$661, +1.35%), no new trades — same six positions since Jul 22, all GTC 10% trailing stops intact and none near triggering. GDX, GLDM, IEFA, and VWO all bounced 1.7-3.8% intraday, flipping IEFA back to a small unrealized gain; DBC remains the book's biggest winner (+8.24%). IEFA's trail ratcheted up to $89.03 (from $87.92) as the price climbed, exactly as designed. **Data-integrity note:** no Jul 29 (Wednesday) EOD entry exists in this log — Alpaca's `last_equity` (49,122.26, balance_asof Jul 29) implies a trading day occurred between the Jul 28 and Jul 30 snapshots with no commit landing, the third such gap this phase. Day P&L above is computed against the Jul 28 snapshot per protocol (comparison window one day wider); Alpaca-native Day P&L (vs. last_equity) would be +$655.24 (+1.33%). Recommend investigating why the Jul 29 session's Step 6 push did not land — this is a recurring pattern (Jul 6-23, then Jul 27, now Jul 29) worth root-causing rather than continuing to patch around.
