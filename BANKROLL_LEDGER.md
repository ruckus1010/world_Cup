# Bankroll Ledger — World Cup Unit System

**Theoretical money. Tracked in UNITS. 1 unit = 1% of starting bankroll.**

## Current State

| Field | Value |
|---|---|
| Starting bankroll | 100.00u |
| Current bankroll | 100.19u |
| Net P/L (cash) | +0.19u |
| ROI | +0.19% (on bankroll); +0.73% (on 25.99u staked) |
| Open exposure | 0.00u |
| Outstanding free bets | 1.35u (~0.95u EV) |
| Record (W-L-P) | 8-20-0 |
| Rolling CLV | −2.16% avg (2 measurable bets); beat close 1 of 2. Days 3–5 closes not captured. |
| Last updated | 2026-06-29 |

## Sizing Tiers

| Tier | Stake | When |
|---|---|---|
| 1u | 1.00u | Standard detected edge |
| 2u | 2.00u | Strong edge or strong promo conversion |
| 3u | 3.00u | Max — clear +EV locks / outsized upside only (rare) |

- Hard cap: 3u on any single outcome. Hard cap: 10u total exposure per day.

## Bankroll History

| Date | Starting | Day P/L | Ending | Note |
|---|---|---|---|---|
| 2026-06-24 | 100.00u | +3.18u | 103.18u | Day 1, 4 bets, 2-2-0. |
| 2026-06-25 | 103.18u | −1.18u | 102.00u | Day 2, 6 bets, 1-5-0. Isak +282 WIN (beat close). PAR-AUS 0-0 cluster failed. First CLV data. |
| 2026-06-26 | 102.00u | +0.31u | 102.31u | Day 3, 6 bets, 2-4-0. WIN: KDB G/A −139, France TT O2.5 +139. Two must-win games busted 0-0 again. |
| 2026-06-27 | 102.31u | −5.23u | 97.08u | Day 4 (final group MD), 7 bets, 1-6-0. WORST DAY. Late beats DZA-AUT (Drawbreaker refund 1.25u) + CRO-GHA. COL-POR U2.5 lone win. JOR-ARG rotation-under MISSED. Both SGPs died in a correlated cluster. |
| 2026-06-29 | 97.08u | **+3.11u** | **100.19u** | Day 5 (R32), 5 bets, 2-3-0 ledger but cash +3.11u via hedge math. GER-PAR Under 2.5 +110 WON 1.5u (+1.65u) — public-inflated-over thesis confirmed; Paraguay bunkered, won on PKs. Brazil SGP (Vini G/A version) LOST 1u. Brahim Diaz 2+ shots boosted LOST 0.5u. NED-MAR SGP (NED qualify + U2.5 + Gakpo G/A boost +715) LOST $9.94 — but live HEDGE on Morocco To Qualify −105 at $41.51 locked +$29.56 either way; Morocco won on PKs. Hedge math: −0.994u SGP + 3.951u hedge gross − 4.151u hedge stake = +2.96u net on that game. Back above 100u starting bankroll for first time since Day 3. |

## Notes
- **Through Day 5:** +0.19u cash on 25.99u staked, record 8-20-0, ROI +0.73%. Back above 100u starting bankroll. Record is misleading because the hedge "loss" was structurally a profit-lock.
- **KEY STANDING LESSONS:** (1) mutual must-win ≠ over; (2) rotation/dead-rubber ≠ under when talent gap is large; (3) correlated singles + overlapping SGP = one unit of risk; (4) NEW Day 5 — **public-inflated favorites at high totals creates UNDER value** (GER-PAR Under +110 confirmed; 97/3 public on GER pumped the over to −140 and left under soft); (5) NEW Day 5 — **live hedging an SGP near its conclusion converts variance to locked profit cleanly when the favorite-vs-dog price has flipped from pregame** (Morocco went from +120 pregame to −105 live after 90' of dominance).
- **Day-5 hedge logic worth repeating:** Once Under 2.5 + Gakpo G/A were effectively locked at 90', the SGP reduced to a single live bet on NED To Qualify. With Morocco then favored live and dominating the stats (65% poss, 0.65 xG to 0.23), the hedge locked profit while still having directional logic on the price flip.
- **CLV still barely populated (2 bets).** Closing-line capture remains the #1 process gap.
- **Outstanding:** 0.10u + 1.25u free bets (1.35u face, ~0.95u EV).
