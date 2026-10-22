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

## Oct 21 — EOD Snapshot (Day N/A, Wednesday)
**Portfolio:** $80,025.45 | **Cash:** $38,772.20 (48.5%) | **Day P&L:** +$25.45 (+0.03%, vs Alpaca last_equity $80,000) | **Phase P&L:** n/a (baseline not comparable)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| AAPL | 6.0089 | $344.27 | $344.21 | +1.39% | -0.36 (-0.02%) | none |
| AMZN | 6 | $262.62 | $262.93 | +0.11% | +1.86 (+0.12%) | none |
| BRK.B | 13 | $541.97 | $542.04 | +0.41% | +0.91 (+0.01%) | none |
| BTC | 35 | $37.36 | $37.36 | +2.41% | +0.00 (+0.00%) | none |
| COWZ | 1 | $70.81 | $70.93 | -0.21% | +0.12 (+0.17%) | none |
| EWG | 5 | $41.72 | $41.75 | +0.77% | +0.15 (+0.07%) | none |
| FLJP | 11 | $40.73 | $40.74 | +0.29% | +0.11 (+0.03%) | none |
| GLDM | 120 | $81.69 | $81.75 | +0.33% | +7.20 (+0.07%) | none |
| GOOGL | 4.0133 | $334.31 | $335.00 | -1.55% | +2.74 (+0.20%) | none |
| HODL | 30 | $23.89 | $23.89 | +2.40% | +0.03 (+0.00%) | none |
| QQQM | 1.5 | $298.95 | $298.87 | +1.11% | -0.12 (-0.03%) | none |
| REZ | 1 | $89.76 | $89.54 | -1.17% | -0.22 (-0.24%) | none |
| SCHD | 97.1816 | $34.62 | $34.68 | -0.04% | +5.45 (+0.16%) | none |
| SCHG | 3 | $35.88 | $35.88 | +0.98% | +0.00 (+0.00%) | none |
| SGOV | 10 | $100.62 | $100.61 | +0.01% | -0.05 (-0.01%) | none |
| SIVR | 32 | $54.85 | $54.98 | +0.27% | +4.16 (+0.24%) | none |
| SMH | 1 | $557.03 | $556.44 | +1.85% | -0.59 (-0.11%) | none |
| SOXX | 1 | $511.15 | $510.08 | +2.01% | -1.07 (-0.21%) | none |
| SPMO | 5.008 | $143.30 | $143.26 | +0.92% | -0.20 (-0.03%) | none |
| VGK | 12.2667 | $87.55 | $87.58 | +0.46% | +0.37 (+0.03%) | none |
| VGT | 4 | $122.33 | $122.31 | +1.75% | -0.10 (-0.02%) | none |
| VNQI | 1 | $42.69 | $42.67 | -0.16% | -0.02 (-0.05%) | none |
| VOO | 2.1264 | $710.69 | $710.99 | +0.59% | +0.64 (+0.04%) | none |
| VTI | 3 | $379.19 | $379.38 | +0.61% | +0.57 (+0.05%) | none |
| VTV | 13 | $224.72 | $225.02 | +0.23% | +3.89 (+0.13%) | none |
| WQTM | 10 | $28.58 | $28.56 | +2.18% | -0.20 (-0.07%) | none |
| WULF | 10 | $12.96 | $12.79 | +6.49% | -1.70 (-1.31%) | none |
| XLB | 5 | $51.27 | $51.30 | +0.15% | +0.17 (+0.07%) | none |
| XLE | 1 | $68.21 | $68.20 | +0.35% | -0.01 (-0.01%) | none |
| XLI | 1 | $167.99 | $168.27 | +0.88% | +0.28 (+0.17%) | none |
**Notes:** Snapshot taken ~3:55pm ET pre-close. **ACCOUNT ANOMALY:** Alpaca account PA3Q1U9Y8 was created 2026-10-21 with $80,000 start equity — not the $50k account tracked in this log (last entry Jul 28; prior DBC/GDX/GLDM/IEFA/SCHP/VWO book is gone). It holds 28 positions incl. US stocks (AAPL, AMZN, BRK.B, GOOGL), US ETFs (VOO, VTI, SCHD, QQQM), crypto-linked (BTC, HODL, WULF) — outside Grantham universe — and has no stop orders. No trades by this bot today. Day P&L uses Alpaca last_equity; Phase P&L vs $50k Day 0 baseline is not meaningful. Human review needed: confirm intended account/keys, universe, and whether to liquidate non-compliant holdings.

## Oct 22 — EOD Snapshot (Day N/A, Thursday)
**Portfolio:** $79,462.38 | **Cash:** $38,772.19 (48.8%) | **Day P&L:** -$563.07 (-0.70%, vs Oct 21 snapshot; Alpaca last_equity basis -$515.25 / -0.64%) | **Phase P&L:** n/a (baseline not comparable)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| AAPL | 6.0089 | $344.27 | $347.86 | +1.12% | +21.57 (+1.04%) | none |
| AMZN | 6 | $262.62 | $250.64 | -4.47% | -71.88 (-4.56%) | none |
| BRK.B | 13 | $541.97 | $547.03 | +1.49% | +65.78 (+0.93%) | none |
| BTC | 35 | $37.36 | $35.97 | -3.69% | -48.65 (-3.72%) | none |
| COWZ | 1 | $70.81 | $71.78 | +1.27% | +0.97 (+1.37%) | none |
| EWG | 5 | $41.72 | $41.35 | -0.84% | -1.85 (-0.89%) | none |
| FLJP | 11 | $40.73 | $40.28 | -1.08% | -4.95 (-1.10%) | none |
| GLDM | 120 | $81.69 | $79.66 | -2.60% | -243.60 (-2.48%) | none |
| GOOGL | 4.0133 | $334.31 | $324.22 | -3.15% | -40.50 (-3.02%) | none |
| HODL | 30 | $23.89 | $23.00 | -3.72% | -26.70 (-3.72%) | none |
| QQQM | 1.5 | $298.95 | $290.16 | -2.84% | -13.19 (-2.94%) | none |
| REZ | 1 | $89.76 | $91.74 | +2.53% | +1.98 (+2.21%) | none |
| SCHD | 97.1816 | $34.62 | $35.35 | +2.00% | +71.17 (+2.11%) | none |
| SCHG | 3 | $35.88 | $34.96 | -2.51% | -2.76 (-2.56%) | none |
| SGOV | 10 | $100.62 | $100.62 | +0.00% | +0.01 (+0.00%) | none |
| SIVR | 32 | $54.85 | $51.84 | -5.68% | -96.32 (-5.49%) | none |
| SMH | 1 | $557.03 | $524.40 | -5.80% | -32.63 (-5.86%) | none |
| SOXX | 1 | $511.15 | $476.48 | -6.64% | -34.67 (-6.78%) | none |
| SPMO | 5.008 | $143.30 | $138.82 | -3.02% | -22.44 (-3.13%) | none |
| VGK | 12.2667 | $87.55 | $86.80 | -0.89% | -9.20 (-0.86%) | none |
| VGT | 4 | $122.33 | $118.88 | -2.76% | -13.80 (-2.82%) | none |
| VNQI | 1 | $42.69 | $42.71 | +0.09% | +0.02 (+0.05%) | none |
| VOO | 2.1264 | $710.69 | $702.12 | -1.21% | -18.22 (-1.21%) | none |
| VTI | 3 | $379.19 | $374.90 | -1.12% | -12.87 (-1.13%) | none |
| VTV | 13 | $224.72 | $226.55 | +0.72% | +23.78 (+0.81%) | none |
| WQTM | 10 | $28.58 | $27.35 | -4.37% | -12.30 (-4.30%) | none |
| WULF | 10 | $12.96 | $11.32 | -11.25% | -16.36 (-12.62%) | none |
| XLB | 5 | $51.27 | $51.50 | +0.35% | +1.15 (+0.45%) | none |
| XLE | 1 | $68.21 | $67.57 | -0.87% | -0.64 (-0.94%) | none |
| XLI | 1 | $167.99 | $166.73 | -0.94% | -1.26 (-0.75%) | none |

**Notes:** Risk-off day, -$563 (-0.70%). No trades by this bot; no open orders, still no stops on any position. Same account anomaly as Oct 21 (PA3Q1U9Y8, $80k start, 28 positions incl. US stocks/ETFs and crypto-linked BTC/HODL/WULF, outside Grantham universe; options level 3 enabled). Biggest decliners: SOXX -6.6%, SMH -5.8%, SIVR -5.7%, WULF -11.3%, AMZN -4.5%, GLDM -2.6%. Human review still needed: confirm intended account/keys and whether to liquidate non-compliant holdings.
