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
| — | — | — | — | — | — | — | — | — | — | No open bets |

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
| Total bets placed | 4 |
| Win / Loss / Push (settled) | 2 / 2 / 0 |
| Units staked | 4.00u |
| Units returned | 7.18u |
| Net P/L | +3.18u |
| ROI on stakes | +79.50% |
| Bets beating close (CLV+) | TBD / 3 (one was live, no close benchmark) |

## Process Notes (Day 1)

- **CLV capture: failed.** Three of three pre-match bets have permanent TBD in the Close/CLV columns. This is lost data and the most important fix for future slates. Hard rule going forward: screenshot bet slip when placing + capture DK closing price ≤5 min before kickoff (ideally also Pinnacle/Circa).
- **Move faster on lineup-driven plays.** Vinicius anytime moved from quoted +125 to taken +110 in the window between team news and bet — 15 cents of edge lost to slow execution.
- **Promo conversion was clean.** 20% profit boost deployed on the longest-odds +EV candidate (Brahim Díaz, +270 → +324 effective), which is the correct way to use a profit boost. Boost did NOT cause a marginal bet to be added — it was applied to a bet already on the short list.
- **Discipline on broken thesis: good.** Dropped Hakimi assist when price moved +320 → +195, dropped El Kaabi when price moved +105 → -110, declined to bet CZE–MEX without lineups.
- **+3.18u net is variance noise on a 4-bet sample.** Real evaluation comes from CLV (currently missing) and process quality (see grades above), not short-run W/L.
