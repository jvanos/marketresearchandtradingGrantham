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

## Jul 27 — EOD Snapshot (Day 16, Monday)
**Portfolio:** $49,484.77 | **Cash:** $12,521.42 (25.3%) | **Day P&L:** -$93.63 (-0.19%) | **Phase P&L:** -$515.23 (-1.03%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $29.02 | -3.59% | +$429.00 (+7.20%) | $27.51 (10% trail) |
| GDX | 82 | $76.97 | $75.84 | +0.81% | -$92.59 (-1.47%) | $70.19 (10% trail) |
| GLDM | 90 | $82.65 | $80.78 | +0.74% | -$168.46 (-2.27%) | $74.42 (10% trail) |
| IEFA | 56 | $97.18 | $96.83 | +0.51% | -$19.60 (-0.36%) | $87.92 (10% trail) |
| SCHP | 240 | $26.19 | $26.05 | -0.15% | -$33.60 (-0.53%) | $23.57 (10% trail) |
| VWO | 93 | $59.06 | $58.23 | +0.74% | -$77.19 (-1.41%) | $53.68 (10% trail) |

**Notes:** Market was closed today (`alpaca.sh clock` returned `is_open: false`, next open Jul 28 09:30 ET) — no trades placed, no orders changed. All six positions and their GTC 10% trailing stops carried unchanged from Friday. Marks shown reflect Alpaca's latest available quotes as of this run, not a live Jul 27 session close. Portfolio down modestly (-$93.63 day, -1.03% phase-to-date); no position near its stop. Zero trades this week so far (Mon–today).
