# Betting Log — World Cup Unit System

**Theoretical units only.** Every wager is logged here: moneylines, totals, AND player props. Claude appends a row when a bet is confirmed placed, and fills Result / Payout / Closing Line / CLV when results are reported.

## Column key

- **Market**: `ML` (moneyline / 3-way), `TOTAL` (game over/under), `PROP` (player prop), `PARLAY`/`SGP`, `PROMO` (promo-driven play)
- **Fair %**: devigged fair probability of the selection
- **CLV**: closing-line value — did we beat the number that closed? (the real scoreboard)

## Open Bets

| ID | Date | Match | Market | Selection | Odds | Stake | Tier | Notes |
|---|---|---|---|---|---|---|---|---|
| 011 | 2026-06-26 | URU–ESP | TOTAL | Match Total Over 2.5 | +120 base → **+156** (30% boost) | 0.50u | Standard | 30% profit boost (max 0.5u). Uruguay must chase a managing Spain. |
| 012 | 2026-06-26 | NZL–BEL | PROMO/PROP | De Bruyne Goal+Assist | −175 base → **−139** (25% G/A boost) | 1.00u | Standard | 25% goals/assists boost (combined G/A market only). Elite creator vs weak NZ, Belgium dominant. Fair ~62–70%; thinner than the pure-assist play we first scoped but safer (goal OR assist). |
| 013 | 2026-06-26 | CPV–KSA | TOTAL | Match Total Over 2.5 | +110 | 0.50u | Standard | Both must win (verified vs 3rd-place table). SIZED SMALL on purpose — same "desperation→goals" thesis that lost the PAR-AUS cluster 0-0. |
| 014 | 2026-06-26 | EGY–IRN | ML+PROMO | Egypt ML (Drawbreaker) | +150 | **0.10u** | Standard | TYPO: intended 1.0u, placed 0.10u. Left in place — cashing out forfeits the Drawbreaker. Egypt content (draw locks top-2); Iran also content (draw → 3pts/GD0, above cutline — verified vs table). Covers Egypt win OR draw; only Iran win loses. Drawbreaker refund likely scales to 0.1u stake, not full 1.25u. |
| 015 | 2026-06-26 | NOR–FRA | TOTAL | France Team Total Over 2.5 | +139 | 0.50u | Standard | Norway rotating (partial — Haaland line +130 suggests he plays), France small rotation. Team-level play, immune to France's attacker toss-up. France 3+ vs weakened Norway. NOT the France ML (−175, priced-in + qualified-France has no urgency to win). |
| 016 | 2026-06-26 | URU–ESP | PROP | Oyarzabal anytime scorer | +155 | **BONUS BET (1.0u)** | House money | Deploys the Day-2 Drawbreaker bonus bet (~0.7u EV). Longest-odds +EV play; bonus bets pay winnings only. Lineup risk (Spain rotates fwds) acceptable on house money. |

## Outstanding Promo Assets

| Asset | Source | Face | Est. EV | Notes |
|---|---|---|---|---|
| — | — | — | — | Day-2 Drawbreaker bonus bet now DEPLOYED on bet 016 (Oyarzabal). None outstanding. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia TT Over 2.5 | +154 | ~48–53% | 2.00u | **WIN** | +3.08u | TBD | TBD | Final 3-1. Chase-for-GD thesis confirmed. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 (win by 3+) | +285 | ~38–43% | 0.50u | **LOSS** | −0.50u | TBD | TBD | Final 3-1 — won by 2. Correlated variance dart. |
| 003 | 2026-06-24 | SCO–BRA | PROP | Vinicius Jr anytime | +110 | ~50–55% | 1.00u | **WIN** | +1.10u | TBD | TBD | Usage-shift thesis cashed. |
| 004 | 2026-06-24 | MAR–HTI | PROMO/PROP | Brahim Díaz anytime (live) | +324 | ~28–34% | 0.50u | **LOSS** | −0.50u | n/a | n/a | +EV live dart, modal-outcome loss. |
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Isak 2+ shots on target | +282 (base +225 ×25% boost) | ~27–32% (revised) | 1.00u | **WIN** | +2.82u | +220 | **+1.56%** | BEAT close. Hit despite corrected/thinner thesis; close (~31%) aligned with revised fair. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden TT Over 1.5 | +230 | ~30–40% (revised) | 1.00u | **LOSS** | −1.00u | TBD | TBD | JPN-SWE 1-1; Sweden scored 1, needed 2. Corrected-down thesis (see error note). |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Total Over 2.5 | +286 (base +220 ×30% boost) | ~36–44% | 0.50u | **LOSS** | −0.50u | +240 | **−5.88%** | PAR-AUS 0-0. WORSE than close; over drifted out, market faded it. Negative CLV foreshadowed cagey result. |
| 008 | 2026-06-25 | PAR–AUS | ML+PROMO | Paraguay ML (Drawbreaker) | +165 | ~36% | 1.00u | **LOSS (refunded)** | −1.00u | TBD | TBD | 0-0 draw → ML loses, Drawbreaker refunded 1.0u bonus bet (deployed on bet 016). |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay TT Over 1.5 | +255 | ~34–45% | 1.00u | **LOSS** | −1.00u | TBD | TBD | 0-0; part of PAR-AUS correlated cluster that failed together. |
| 010 | 2026-06-25 | PAR–AUS | SGP/PROMO | 3-leg: O2.5+BTTS+Enciso | +910 (base +700 ×30% boost) | ~10–11.5% | 0.50u | **LOSS** | −0.50u | TBD | TBD | 0-0; all legs dead. Flagged at placement as marginal-EV lottery. |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 16 (10 settled, 6 open) |
| Win / Loss / Push (settled) | 3 / 7 / 0 |
| Units staked (settled) | 9.00u |
| Net P/L (settled, cash) | +2.00u |
| ROI on settled stakes | +22.2% |
| Open cash exposure (Day 3) | 2.60u (+ 1.0u bonus bet on Oyarzabal) |
| Outstanding bonus bets | 0 (deployed) |
| **Rolling CLV (measurable)** | **−2.16% avg over 2 bets; beat close 1 of 2** |

## Process Notes

### Day 1 (2026-06-24)
- CLV capture FAILED (3 bets permanent TBD). Promo conversion clean. Move faster on lineup-driven plays (Vini +125→+110).

### Day 2 (2026-06-25)
- **First real CLV data captured.** Isak +1.56% (beat close, won), Match O2.5 −5.88% (worse than close, lost). CLV directionally agreed with both outcomes.
- **PAR-AUS correlated cluster failed together** on a 0-0 — 4 bets down at once. Drawbreaker softened one leg. Lesson: correlated stacking = one cagey game zeroes the cluster.
- **"Desperation → goals" is a weak inference.** Needing a result raises over probability; doesn't make it a lock.

### ⚠️ Day 2 ERROR — Sweden "must-win" thesis was WRONG (caught by user)
- Built bets 005/006 on an unverified "Sweden must win" claim; the 3rd-place table showed a draw advanced them. Root cause: asserted qualification incentive without checking the table.

### Day 3 (2026-06-26)
- **STANDING RULE applied successfully.** Held the EGY-IRN and CPV-KSA theses as unverified until the user pulled the 3rd-place table; both confirmed (Iran content w/ draw → 3pts/GD0 above cut; CPV/KSA both genuinely must win). Verified, not assumed — the rule working as intended.
- **Line-move discipline.** Dropped Belgium TT O2.5 when it moved +124 → −178 (edge inverted; re-derived EV at actual price, did not chase). Echoes the Day-1 Vinicius lesson.
- **Passed France ML −175** despite "weak Norway" narrative: line already moved on the news (−160→−175) and qualified France has no urgency to win (mutual low-stakes). Took France TT O2.5 +139 instead (team-level, no urgency dependency).
- **Promo discipline.** Deployed 30% (max 0.5u) → URU O2.5; 25% G/A → KDB G/A; Drawbreaker → Egypt ML; bonus bet → Oyarzabal. Let BOTH SGP promos (30% 3-leg, 20% 2-leg) expire — no clean SGP without over-concentrating NZL-BEL or repeating the PAR-AUS goal-parlay mistake. Consistent with Day-2 discipline.
- **Sizing-typo logged honestly:** Egypt ML placed 0.10u vs intended 1.0u; left in place to preserve Drawbreaker rather than cash out.
- **Diversification improved vs Day 2:** after dropping Belgium TT, exposure spread across 4 separate games (URU-ESP ×2, CPV-KSA, EGY-IRN, NOR-FRA), no correlated cluster.

### 🔒 STANDING RULE (2026-06-25, per user instruction)
**Never base a play on an unverified qualification claim. If a thesis depends on "must win," "already through," "a draw eliminates them," best-third positioning, or any GD/tiebreaker math — VERIFY against actual standings + the live 3rd-place table BEFORE pricing. If the data isn't in hand, ASK THE USER to retrieve it and do NOT finalize until confirmed. Directional reads (rotation, game-script) may stay flagged low-confidence; hard qualification claims must be sourced, not assumed. When uncertain on anything load-bearing, STOP and ASK.**
