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

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 3 |
| Win / Loss / Push | 2 / 1 / 0 |
| Units staked | 3.50u |
| Units returned | 6.68u |
| Net P/L | +3.68u |
| ROI | +105.14% (on settled stakes) |
| Bets beating close (CLV+) | TBD / 3 |
