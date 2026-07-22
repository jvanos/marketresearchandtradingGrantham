# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $50,000.00 | **Cash:** $50,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

### Jul 22 — EOD Snapshot (Day 13, Wednesday)
**Portfolio:** $49,936.34 | **Cash:** $12,521.43 (25.1%) | **Day P&L:** +$137.14 (+0.28%) | **Phase P&L:** -$63.66 (-0.13%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $29.86 | +0.98% | +$613.80 | $26.96 |
| GDX | 82 | $76.97 | $76.90 | +3.65% | -$5.67 | $70.19 |
| GLDM | 90 | $82.65 | $81.77 | +1.18% | -$79.36 | $74.42 |
| IEFA | 56 | $97.18 | $97.08 | +0.17% | -$5.60 | $87.92 |
| SCHP | 240 | $26.19 | $26.15 | -0.13% | -$10.80 | $23.57 |
| VWO | 93 | $59.06 | $58.81 | -0.09% | -$23.25 | $53.68 |

**Notes:** Bought GDX (82sh @ $76.97) and SCHP (240sh @ $26.19) today, both with 10% GTC trailing stops attached immediately after fill. Portfolio essentially flat on the day (+0.28%) and roughly flat since launch (-0.13%), with commodities (DBC) the standout winner (+10.3% unrealized) offsetting small drawdowns in gold miners, gold, TIPS, and EM/intl equities. Deployed capital is 74.9%, just under the 75-85% target band. **Logging gap:** no EOD snapshots or commits were made between the Jul 3 Grantham pivot and today, even though the account traded live throughout — GLDM/DBC/EWY bought Jul 7, EWY stopped out -7.4% Jul 13, IEFA/VWO bought Jul 14. This entry reconstructs current state from live Alpaca data; the Jul 7-21 EOD history was never captured and can't be recovered. Whatever ran the market-open/midday routines during that window wasn't completing this routine's mandatory commit step — worth checking that daily-summary is actually firing on schedule going forward.

## Open Positions

| Date | Ticker | Side | Shares | Entry | Stop | Target | R:R | Thesis |
|---|---|---|---|---|---|---|---|---|
