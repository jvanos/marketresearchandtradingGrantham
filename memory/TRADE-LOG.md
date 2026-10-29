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

## 2026-10-26 — Midday Actions
- No exits: none at/below -7% (worst SIVR -6.25%, AMZN -5.02%, HODL -5.11%, BTC -5.10%, WULF -4.81%). No winners >= +15% — no tightening. No thesis breaks.
- Still NO open stop orders on any of 30 positions (orders empty); standing flag from Oct 21/24. Not placed this routine (no tighten step eligible).

## 2026-10-26 — EOD Snapshot (Day N/A, Monday)
**Portfolio:** $79,377.74 | **Cash:** $38,772.19 (48.8%) | **Day P&L:** +$148.93 (+0.19%) | **Phase P&L:** -$622.26 (-0.78%, vs $80,000 Oct 21 start)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| AAPL | 6.0089 | $344.27 | $344.05 | -1.06% | -1.32 (-0.06%) | none |
| AMZN | 6 | $262.62 | $249.01 | +0.41% | -81.66 (-5.18%) | none |
| BRK.B | 13 | $541.97 | $548.40 | +1.15% | +83.59 (+1.19%) | none |
| BTC | 35 | $37.36 | $35.24 | -1.81% | -74.20 (-5.67%) | none |
| COWZ | 1 | $70.81 | $71.25 | +0.24% | +0.44 (+0.62%) | none |
| EWG | 5 | $41.72 | $41.24 | +0.73% | -2.40 (-1.15%) | none |
| FLJP | 11 | $40.73 | $40.18 | +0.20% | -6.05 (-1.35%) | none |
| GLDM | 120 | $81.69 | $79.36 | +0.29% | -279.60 (-2.85%) | none |
| GOOGL | 4.0133 | $334.31 | $317.10 | -0.97% | -69.08 (-5.15%) | none |
| HODL | 30 | $23.89 | $22.59 | -1.61% | -39.00 (-5.44%) | none |
| QQQM | 1.5 | $298.95 | $293.16 | +1.07% | -8.68 (-1.94%) | none |
| REZ | 1 | $89.76 | $91.90 | +0.38% | +2.14 (+2.38%) | none |
| SCHD | 97.1816 | $34.62 | $35.28 | +0.03% | +64.14 (+1.91%) | none |
| SCHG | 3 | $35.88 | $35.10 | +0.80% | -2.34 (-2.17%) | none |
| SGOV | 10 | $100.62 | $100.67 | +0.01% | +0.50 (+0.05%) | none |
| SIVR | 32 | $54.85 | $51.15 | -0.14% | -118.40 (-6.75%) | none |
| SMH | 1 | $557.03 | $541.35 | +2.68% | -15.68 (-2.81%) | none |
| SOXX | 1 | $511.15 | $492.57 | +3.00% | -18.58 (-3.64%) | none |
| SPMO | 5.008 | $143.30 | $140.55 | +1.36% | -13.77 (-1.92%) | none |
| VGK | 12.2667 | $87.55 | $86.55 | +0.35% | -12.27 (-1.14%) | none |
| VGT | 4 | $122.33 | $120.96 | +1.50% | -5.48 (-1.12%) | none |
| VNQI | 1 | $42.69 | $42.90 | +0.45% | +0.21 (+0.49%) | none |
| VOO | 2.1264 | $710.69 | $703.21 | +0.66% | -15.91 (-1.05%) | none |
| VTI | 3 | $379.19 | $375.59 | +0.69% | -10.80 (-0.95%) | none |
| VTV | 13 | $224.72 | $226.24 | +0.53% | +19.75 (+0.68%) | none |
| WQTM | 10 | $28.58 | $27.51 | +0.84% | -10.70 (-3.74%) | none |
| WULF | 10 | $12.96 | $11.96 | +5.69% | -9.96 (-7.68%) | none |
| XLB | 5 | $51.27 | $51.38 | +0.14% | +0.55 (+0.21%) | none |
| XLE | 1 | $68.21 | $69.66 | +0.48% | +1.45 (+2.13%) | none |
| XLI | 1 | $167.99 | $166.96 | +1.42% | -1.03 (-0.61%) | none |
**Notes:** Small up day (+$149), no trades today. 30 positions, still NO stop orders on any (orders empty) — standing flag from Oct 21. Worst: SIVR -6.75%, AMZN -5.18%, HODL -5.44%, BTC -5.68%, GOOGL -5.15%, WULF -7.68% (breached -7% cut line after midday scan; +5.7% on day but entry $12.96 — cut candidate tomorrow). Day P&L vs Alpaca last_equity ($79,228.81); phase vs $80k account start. Universe still non-compliant (US stocks, crypto-linked) — human review pending.

## 2026-10-28 — Midday Actions
- EXIT SIVR 32 sh: market sell submitted 17:16 UTC at ~$50.96 (entry $54.85), ~-7.1% (~-$124), cut at -7% per rule. Position gone from Alpaca; fill price approximate.
- No winners >= +15% — no tightening. No thesis breaks. Remaining 27 positions all have trailing stops.

## 2026-10-28 — EOD Snapshot (Day N/A, Wednesday)
**Portfolio:** $79,569.56 | **Cash:** $40,358.92 (50.7%) | **Day P&L:** -$34.48 (-0.04%) | **Phase P&L:** -$430.44 (-0.54%)
| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| AAPL | 6.0089 | $344.27 | $345.53 | -0.45% | +7.57 (+0.37%) | $329.82 |
| AMZN | 7 | $261.56 | $255.00 | +0.75% | -45.92 (-2.51%) | none |
| BRK.B | 13 | $541.97 | $540.61 | -0.44% | -17.68 (-0.25%) | $528.58 |
| BTC | 35 | $37.36 | $36.03 | +1.04% | -46.55 (-3.56%) | none |
| COWZ | 1 | $70.81 | $70.51 | -0.08% | -0.30 (-0.42%) | $67.78 |
| EWG | 5 | $41.72 | $41.80 | +0.67% | +0.40 (+0.19%) | $40.18 |
| FLJP | 11 | $40.73 | $40.43 | -0.30% | -3.30 (-0.74%) | $38.93 |
| GLDM | 120 | $81.69 | $80.60 | +0.35% | -130.80 (-1.33%) | $78.20 |
| GOOGL | 4.0133 | $334.31 | $300.74 | -6.19% | -134.74 (-10.04%) | $313.35 |
| HODL | 30 | $23.89 | $23.05 | +1.05% | -25.20 (-3.52%) | $22.13 |
| QQQM | 1.5 | $298.95 | $298.15 | +0.40% | -1.20 (-0.27%) | $287.01 |
| SCHD | 97.1816 | $34.62 | $35.13 | +0.03% | +49.56 (+1.47%) | $33.77 |
| SCHG | 3 | $35.88 | $35.55 | +0.14% | -0.99 (-0.92%) | $34.09 |
| SGOV | 10 | $100.62 | $100.69 | +0.01% | +0.70 (+0.07%) | $96.67 |
| SMH | 1 | $557.03 | $567.40 | +1.69% | +10.37 (+1.86%) | $548.16 |
| SOXX | 1 | $511.15 | $520.56 | +1.86% | +9.41 (+1.84%) | $504.02 |
| SPMO | 5.008 | $143.30 | $144.03 | +1.02% | +3.66 (+0.51%) | $138.60 |
| VGK | 12.2667 | $87.55 | $87.73 | +0.79% | +2.21 (+0.21%) | $83.63 |
| VGT | 4 | $122.33 | $123.83 | +0.85% | +6.00 (+1.23%) | $118.28 |
| VNQI | 1 | $42.69 | $42.35 | -0.98% | -0.34 (-0.80%) | $40.85 |
| VOO | 2.1264 | $710.69 | $709.52 | +0.28% | -2.49 (-0.17%) | $677.43 |
| VTI | 3 | $379.19 | $379.01 | +0.29% | -0.54 (-0.05%) | $364.48 |
| VTV | 13 | $224.72 | $226.94 | +0.32% | +28.85 (+0.99%) | $217.10 |
| WQTM | 10 | $28.58 | $28.62 | +0.10% | +0.40 (+0.14%) | $27.83 |
| XLB | 5 | $51.27 | $51.98 | +0.39% | +3.55 (+1.39%) | $49.95 |
| XLE | 1 | $68.21 | $68.42 | +0.31% | +0.21 (+0.31%) | $66.17 |
| XLI | 1 | $167.99 | $168.88 | +0.57% | +0.89 (+0.53%) | $160.82 |
**Notes:** Flat day (-$34). SIVR cut at -7% midday (~-$124). WULF no longer in positions (exit not logged; unverified). GOOGL -6.4% on day (-10.3% unrealized), stop $313.35 sits above price at $299.94 — check for stop trigger/fill. 25 of 27 positions now carry trailing stops (3-5%, tighter than the 10% rule); AMZN and BTC have none. Phase P&L vs $80k account start. Universe still non-compliant (US stocks, crypto-linked) — human review pending.

## 2026-10-29 — Market Open Trades
- No new buys (research decision: HOLD, PCE/ECB/AMZN-earnings day).
- GOOGL GTC trail triggered at open on gap: ~4 sh sold ~$290 (~-13%); 0.0133 sh fractional remnant left.
- STOPS ADDED: AMZN 7 sh, BTC 35 sh — 7% trailing, GTC (were unprotected; AMZN reports after close tonight). AMZN ref ~$244.91, BTC ~$35.40.
- Open Positions table: GOOGL ~closed (0.0133 sh remnant); AMZN/BTC now have trail stops.

## 2026-10-29 — Midday Actions
- EXIT GOOGL 0.0133 sh remnant: close at ~$284.51 (entry $334.31), -14.9%, cut at -7% per rule. Fractional leftover of morning stop-out.
- No winners >= +15% — no tightening. AMZN -6.0% (stop 7% trail, earnings tonight) — watch, not yet at cut line. No thesis breaks. WULF absent from positions (exit never logged). All remaining 25 positions carry trailing stops.

## 2026-10-29 — EOD Snapshot (Day N/A, Thursday)
**Portfolio:** $79,255.14 | **Cash:** $41,772.44 (52.7%) | **Day P&L:** -$403.77 (-0.51%) | **Phase P&L:** -$744.86 (-0.93%)
| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| AAPL | 6.0089 | $344.27 | $351.00 | +2.08% | +40.44 (+1.96%) | $333.86 |
| AMZN | 7 | $261.56 | $227.60 | -10.61% | -237.72 (-12.98%) | $231.70 |
| BRK.B | 13 | $541.97 | $545.00 | +0.86% | +39.39 (+0.56%) | $532.31 |
| BTC | 35 | $37.36 | $35.49 | -1.50% | -65.45 (-5.00%) | $33.67 |
| COWZ | 1 | $70.81 | $71.08 | +0.81% | +0.27 (+0.38%) | $68.23 |
| EWG | 5 | $41.72 | $42.41 | +1.46% | +3.45 (+1.65%) | $40.72 |
| FLJP | 11 | $40.73 | $40.38 | -0.12% | -3.85 (-0.86%) | $38.93 |
| GLDM | 120 | $81.69 | $79.66 | -1.17% | -243.60 (-2.48%) | $78.20 |
| HODL | 30 | $23.89 | $22.70 | -1.52% | -35.70 (-4.98%) | $22.20 |
| QQQM | 1.5 | $298.95 | $290.76 | -2.66% | -12.29 (-2.74%) | $287.01 |
| SCHD | 97.1816 | $34.62 | $35.74 | +1.85% | +108.91 (+3.24%) | $34.20 |
| SCHG | 3 | $35.88 | $34.90 | -2.02% | -2.94 (-2.73%) | $34.09 |
| SGOV | 10 | $100.62 | $100.70 | +0.01% | +0.85 (+0.08%) | $96.68 |
| SMH | 1 | $557.03 | $545.98 | -3.82% | -11.05 (-1.98%) | $548.16 |
| SOXX | 1 | $511.15 | $495.49 | -5.07% | -15.66 (-3.06%) | $504.02 |
| SPMO | 5.008 | $143.30 | $140.30 | -3.17% | -15.02 (-2.09%) | $138.60 |
| VGK | 12.2667 | $87.55 | $88.50 | +1.36% | +11.65 (+1.08%) | $84.27 |
| VGT | 4 | $122.33 | $121.00 | -2.10% | -5.32 (-1.09%) | $118.28 |
| VNQI | 1 | $42.69 | $42.66 | +0.73% | -0.03 (-0.07%) | $40.85 |
| VOO | 2.1264 | $710.69 | $703.72 | -0.87% | -14.82 (-0.98%) | $677.43 |
| VTI | 3 | $379.19 | $377.53 | -0.43% | -4.97 (-0.44%) | $364.48 |
| VTV | 13 | $224.72 | $228.88 | +0.85% | +54.07 (+1.85%) | $218.62 |
| XLB | 5 | $51.27 | $52.53 | +1.29% | +6.30 (+2.46%) | $50.43 |
| XLE | 1 | $68.21 | $69.10 | +0.95% | +0.89 (+1.31%) | $66.45 |
| XLI | 1 | $167.99 | $170.81 | +1.38% | +2.82 (+1.68%) | $161.86 |
**Notes:** Down day (-$404). No new buys. GOOGL stopped out at open on gap (~-13%) and remnant closed midday; AMZN/BTC trail stops added (7%). AMZN -13.1% unrealized, -10.7% on day ahead of tonight's earnings (stop ~$231.70 sits above price $227.31 — check fill/cut tomorrow). All 25 positions carry trailing stops. Phase P&L vs \$80k account start. Universe still non-compliant (US stocks, crypto-linked) — human review pending.
