# Betting Log — World Cup Unit System

**Theoretical units only.** Every wager is logged here: moneylines, totals, AND player props. Claude appends a row when a bet is confirmed placed, and fills Result / Payout / Closing Line / CLV when results are reported.

## Column key

- **Market**: `ML` (moneyline / 3-way), `TOTAL` (game over/under), `PROP` (player prop), `PARLAY`/`SGP`, `PROMO` (promo-driven play)
- **Fair %**: devigged fair probability of the selection
- **CLV**: closing-line value — did we beat the number that closed? (the real scoreboard)

## Open Bets

| ID | Date | Match | Market | Selection | Odds | Stake | Tier | Notes |
|---|---|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — | — | No open bets |

## Outstanding Promo Assets

| Asset | Source | Face | Est. EV | Notes |
|---|---|---|---|---|
| 0.10u free bet | Drawbreaker on bet 014 (EGY-IRN draw) | 0.10u | ~0.07u | Refund scaled to the 0.10u stake (as predicted). Deploy on a future longer-odds +EV play. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia TT Over 2.5 | +154 | ~48–53% | 2.00u | **WIN** | +3.08u | TBD | TBD | Final 3-1. Chase-for-GD thesis confirmed. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 (win by 3+) | +285 | ~38–43% | 0.50u | **LOSS** | −0.50u | TBD | TBD | Final 3-1 — won by 2. Correlated variance dart. |
| 003 | 2026-06-24 | SCO–BRA | PROP | Vinicius Jr anytime | +110 | ~50–55% | 1.00u | **WIN** | +1.10u | TBD | TBD | Usage-shift thesis cashed. |
| 004 | 2026-06-24 | MAR–HTI | PROMO/PROP | Brahim Díaz anytime (live) | +324 | ~28–34% | 0.50u | **LOSS** | −0.50u | n/a | n/a | +EV live dart, modal-outcome loss. |
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Isak 2+ shots on target | +282 (base +225 ×25% boost) | ~27–32% (revised) | 1.00u | **WIN** | +2.82u | +220 | **+1.56%** | BEAT close. Hit despite corrected/thinner thesis; close (~31%) aligned with revised fair. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden TT Over 1.5 | +230 | ~30–40% (revised) | 1.00u | **LOSS** | −1.00u | TBD | TBD | JPN-SWE 1-1; Sweden scored 1, needed 2. Corrected-down thesis (see error note). |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Total Over 2.5 | +286 (base +220 ×30% boost) | ~36–44% | 0.50u | **LOSS** | −0.50u | +240 | **−5.88%** | PAR-AUS 0-0. WORSE than close; over drifted out. Negative CLV foreshadowed cagey result. |
| 008 | 2026-06-25 | PAR–AUS | ML+PROMO | Paraguay ML (Drawbreaker) | +165 | ~36% | 1.00u | **LOSS (refunded)** | −1.00u | TBD | TBD | 0-0 draw → ML loses, Drawbreaker refunded 1.0u bonus bet (deployed on bet 016). |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay TT Over 1.5 | +255 | ~34–45% | 1.00u | **LOSS** | −1.00u | TBD | TBD | 0-0; part of PAR-AUS correlated cluster that failed together. |
| 010 | 2026-06-25 | PAR–AUS | SGP/PROMO | 3-leg: O2.5+BTTS+Enciso | +910 (base +700 ×30% boost) | ~10–11.5% | 0.50u | **LOSS** | −0.50u | TBD | TBD | 0-0; all legs dead. Flagged at placement as marginal-EV lottery. |
| 011 | 2026-06-26 | URU–ESP | TOTAL | Match Total Over 2.5 | +156 (base +120 ×30% boost) | ~47–55% | 0.50u | **LOSS** | −0.50u | TBD | TBD | URU-ESP 1-0 — only 1 goal, under. Spain managed; Uruguay didn't generate enough. |
| 012 | 2026-06-26 | NZL–BEL | PROMO/PROP | De Bruyne Goal+Assist | −139 (base −175 ×25% boost) | ~62–70% | 1.00u | **WIN** | +0.72u | TBD | TBD | KDB G/A cashed. Belgium-dominance thesis worked. Boost converted -175 to -139. |
| 013 | 2026-06-26 | CPV–KSA | TOTAL | Match Total Over 2.5 | +110 | ~50–58% | 0.50u | **LOSS** | −0.50u | TBD | TBD | CPV-KSA 0-0. SECOND must-win game to bust 0-0 (after PAR-AUS). "Both must win→goals" inference burned again — sized small for exactly this reason. See note. |
| 014 | 2026-06-26 | EGY–IRN | ML+PROMO | Egypt ML (Drawbreaker) | +150 | ~38% | 0.10u | **LOSS (refunded)** | −0.10u | TBD | TBD | Draw (as the thesis expected). ML loses but Drawbreaker refunded 0.10u free bet (scaled to stake). Typo stake 0.10u vs intended 1.0u. The happy-draw read was CORRECT — just expressed via the one leg (ML) that doesn't cash on a draw; the Drawbreaker is what monetized the correct read. |
| 015 | 2026-06-26 | NOR–FRA | TOTAL | France Team Total Over 2.5 | +139 | ~40–50% | 0.50u | **WIN** | +0.70u | TBD | TBD | France 3+ vs weakened Norway. Team-level play (immune to attacker toss-up) cashed where the France ML −175 we PASSED would also have won but at worse value/with no edge. |
| 016 | 2026-06-26 | URU–ESP | PROP | Oyarzabal anytime | +155 | ~43% | BONUS 1.0u | **LOSS** | 0.00u (bonus) | TBD | TBD | No goal. Bonus bet (house money) — zero cash impact. Day-2 Drawbreaker refund fully consumed here. |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 16 (all settled) |
| Win / Loss / Push | 5 / 11 / 0 |
| Units staked (cash) | 11.60u |
| Net P/L (cash) | +2.31u |
| ROI on stakes | +20.0% |
| Outstanding free bets | 0.10u (~0.07u EV) |
| **Rolling CLV (measurable)** | **−2.16% avg over 2 bets; beat close 1 of 2 (Day-3 closes not captured)** |

## Process Notes

### Day 1 (2026-06-24)
- CLV capture FAILED (3 bets permanent TBD). Promo conversion clean. Move faster on lineup-driven plays.

### Day 2 (2026-06-25)
- First real CLV data: Isak +1.56% (beat close, won), Match O2.5 −5.88% (worse, lost) — CLV agreed with both outcomes.
- PAR-AUS correlated cluster failed together on a 0-0 (4 bets). "Desperation→goals" is a weak inference.
- ERROR: Sweden "must-win" thesis was wrong (built on unverified qualification claim). → STANDING RULE added.

### Day 3 (2026-06-26)
- **Green day: 2-4-0, +0.31u cash.** Two winners (KDB G/A, France TT) outweighed four small losers — the upside-system shape (fewer winners, profit from them being priced right) in miniature.
- **STANDING RULE applied successfully** — EGY-IRN/CPV-KSA theses verified vs 3rd-place table before sizing.
- **"Both must win → goals" burned AGAIN:** CPV-KSA 0-0, the second consecutive must-win game to bust under (after PAR-AUS). This is now a PATTERN, not a one-off. Two data points: must-win desperation does NOT reliably produce goals — if anything these games are TIGHT (fear of losing > desire to win). REVISED LESSON: stop treating mutual must-win as an over signal; if anything lean slight UNDER or avoid. Sizing CPV small was right; the better call may have been no bet.
- **The happy-draw read (EGY-IRN) was CORRECT** — it drew, as the thesis predicted. But we expressed it via Egypt ML (loses on a draw) + Drawbreaker. The Drawbreaker monetized the correct read; the ML leg didn't. Worth noting: a direct DRAW bet would have cashed outright. The Drawbreaker structure was the more conservative expression and it (barely, at 0.10u) paid via refund.
- **France TT O2.5 cashed; passing the France ML −175 was still correct** — the ML would also have won, but at no edge (priced-in, no urgency). We took the +EV team-total instead of the efficient ML. Right process even though both would've won.
- **Line-move discipline** (dropped Belgium TT +124→−178) avoided a negative-EV bet. Both SGP promos expired unused (no clean play).

### 🔒 STANDING RULE (2026-06-25)
**Never base a play on an unverified qualification claim. If a thesis depends on "must win," "already through," "a draw eliminates them," best-third positioning, or any GD/tiebreaker math — VERIFY against actual standings + the live 3rd-place table BEFORE pricing. If the data isn't in hand, ASK THE USER to retrieve it. Directional reads may stay flagged low-confidence; hard qualification claims must be sourced. When uncertain on anything load-bearing, STOP and ASK.**

### 🔒 STANDING LESSON (2026-06-26)
**Mutual must-win games do NOT reliably go over. Two-for-two (PAR-AUS 0-0, CPV-KSA 0-0) busted under. Fear of losing makes these games tight, not open. Do not use "both teams must win" as a totals-OVER signal going forward; treat it as neutral-to-under and require an independent reason for any over.**
