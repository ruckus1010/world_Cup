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
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Alexander Isak 2+ shots on target | +282 (base +225 × 25% boost) | ~27–32% (REVISED DOWN) | thin +EV, boost-dependent | 1.00u | Standard | 25% player-SOT boost. **THESIS CORRECTED (see Day 2 error note): Sweden NOT must-win — they sit 2nd among 3rd-place teams (3pts/GD 0), comfortably above the 8-team cut. A draw very likely advances them (Polymarket had them ~92% to advance).** Reduced-desperation chase → fewer Sweden shots → Isak 2+SOT fair revised from 31–36% to ~27–32%. Breakeven +282 = 26.2%, so STILL marginally +EV thanks to the boost, but thinner than originally claimed. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden team total Over 1.5 (away O/U 1.5) | +230 | ~30–40% (REVISED DOWN) | borderline / thin | 1.00u | Standard | Got +230 vs planned +202 — better price (entry CLV win). **THESIS CORRECTED: Sweden is NOT must-win (see error note). Original "must score 2+ to advance, cannot rotate" claim was WRONG — a draw likely advances them as a top 3rd-place team.** Fair revised from 35–47% to ~30–40%. Breakeven +230 = 30.3%. Now BORDERLINE, not the strong play originally represented. Match-total/BTTS angles hold up better than this Sweden-specific TT because they don't depend on Sweden's desperation. |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Total Over 2.5 | +286 (base +220 × 30% boost) | ~36–44% | +0.29 EV/u | 0.50u | Standard | 30% any-wager boost. Play-in: both chase, esp. Paraguay (must win, GD -2 vs AUS 0). Paraguay desperation thesis CONFIRMED accurate vs 3rd-place table (Paraguay 3pts/GD -2, below the cut line — they genuinely need the win). |
| 008 | 2026-06-25 | PAR–AUS | ML + PROMO | Paraguay moneyline (Drawbreaker) | +165 | ~36% | +EV via refund | 1.00u | Standard | Drawbreaker: refunds up to 1.25u bonus bet if match draws. Paraguay must win; high draw equity (~42%) makes refund live. Paraguay desperation CONFIRMED vs table (GD -2, below cut). |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay team total Over 1.5 (home O/U 1.5) | +255 | ~34–45% | +EV | 1.00u | Standard | Got +255 vs planned +202 — better price (entry CLV win). Paraguay must win/chase, cannot rotate. Desperation CONFIRMED vs table. |
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
- **Bet blind on lineups by necessity** (user unavailable at kickoff). Filtered to team-level desperation theses + two player props (Isak, Enciso) user was confident would start. Correctly DECLINED 3pm games (muted desperation, efficient pricing, rotation-dependent edges unverifiable).
- **3pm-skip validated post-hoc:** Nagelsmann confirmed Germany would NOT rotate vs Ecuador (only forced changes: Rüdiger for injured Schlotterbeck, Raum for Nene Brown). The German-rotation-striker edge (Undav/Woltemade anytime) we declined to bet blind did not exist — Undav not starting. Discipline call validated.
- **Promo discipline:** deployed 4 of 5 promos (25% SOT, 30% any-wager, Drawbreaker, 30% SGP). Let the 20% SGP (+400) expire — no qualifying play.
- **Correlation acknowledged:** bets 007–010 all PAR–AUS (3.0u on "Paraguay chases open game"); bets 005–006 both JPN–SWE Sweden-chase (2.0u).
- **SGP (bet 010) flagged honestly as marginal-EV lottery**, not a clear edge — sized to 0.5u.

### ⚠️ Day 2 ERROR — Sweden "must-win" thesis was WRONG (caught by user post-placement)
- **What happened:** Bets 005 and 006 (both JPN–SWE) were built and sold on the premise that Sweden was a hard must-win team that "cannot rotate" and had to throw everyone forward. This was used explicitly as a *robustness argument* for betting them blind on lineups.
- **The reality:** The 3rd-place-teams table showed Sweden sitting 2nd among all 3rd-place sides (3pts, GD 0, GF 6), comfortably ABOVE the 8-team advancement cut line (8th = Cape Verde, 2pts). A DRAW (→4pts) very likely advances them. Polymarket had Sweden ~92% to advance. They were never must-win.
- **Impact on the bets:** The "forced chase" engine driving both Sweden bets was overstated. Revised fairs: Sweden TT O1.5 dropped from 35–47% to ~30–40% (now borderline at +230 / breakeven 30.3%); Isak 2+SOT dropped from 31–36% to ~27–32% (still marginally +EV at +282 / breakeven 26.2%, but thinner, boost-dependent). Bets are not bad, just thinner than represented. Conviction was inflated by a qualification-math error.
- **Root cause:** Asserted a qualification incentive ("must win, cannot rotate") from memory/assumption WITHOUT verifying the 3rd-place table, which determines whether a draw is actually fatal. The whole system is built on reading qualification incentives correctly — getting this wrong is a core-process failure, not a peripheral one.

### 🔒 STANDING RULE (added 2026-06-25, per user instruction)
**Never base a play on an unverified qualification claim. If a thesis depends on "must win," "already through," "a draw eliminates them," "needs help," best-third positioning, or any GD/tiebreaker math — VERIFY IT against actual standings + the live 3rd-place table BEFORE pricing or recommending. If the data isn't in hand, ASK THE USER to retrieve it (standings, 3rd-place table, advancement scenarios, Polymarket/market advancement odds) and do NOT finalize the play until confirmed.** Directional reads (rotation likelihood, game-script guesses) can stay flagged as low-confidence, but hard qualification claims must be sourced, not assumed. When uncertain on anything load-bearing, stop and ask rather than asserting.
