# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $50,000.00 | **Cash:** $50,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

## Jul 14 — EOD Snapshot (Day 7, Tuesday)
**Portfolio:** $49,554.59 | **Cash:** $25,118.51 (50.7%) | **Day P&L:** +$143.52 (+0.29%) | **Phase P&L:** -$445.41 (-0.89%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| DBC | 220 | $27.07 | $28.61 | +0.99% | +$338.80 (+5.69%) | $25.848 (trail 10%) |
| GLDM | 90 | $82.651778 | $80.24 | +1.35% | -$217.06 (-2.92%) | $74.421 (trail 10%) |
| IEFA | 56 | $97.18 | $96.89 | +0.77% | -$16.24 (-0.30%) | $87.867 (trail 10%) |
| VWO | 93 | $59.06 | $59.08 | +0.49% | +$1.86 (+0.03%) | $53.325 (trail 10%) |

**Notes:** Bought IEFA (56 sh, non-US developed) and VWO (93 sh, emerging
markets) today, both with 10% GTC trailing stops placed immediately after
fill. All 4 open positions (DBC, GLDM, IEFA, VWO) are Grantham-compliant
(commodities/gold + non-US equity ETFs), no options, no US stocks, no
crypto. 2 buys filled this week (well under the 8/week cap). Day P&L is
sourced from Alpaca's live `last_equity` rather than this log's tail
because the log had no prior EOD snapshot to read from — see the "Log Gap"
note above; this snapshot and today's commit/push restore normal
continuity going forward. Phase P&L vs. the $50,000 Day 0 baseline is
still net negative (-0.89%), driven mainly by the EWY stop-out on 07-13.

## Open Positions

| Date | Ticker | Side | Shares | Entry | Stop | Target | R:R | Thesis |
|---|---|---|---|---|---|---|---|---|
| 2026-07-07 | DBC | BUY | 220 | $27.07 | $25.848 trailing 10% GTC | — | — | Not recorded — log was out of sync (see note below); backfilled from Alpaca order history. |
| 2026-07-07 | GLDM | BUY | 90 | $82.651778 | $74.421 trailing 10% GTC | — | — | Not recorded — log was out of sync (see note below); backfilled from Alpaca order history. |
| 2026-07-14 | IEFA | BUY | 56 | $97.18 | $87.867 trailing 10% GTC | — | — | Non-US developed markets exposure (EAFE core). |
| 2026-07-14 | VWO | BUY | 93 | $59.06 | $53.325 trailing 10% GTC | — | — | Emerging markets exposure. |

## Closed Positions

| Date | Ticker | Side | Shares | Entry | Exit | P&L | Notes |
|---|---|---|---|---|---|---|---|
| 2026-07-07 → 2026-07-13 | EWY | BUY→SELL | 41 | $181.806829 | $168.325366 | -$552.74 (-7.42%) | Cut per -7% loser rule; not logged at the time (see gap note below). |

## Log Gap — 2026-07-03 to 2026-07-14

The 2026-07-03 pivot commit reset this file to the Day 0 baseline and no
EOD snapshot or trade entry was appended for 8 trading days afterward
(DBC/GLDM entries on 07-07, EWY round-trip 07-07→07-13, IEFA/VWO entries
today) — routines ran and traded live but their commits/pushes never
landed. Rows above are backfilled from Alpaca's live order history, which
is authoritative; thesis text for the 07-07 entries was not preserved
anywhere and could not be recovered. Today's snapshot restores continuity;
see EOD entry below for current Day P&L sourcing.
