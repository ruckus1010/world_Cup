# Betting Log — World Cup Unit System

**Theoretical units only.** Every wager is logged here: moneylines, totals, AND player props. Claude appends a row when a bet is confirmed placed, and fills Result / Payout / Closing Line / CLV when results are reported.

## Column key

- **Market**: `ML` (moneyline / 3-way), `TOTAL` (game over/under), `PROP` (player prop), `PARLAY`/`SGP`, `PROMO` (promo-driven play)
- **Fair %**: devigged fair probability of the selection
- **Edge**: estimated edge vs. fair line (the reason the bet exists)
- **Stake**: units (1u / 2u / 3u tiers)
- **CLV**: closing-line value — did we beat the number that closed? (the real scoreboard)

## Open Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Edge | Stake | Tier | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Alexander Isak 2+ shots on target | +282 (base +225 × 25% boost) | ~31–36% | +0.26 EV/u | 1.00u | Standard | 25% player-SOT boost. Sweden must-win → chase → Isak shot volume. User confident on Isak start. Breakeven +282 = 26.2%, fair well above. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden team total Over 1.5 (away O/U 1.5) | +230 | ~35–47% | +EV | 1.00u | Standard | Got +230 vs planned +202 — better price (entry CLV win). Sweden must score 2+ to advance, cannot rotate. |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Total Over 2.5 | +286 (base +220 × 30% boost) | ~36–44% | +0.29 EV/u | 0.50u | Standard | 30% any-wager boost. Play-in: both chase, esp. Paraguay (must win, GD -2 vs AUS 0). |
| 008 | 2026-06-25 | PAR–AUS | ML + PROMO | Paraguay moneyline (Drawbreaker) | +165 | ~36% | +EV via refund | 1.00u | Standard | Drawbreaker: refunds up to 1.25u bonus bet if match draws. Paraguay must win; high draw equity (~42%) makes refund live. |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay team total Over 1.5 (home O/U 1.5) | +255 | ~34–45% | +EV | 1.00u | Standard | Got +255 vs planned +202 — better price (entry CLV win). Paraguay must win/chase, cannot rotate. |
| 010 | 2026-06-25 | PAR–AUS | SGP/PROMO | 3-leg SGP: Match O2.5 + BTTS Yes + Enciso anytime | +910 (base +700 × 30% boost) | ~10–11.5% | ~0 to +0.08 EV/u | 0.50u | Fun dart | 30% SGP boost. Marginal-EV lottery, sized down to 0.5u. Boost gets to ~breakeven; correlated legs all ride PAR-AUS opening up. User confident on Enciso start. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia TT Over 2.5 | +154 | ~48–53% | 2.00u | **WIN** | +3.08u | TBD | TBD | Final 3-1 Bosnia. Thesis confirmed: Bosnia chased the scoreline for GD/best-third. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 (win by 3+) | +285 | ~38–43% | 0.50u | **LOSS** | −0.50u | TBD | TBD | Final 3-1 — Bosnia won by 2, not 3+. Variance dart, correlated with bet 001. |
| 003 | 2026-06-24 | SCO–BRA | PROP | Vinicius Jr anytime scorer | +110 | ~50–55% | 1.00u | **WIN** | +1.10u | TBD | TBD | Usage shift thesis cashed. Rodrygo & Raphinha absent → Vini sole focal point. Lineup-confirmed start. |
| 004 | 2026-06-24 | MAR–HTI | PROMO/PROP | Brahim Díaz anytime (live @ HT 2-2) | +324 (+270 base × 20% boost) | ~28–34% | 0.50u | **LOSS** | −0.50u | n/a (live) | n/a | Live promo-boosted dart. +EV by the math (true ~31% vs +324 implied 23.6%); landed on the modal outcome (≈69% loss probability). Sound process, variance outcome. |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 10 |
| Win / Loss / Push (settled) | 2 / 2 / 0 |
| Open bets | 6 (Day 2: bets 005–010) |
| Units staked (settled) | 4.00u |
| Units returned (settled) | 7.18u |
| Net P/L (settled) | +3.18u |
| Open exposure | 5.00u |
| ROI on settled stakes | +79.50% |
| Bets beating close (CLV+) | TBD / 3 |

## Process Notes

### Day 1 (2026-06-24)
- **CLV capture: failed.** Three of three pre-match bets have permanent TBD. Hard rule going forward: capture entry price + closing price.
- **Move faster on lineup-driven plays.** Vinicius +125 → +110 = 15 cents lost.
- **Promo conversion clean.** Boost on longest-odds +EV play. Boost the bet, don't bet the boost.

### Day 2 (2026-06-25)
- **Entry prices captured via bet-slip screenshots** — improvement on Day 1. Two team totals came in better than planned (Paraguay TT +255 vs +202, Sweden TT +230 vs +202), small entry-CLV win. Closing-line capture still pending (user out during kickoffs).
- **Bet blind on lineups by necessity** (user unavailable at kickoff). Filtered to team-level desperation theses (must-win teams can't rotate) + two player props (Isak, Enciso) user was confident would start. Correctly DECLINED 3pm games (muted desperation, efficient pricing, rotation-dependent edges unverifiable).
- **3pm-skip validated post-hoc:** Nagelsmann confirmed Germany would NOT rotate vs Ecuador (only forced changes: Rüdiger for injured Schlotterbeck, Raum for Nene Brown). The German-rotation-striker edge (Undav/Woltemade anytime) we declined to bet blind did not exist — Undav not starting. Discipline call validated.
- **Promo discipline:** deployed 4 of 5 promos (25% SOT, 30% any-wager, Drawbreaker, 30% SGP). Let the 20% SGP (+400) expire — no qualifying play. Did NOT force unused promos onto bad bets.
- **Correlation acknowledged:** bets 007–010 all PAR–AUS (3.0u on "Paraguay chases open game"); bets 005–006 both JPN–SWE Sweden-chase (2.0u). Two themes, each expressed multiple ways. A flat game takes down a cluster.
- **SGP (bet 010) flagged honestly as marginal-EV lottery**, not a clear edge — sized to 0.5u for that reason.
