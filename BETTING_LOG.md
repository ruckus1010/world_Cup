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
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia Team Total Over 2.5 | +154 | ~48–53% | +18–25% EV | 2.00u | Strong | Devig fair ~40%; Bosnia chasing GD for best-third lottery, Qatar broken after 0-6. Got +6 cents better than quoted +148. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 (win by 3+) | +285 | ~38–43% | +45–65% EV | 0.50u | Upside dart | Correlated with bet 001 — same blowout thesis, bigger payout. Sized small to acknowledge correlation. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — | — | — | — | — | — | No settled bets yet |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 2 |
| Win / Loss / Push | 0 / 0 / 0 |
| Units staked | 2.50u |
| Units returned | 0.00u |
| Net P/L | +0.00u |
| ROI | 0.00% |
| Bets beating close (CLV+) | 0 / 0 |
