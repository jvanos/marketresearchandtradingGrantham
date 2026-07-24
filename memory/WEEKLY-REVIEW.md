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

---

## Week ending 2026-07-24

**Market status at review time:** closed (Fri after-hours; next open Mon
2026-07-27 09:30 ET). Producing this review regardless per protocol.

**Data-integrity note (read first):** memory/TRADE-LOG.md and
memory/RESEARCH-LOG.md were not committed by any daily routine between the
Jul 3 Grantham pivot and today — a 21-day gap despite live fills on Jul 7,
13, 14, 22. Today's Jul 24 EOD snapshot was reconstructed from live Alpaca
data, not from daily logs. This is the FIRST entry in this file. Practical
effect on this review: a true Monday-AM starting equity for this week was
never snapshotted and cannot be recovered from the Alpaca API (no
portfolio-history endpoint exposed by scripts/alpaca.sh, and per-symbol
quotes only return latest, not historical). Figures below use the Jul 3
relaunch ($50,000) as the reliable baseline instead, with the current week's
2 new trades broken out separately since their full lifecycle (entry to
now) falls entirely inside this week. **Root cause of the commit gap is
unconfirmed and needs investigation** — flagging for the human operator.

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | Not recoverable (see data-integrity note) — using Jul 3 relaunch baseline of $50,000.00 |
| Ending portfolio | $49,610.39 (Fri Jul 24, live) |
| Week return | Not computable in isolation (see note) |
| Phase return (since Jul 3) | -$389.61 (-0.78%) |
| S&P 500 week | Conflicting source data (see note) — Investopedia (dated 7/24) put indexes down ~0.7-1.5% entering Friday; another source claimed +1.76%, but its own date metadata pointed to early July, not this week. Treating as unreliable rather than reporting a false-precision number. |
| Bot vs S&P | Not computable given the above (both sides uncertain) |
| Trades | 2 (W:0 / L:0 / open:2) — both still-open buys, no closes this week |
| Win rate | N/A — no closed trades this week |
| Best trade | DBC +11.19% unrealized (opened Jul 7, held) |
| Worst trade | GLDM -3.16% unrealized (opened Jul 7, held) |
| Profit factor | N/A — no closed trades this week |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|--------|-------|------|-----|-------|
| — none — | | | | No positions closed this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|--------|-------|-------|------------|------|
| DBC | $27.07 | $30.10 | +$666.60 (+11.19%) | $27.51 (10% trail) |
| GDX | $76.97 | $75.40 | -$128.67 (-2.04%) | $70.19 (10% trail) |
| GLDM | $82.65 | $80.04 | -$234.92 (-3.16%) | $74.42 (10% trail) |
| IEFA | $97.18 | $96.34 | -$47.04 (-0.86%) | $87.92 (10% trail) |
| SCHP | $26.19 | $26.11 | -$20.26 (-0.32%) | $23.57 (10% trail) |
| VWO | $59.06 | $58.28 | -$72.54 (-1.32%) | $53.68 (10% trail) |

Cash: $12,521.42 (25.3% of equity) — within the 75-85% deployed target
(currently ~75% deployed, at the low edge).

### What Worked
- Both new adds this week (GDX, SCHP) stayed inside the 8-trades/week and
  20%-per-position caps with no wrapper rejections.
- DBC remains the standout — +11.19% unrealized, GTC trailing stop never
  moved down, tightening schedule (7% at +15%) not yet triggered but close.
- No rule violations detected: no options, no US-domiciled stocks, no
  crypto, all 6 holdings fit the Grantham universe.
- Deployment (~75%) sits inside the 75-85% target band.

### What Didn't Work
- 4 of 6 positions are underwater (GDX, GLDM, IEFA, VWO), all modestly
  (-0.3% to -3.2%) — broad-based softness across gold/miners, TIPS, and
  EM/intl equities this week rather than one bad pick.
- Zero closed trades this week means zero realized data to grade
  entry/exit quality against — everything is still a live bet.
- GLDM is the weakest position (-3.16%) and getting closer to the
  -7% manual-cut line without yet being near it.
- **The daily logging pipeline silently failed for 3 weeks.** Whatever
  ran pre-market/market-open/midday/daily-summary during that window
  either didn't run its commit step or the commits didn't land — this
  is a bigger process failure than any single trade this week.

### Key Lessons
- Live trades happened for weeks with no auditable daily trail; the only
  reason this week's positions could be reconstructed at all is that
  Alpaca itself retains order/position history — the memory files did
  not do their job as a durable record.
- Can't yet tell if the GDX/SCHP entries this week were well-timed since
  there's no research-log entry from Jul 22 explaining the catalyst for
  either.

### Adjustments for Next Week
- **Priority: confirm the daily routines actually commit+push at end of
  run.** Add a check at the start of Friday's review (or better, at the
  start of every routine) that fails loudly if the prior day's log entry
  is missing, instead of silently discovering a 3-week gap.
- Watch GLDM for the -7% manual cut line and DBC for the +15%
  trail-tighten trigger (7%).
- Backfill Jul 6-23 research/trade narrative from Alpaca order history
  where possible, clearly marked as reconstructed, so future weekly
  reviews aren't working from a blank log.

### Proposed Strategy Changes
None this week. The open issue is operational (logging/commit reliability
enforced by CLAUDE.md's "Persistence" requirement, not currently
code-enforced), not a trading-rule change — no proposal needed for
TRADING-STRATEGY.md or scripts/alpaca.sh.

### Overall Grade: C

Trade discipline and universe compliance were clean this week, but grading
is capped by a hard fact: for the first review of this bot, there is
effectively no committed intra-week record to grade against. A 21-day gap
in mandatory daily logging is a process failure serious enough to offset
otherwise-reasonable trade selection.