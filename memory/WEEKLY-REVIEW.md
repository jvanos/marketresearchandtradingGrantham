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

## Week ending 2026-07-31

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $49,578.40 (Jul 24 EOD — no Jul 27 Monday AM snapshot exists, see note) |
| Ending portfolio | $49,523.43 |
| Week return | -$54.97 (-0.11%) |
| S&P 500 week | -0.6% |
| Bot vs S&P | +0.49% |
| Trades | 0 (W:0 / L:0 / open:6) |
| Win rate | N/A — no closed trades this week |
| Best trade | DBC +8.68% unrealized |
| Worst trade | GDX -3.89% unrealized |
| Profit factor | N/A — no closed trades this week |

**Note on market status:** market closed for the day at time of this review (after 4pm ET Friday) — normal end-of-day, not a holiday closure. HALT file not present.

**Data-integrity note:** TRADE-LOG.md and RESEARCH-LOG.md have no entries for Jul 27, 29, 30, or 31 — only a Jul 28 entry exists for this week. This echoes the 21-day and single-day commit gaps already flagged in the Jul 24 and Jul 28 log entries. Week-end figures above come directly from live `alpaca.sh account`/`positions` calls, not from a chain of daily snapshots. This is now a recurring, multi-week issue — see Key Lessons.

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| — | — | — | — | No trades closed this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| DBC | $27.07 | $29.42 | +$517.00 (+8.68%) | $27.51 (10% trail) |
| GDX | $76.97 | $73.98 | -$245.43 (-3.89%) | $70.19 (10% trail) |
| GLDM | $82.65 | $79.95 | -$243.16 (-3.27%) | $74.42 (10% trail) |
| IEFA | $97.18 | $98.57 | +$77.84 (+1.43%) | $87.92 (10% trail) |
| SCHP | $26.19 | $26.12 | -$16.80 (-0.27%) | $23.57 (10% trail) |
| VWO | $59.06 | $58.92 | -$13.23 (-0.24%) | $53.68 (10% trail) |

### What Worked
- DBC remains the standout winner, now +8.68% unrealized, stop untouched
- All 6 GTC trailing stops stayed live and untriggered all week — no accidental gaps
- No impulsive trades forced despite a quiet, low-catalyst week — patience honored
- Bot beat the S&P 500 by ~0.5pp this week (-0.11% vs -0.6%) despite a broad market pullback

### What Didn't Work
- Zero new trades placed (0 of 8 weekly cap used) — Perplexity research returned generic/non-actionable output, no fresh catalysts surfaced
- GDX and GLDM both still underwater (-3.9%/-3.3%) for a second straight week with no documented thesis re-check
- Deployment still ~74.7% of equity — low end of the 75-85% target band, ~25% cash sitting idle
- TRADE-LOG/RESEARCH-LOG commit gaps continued (Jul 27, 29, 30, 31 missing) — same failure mode flagged the last two entries, still unresolved

### Key Lessons
- The daily EOD commit/push step is failing or being skipped outside the Friday routine on a recurring basis (21-day gap, then 1-day gap, now a 3-day gap) — this needs root-cause investigation (cron misfire, push/permission failure, or routine not firing), not another log note
- Perplexity research has repeatedly come back generic with no live macro prints — query reformulation or a fallback source may be needed before it can reliably drive new trade ideas
- Two consecutive weeks of GDX/GLDM being flat-to-down without a fresh catalyst check risks drifting into "holding on hope" rather than thesis-driven conviction

### Adjustments for Next Week
- Investigate and fix the recurring missing daily-commit issue before relying on TRADE-LOG/RESEARCH-LOG for next Friday's review
- Explicitly re-underwrite GDX and GLDM theses (hold vs. cut) given 2 straight weeks underwater
- Look for a specific catalyst to redeploy idle cash toward the 75-85% deployment band, without forcing a trade absent an edge

### Proposed Strategy Changes
None this week — no rule has been proven out or has failed badly enough over 2+ weeks to warrant a proposal. The recurring commit/logging gap is an infrastructure issue, not a trading-rule issue, and is called out above for human follow-up.

### Overall Grade: C+

Rationale: risk-neutral, disciplined week that modestly beat the S&P (no rule violations, all stops intact, no forced trades) — but a third straight week of an unresolved commit/logging gap is a real process failure that undermines confidence in every other number in this file, and GDX/GLDM are drifting without a documented thesis check.