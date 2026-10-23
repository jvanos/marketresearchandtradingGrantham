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

## Week ending 2026-10-23

**Data caveats:** `scripts/memory.sh` is missing from this repo (archive/read steps skipped; logs read directly). Account PA3Q1U9Y8 was created Wed Oct 21 with $80,000 — no Monday baseline exists; Week return uses $80,000 start. `GITHUB_REPO` env var unset. Account holds out-of-universe positions and no stops (see Oct 21 TRADE-LOG anomaly) — unresolved.

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $80,000.00 (account open, Oct 21) |
| Ending portfolio | $79,252.59 |
| Week return | -$747.41 (-0.93%) |
| S&P 500 week | ~-0.5% (7,623.68 close) |
| Bot vs S&P | ~-0.4% |
| Trades | 0 (W:0 / L:0 / open:28) |
| Win rate | n/a |
| Best trade | n/a (best open: XLE +1.67%) |
| Worst trade | n/a (worst open: WULF -12.11%) |
| Profit factor | n/a |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| none | | | | |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| GLDM | $81.69 | $79.04 | -$318.00 (-3.24%) | none |
| SIVR | $54.85 | $51.19 | -$117.12 (-6.67%) | none |
| AMZN | $262.62 | $248.50 | -$84.69 (-5.38%) | none |
| GOOGL | $334.31 | $321.28 | -$52.31 (-3.90%) | none |
| BTC | $37.36 | $35.94 | -$49.70 (-3.80%) | none |
| SOXX | $511.15 | $479.31 | -$31.84 (-6.23%) | none |
| SMH | $557.03 | $527.60 | -$29.43 (-5.28%) | none |
| HODL | $23.89 | $22.97 | -$27.60 (-3.85%) | none |
| SPMO | $143.30 | $138.97 | -$21.68 (-3.02%) | none |
| VOO | $710.69 | $699.66 | -$23.45 (-1.55%) | none |
| VTI | $379.19 | $373.50 | -$17.07 (-1.50%) | none |
| VGK | $87.55 | $86.25 | -$15.95 (-1.49%) | none |
| WULF | $12.96 | $11.39 | -$15.70 (-12.11%) | none |
| WQTM | $28.58 | $27.28 | -$13.00 (-4.55%) | none |
| QQQM | $298.95 | $290.55 | -$12.60 (-2.81%) | none |
| VGT | $122.33 | $119.45 | -$11.53 (-2.36%) | none |
| FLJP | $40.73 | $40.10 | -$6.93 (-1.55%) | none |
| EWG | $41.72 | $40.94 | -$3.90 (-1.87%) | none |
| XLI | $167.99 | $165.00 | -$2.99 (-1.78%) | none |
| SCHG | $35.88 | $34.90 | -$2.94 (-2.73%) | none |
| SCHD | $34.62 | $35.28 | +$64.14 (+1.91%) | none |
| AAPL | $344.27 | $347.57 | +$19.83 (+0.96%) | none |
| VTV | $224.72 | $225.68 | +$12.43 (+0.43%) | none |
| BRK.B | $541.97 | $542.73 | +$9.88 (+0.14%) | none |
| REZ | $89.76 | $91.55 | +$1.79 (+1.99%) | none |
| XLB | $51.27 | $51.50 | +$1.15 (+0.45%) | none |
| XLE | $68.21 | $69.35 | +$1.14 (+1.67%) | none |
| COWZ / SGOV / VNQI | — | — | ~+$0.7 | none |

### What Worked
- No bot trades placed; no new risk added in a down tape.
- ~49% cash ($38.8k) cushioned the drawdown vs a fully invested book.
- SCHD/BRK.B/VTV defensive holdings held flat to up.

### What Didn't Work
- Gold/silver (GLDM, SIVR) were the largest drags (-$435 combined).
- Semis (SOXX/SMH) fell -5% to -6%.
- 0 of 28 positions have a stop order; SIVR (-6.7%) and SOXX (-6.2%) near the -7% cut line; WULF already past it (-12.1%).
- Deployed ~51% vs 75-85% target; book is mostly outside the Grantham universe.

### Key Lessons
- Account/keys changed under the bot (new $80k account, inherited book). Rulebook cannot be applied until a human confirms intended account and universe.

### Adjustments for Next Week
- Human to confirm account, universe, and whether to liquidate non-compliant holdings.
- If account is confirmed: cut WULF (-7% rule), place GTC 10% trailing stops on all kept positions, watch SIVR/SOXX at -7%.
- Restore `scripts/memory.sh` or update routine to stop referencing it.

### Proposed Strategy Changes
- None. Universe in TRADING-STRATEGY.md (Grantham) conflicts with this routine's prompt ("any liquid US-listed stock or ETF"); human should reconcile.

### Overall Grade: C
(No active management; assessed on risk posture — unprotected, off-universe book; return slightly trailed S&P.)
