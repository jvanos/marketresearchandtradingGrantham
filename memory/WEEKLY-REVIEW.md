# Weekly Review

Friday reviews appended here.
Template for each entry:

## Week ending YYYY-MM-DD

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $X |
| Ending portfolio | $X |
| Week return | ±$X (±X%) |
| S&P 500 week | ±X% |
| Bot vs S&P | ±X% |
| Trades | N (W:X / L:Y / open:Z) |
| Win rate | X% |
| Best trade | SYM +X% |
| Worst trade | SYM -X% |
| Profit factor | X.XX |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |

### What Worked
- ...

### What Didn't Work
- ...

### Key Lessons
- ...

### Adjustments for Next Week
- ...

### Proposed Strategy Changes
(Optional — see TRADING-STRATEGY.md "Enforcement note". Propose changes
here for human review; do not edit TRADING-STRATEGY.md directly.)

### Overall Grade: X

## Week ending 2026-10-24

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $80,000 (Alpaca last_equity at account creation Oct 21; no Monday baseline exists) |
| Ending portfolio | $79,228.81 |
| Week return | -$771.19 (-0.96%) |
| S&P 500 week | -0.47% (7,623.68) |
| Bot vs S&P | -0.49% |
| Trades | 0 by bot (W:0 / L:0 / open:28 inherited) |
| Win rate | n/a (no closed trades) |
| Best trade | n/a — best open: REZ +1.99% |
| Worst trade | n/a — worst open: WULF -12.65% |
| Profit factor | n/a |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| none | | | | No orders this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| GLDM | $81.69 | $79.13 | -$307.20 (-3.13%) | none |
| SIVR | $54.85 | $51.22 | -$116.16 (-6.62%) | none |
| AMZN | $262.62 | $248.00 | -$87.72 (-5.57%) | none |
| GOOGL | $334.31 | $320.21 | -$56.60 (-4.22%) | none |
| BTC | $37.36 | $35.89 | -$51.45 (-3.94%) | none |
| SOXX | $511.15 | $478.20 | -$32.95 (-6.45%) | none |
| SMH | $557.03 | $527.20 | -$29.83 (-5.36%) | none |
| HODL | $23.89 | $22.96 | -$27.90 (-3.89%) | none |
| VOO | $710.69 | $698.58 | -$25.75 (-1.70%) | none |
| SPMO | $143.30 | $138.66 | -$23.24 (-3.24%) | none |
| VTI | $379.19 | $373.01 | -$18.54 (-1.63%) | none |
| WULF | $12.96 | $11.32 | -$16.40 (-12.65%) | none |
| VGK | $87.55 | $86.25 | -$15.95 (-1.49%) | none |
| WQTM | $28.58 | $27.28 | -$13.00 (-4.55%) | none |
| QQQM | $298.95 | $290.06 | -$13.34 (-2.97%) | none |
| VGT | $122.33 | $119.17 | -$12.64 (-2.58%) | none |
| FLJP | $40.73 | $40.10 | -$6.93 (-1.55%) | none |
| EWG | $41.72 | $40.94 | -$3.90 (-1.87%) | none |
| XLI | $167.99 | $164.62 | -$3.37 (-2.01%) | none |
| SCHG | $35.88 | $34.82 | -$3.18 (-2.95%) | none |
| SCHD | $34.62 | $35.27 | +$63.17 (+1.88%) | none |
| AAPL | $344.27 | $347.73 | +$20.76 (+1.00%) | none |
| VTV | $224.72 | $225.05 | +$4.28 (+0.15%) | none |
| REZ | $89.76 | $91.55 | +$1.79 (+1.99%) | none |
| XLE | $68.21 | $69.33 | +$1.12 (+1.64%) | none |
| BRK.B | $541.97 | $542.19 | +$2.86 (+0.04%) | none |
| SGOV | $100.62 | $100.66 | +$0.40 (+0.04%) | none |
| COWZ | $70.81 | $71.08 | +$0.27 (+0.38%) | none |
| VNQI | $42.69 | $42.71 | +$0.02 (+0.05%) | none |
| XLB | $51.27 | $51.31 | +$0.20 (+0.08%) | none |

Cash $38,772 (48.9%); 30 positions listed above incl. fractional lots; zero open orders.

### What Worked
- Nothing traded, so no execution losses; cash ~49% cushioned the drawdown.
- Non-US/Europe sleeve (VGK, EWG, FLJP) held within -2%.
- Income/value ETFs (SCHD, VTV) positive.

### What Didn't Work
- Book is not Grantham-compliant: US mega-caps (AAPL, AMZN, GOOGL, BRK.B), US index ETFs (VOO, VTI, QQQM), semis (SMH/SOXX), crypto-linked (BTC, HODL, WULF).
- Zero stop orders on any position — rule 5 violated across the board.
- Trailing rules unenforceable; SOXX (-6.5%), SIVR (-6.6%), WULF (-12.7%) at/through the -7% cut line.
- Gold/silver fell (gold ~$4,010, -$50 Fri) — GLDM/SIVR dragged; oil spiked (Brent $116) with no commodity energy exposure beyond 1 XLE share.
- Underperformed S&P by 0.49%.

### Key Lessons
- Account PA3Q1U9Y8 (created Oct 21, $80k) is NOT the tracked $50k account; strategy/log baseline is stale (last entry Jul 28). Human must confirm intended keys/universe.
- Without stops, an overnight gap is unhedged; the bot has not placed any protective orders.
- Prior memory-gap pattern (missing commits) persists; `scripts/memory.sh` referenced by routine does not exist in repo (read memory files directly this week).

### Adjustments for Next Week
- HUMAN DECISION NEEDED: liquidate/keep non-compliant holdings (US stocks, US ETFs, crypto-linked)?
- Do not auto-trade the inherited book until confirmed. If keeping, place 10% GTC trails and cut WULF (-12.7%) per -7% rule.
- Reset baseline for phase P&L to $80,000 / Oct 21.
- Fix/restore `scripts/memory.sh` or update routines/weekly-review.md.

### Proposed Strategy Changes
- None to rules. Housekeeping: update TRADING-STRATEGY.md starting capital (~$80k) and PROJECT-CONTEXT once the human confirms the account; align the routine's universe text (CLAUDE.md says Grantham-only, scheduled prompt says any liquid US stock/ETF) — human to decide which governs.

### Overall Grade: C-
(No trades; unprotected, out-of-universe book; -0.96% vs S&P -0.47%.)

## Week ending 2026-10-30

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $79,228.81 (Oct 24 close; Monday AM baseline) |
| Ending portfolio | $78,795.84 |
| Week return | -$432.97 (-0.55%) |
| S&P 500 week | -0.5% (7,630.07) |
| Bot vs S&P | ~-0.05% (in line) |
| Trades | 15 exits, 0 buys (W:0 / L:15 / open:17) — approx; most stop-out fills not logged |
| Win rate | 0% (closed trades) |
| Best trade | n/a — all exits losers; best open: SCHD +3.41% |
| Worst trade | GOOGL ~-13% (stop gap Oct 29); WULF absent, exit never logged |
| Profit factor | 0.00 (no winners closed) |
| Phase P&L | -$1,204 (-1.51% vs $80k Oct 21) |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| SIVR 32 | $54.85 | ~$50.96 | ~-$124 (-7.1%) | Oct 28 manual -7% cut |
| GOOGL ~4 | $334.31 | ~$290 / $284.51 | ~-$180 (-13%/-14.9%) | Oct 29 trail gapped at open; remnant cut |
| AMZN 7 | $262.62 | $232.02 | -$214 (-11.7%) | Oct 30 stop post-earnings (stop added only Oct 29) |
| BTC 35 | $37.36 | $34.06 | -$116 (-8.8%) | Oct 30 manual market sell |
| SMH, SOXX, VGT 4, SCHG 3 | various | n/a | losses (fills not logged) | Oct 30 trail stops, tech/semis selloff |
| GLDM 120, HODL 30, QQQM 1, SPMO 5 | various | n/a | losses (fills not logged) | Oct 30 trail stops |
| WULF | $12.96 | n/a | n/a | gone by Oct 29, exit never logged |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| SCHD 97.18 | $34.62 | $35.80 | +$114.67 (+3.41%) | $34.65 |
| VTV 13 | $224.72 | $228.02 | +$42.89 (+1.47%) | $219.75 |
| XLB 5 | $51.27 | $52.63 | +$6.80 (+2.65%) | $50.67 |
| XLE 1 | $68.21 | $69.96 | +$1.75 (+2.57%) | $67.34 |
| BRK.B 13 | $541.97 | $542.79 | +$10.66 (+0.15%) | $533.96 |
| AAPL 6.01 | $344.27 | $344.67 | +$2.42 (+0.12%) | $333.86 |
| VGK 12.27 | $87.55 | $87.67 | +$1.47 (+0.14%) | $84.27 |
| COWZ 1 / SGOV 10 / VNQI 1 / EWG 5 | — | — | ~+$0 to +$1 | trailing |
| XLI 1 | $167.99 | $167.70 | -$0.29 (-0.17%) | $161.86 |
| FLJP 11 | $40.73 | $39.59 | -$12.54 (-2.80%) | $38.93 |
| VTI 3 | $379.19 | $371.82 | -$22.11 (-1.94%) | $364.48 |
| VOO 2.13 | $710.69 | $695.01 | -$33.34 (-2.21%) | $677.43 |
| QQQM 0.5 / SPMO 0.008 | — | — | -$7.27 / -$0.05 | none (fractional remnants) |

Cash $57,145.97 (72.5%); 17 positions.

### What Worked
- Trailing stops (added Oct 27-29) exited semis/tech/crypto-linked before the Oct 30 rout deepened.
- Cash rose to 72.5%; week loss (-0.55%) matched the S&P (-0.5%).
- -7% cut rule applied on SIVR (Oct 28) and BTC.
- Value/dividend ETFs (SCHD, VTV) and XLB/XLE green.

### What Didn't Work
- 15 exits, 0 winners; every closed trade a loss — inherited book was concentrated in tech/semis/crypto-linked.
- AMZN held into earnings with no stop until Oct 29 (-11.7%); GOOGL gapped through its trail (-13%).
- Exit logging gaps: WULF, most Oct 30 fills unrecorded; fractional remnants (QQQM, SPMO) left without stops.
- Only ~27.5% deployed vs 75-85% target; no new buys all week (0 of 8).
- Book still out-of-universe per CLAUDE.md (US stocks/ETFs held).

### Key Lessons
- Trailing stops don't protect against earnings gaps — de-risk or size down before earnings.
- Fractional remnants after partial stop fills need immediate close; log every fill.
- Underdeployment is now the main drag/risk; patience is fine but needs a defined re-entry plan.
- `scripts/memory.sh` still missing (again read memory files directly).

### Adjustments for Next Week
- Close QQQM/SPMO remnants Monday.
- Human decision pending: universe (Grantham-only vs any liquid US stock/ETF) and whether to liquidate US-index holdings.
- If deploying: follow momentum in intl equities/commodities/TIPS with research-backed thesis; stops on every fill.
- Log all stop-out fills with prices (use order history).

### Proposed Strategy Changes
- None to rules. Housekeeping (human): reconcile CLAUDE.md universe vs scheduled prompt; restore scripts/memory.sh or update routine; update starting capital to ~$80k.

### Overall Grade: D+
(-0.55% ≈ S&P, but 0 winners, large gap losses, 27.5% deployed, no buys.)
