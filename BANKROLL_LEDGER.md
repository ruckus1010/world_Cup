# Bankroll Ledger — World Cup Unit System

**Theoretical money. Tracked in UNITS. 1 unit = 1% of starting bankroll.**

## Current State

| Field | Value |
|---|---|
| Starting bankroll | 100.00u |
| Current bankroll | 102.00u |
| Net P/L (cash) | +2.00u |
| ROI | +2.00% (on bankroll); +22.2% (on 9.0u staked) |
| Open exposure | 0.00u |
| Outstanding bonus bets | 1.0u (~0.7u EV) from Drawbreaker |
| Record (W-L-P) | 3-7-0 |
| Rolling CLV | −2.16% avg (2 measurable bets); beat close 1 of 2 |
| Last updated | 2026-06-25 |

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
| 2026-06-24 | 100.00u | +3.18u | 103.18u | Day 1, 4 bets, 2-2-0. WIN: Bosnia TT O2.5 (+3.08u), Vini anytime (+1.10u). LOSS: Bosnia -2.5, Brahim Díaz live. |
| 2026-06-25 | 103.18u | −1.18u | 102.00u | Day 2, 6 bets, 1-5-0. WIN: Isak 2+SOT +282 (+2.82u, beat close +1.56%). LOSS: Sweden TT, Match O2.5 (CLV -5.88%), Paraguay ML (0-0 draw, Drawbreaker refunded 1.0u bonus bet), Paraguay TT, SGP. JPN-SWE 1-1, PAR-AUS 0-0. PAR-AUS correlated cluster failed together as flagged. First real CLV data captured. |

## Notes
- **Bonus bet outstanding:** 1.0u from the Drawbreaker (PAR-AUS draw). Deploy on a future +EV play; worth ~0.7u in EV since bonus bets pay winnings only.
- **Through 2 days:** +2.00u cash on 9.0u staked. Record 3-7-0 looks bad, but P/L is positive because the wins were larger-odds (Bosnia +154 2u, Isak +282 1u) while losses were mostly 0.5-1u. This is the expected shape of an upside-hunting system: more losers than winners, profit carried by bigger-priced hits. CLV (-2.16% over 2 bets) is the real read and it's a tiny, near-neutral sample — too small to conclude anything yet.
