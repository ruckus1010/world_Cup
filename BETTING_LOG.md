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
| 1.0u bonus bet | Drawbreaker on bet 008 (PAR-AUS drew 0-0) | 1.0u | ~0.7u | Use on a +EV play; bonus bets return winnings only (no stake back), so worth ~70% of face. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia TT Over 2.5 | +154 | ~48–53% | 2.00u | **WIN** | +3.08u | TBD | TBD | Final 3-1. Chase-for-GD thesis confirmed. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 (win by 3+) | +285 | ~38–43% | 0.50u | **LOSS** | −0.50u | TBD | TBD | Final 3-1 — won by 2. Correlated variance dart. |
| 003 | 2026-06-24 | SCO–BRA | PROP | Vinicius Jr anytime | +110 | ~50–55% | 1.00u | **WIN** | +1.10u | TBD | TBD | Usage-shift thesis cashed. |
| 004 | 2026-06-24 | MAR–HTI | PROMO/PROP | Brahim Díaz anytime (live) | +324 | ~28–34% | 0.50u | **LOSS** | −0.50u | n/a | n/a | +EV live dart, modal-outcome loss. |
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Isak 2+ shots on target | +282 (base +225 ×25% boost) | ~27–32% (revised) | 1.00u | **WIN** | +2.82u | +220 | **+1.56%** | BEAT close (entry base +225 vs close +220). Hit despite corrected/thinner thesis. Close (~31% implied) aligned with REVISED fair, validating the downward revision — was closer to a coin flip than the original inflated thesis claimed. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden TT Over 1.5 | +230 | ~30–40% (revised) | 1.00u | **LOSS** | −1.00u | TBD | TBD | JPN-SWE 1-1; Sweden scored 1, needed 2. Thesis had been corrected down from must-win (see error note); loss consistent with reduced-desperation reality. |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Total Over 2.5 | +286 (base +220 ×30% boost) | ~36–44% | 0.50u | **LOSS** | −0.50u | +240 | **−5.88%** | PAR-AUS 0-0. WORSE than close (entry base +220 vs close +240 — over drifted OUT; market faded it pre-KO). Negative CLV correctly foreshadowed the cagey result. Betting blind/early meant we couldn't react to the drift. |
| 008 | 2026-06-25 | PAR–AUS | ML+PROMO | Paraguay ML (Drawbreaker) | +165 | ~36% | 1.00u | **LOSS (refunded)** | −1.00u | TBD | TBD | 0-0 draw → ML loses, but Drawbreaker triggered → 1.0u bonus bet credited (see Outstanding Promo Assets). Promo did exactly its job on a draw. |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay TT Over 1.5 | +255 | ~34–45% | 1.00u | **LOSS** | −1.00u | TBD | TBD | 0-0; Paraguay scored 0. Part of the PAR-AUS correlated cluster that failed together. |
| 010 | 2026-06-25 | PAR–AUS | SGP/PROMO | 3-leg: O2.5+BTTS+Enciso | +910 (base +700 ×30% boost) | ~10–11.5% | 0.50u | **LOSS** | −0.50u | TBD | TBD | 0-0; all three legs dead. Flagged at placement as marginal-EV lottery. |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 10 (all settled) |
| Win / Loss / Push | 3 / 7 / 0 |
| Units staked | 9.00u |
| Net P/L (cash) | +2.00u |
| ROI on stakes | +22.2% |
| Outstanding bonus bets | 1.0u (~0.7u EV) |
| **Rolling CLV (measurable)** | **−2.16% avg over 2 bets; beat close 1 of 2** |

## Process Notes

### Day 1 (2026-06-24)
- CLV capture FAILED (3 bets permanent TBD). Promo conversion clean. Move faster on lineup-driven plays (Vini +125→+110).

### Day 2 (2026-06-25)
- **First real CLV data captured** — the single biggest process win of the run so far. Two measurable points: Isak +1.56% (beat close, won), Match O2.5 −5.88% (worse than close, lost). CLV directionally agreed with both outcomes. This is exactly why CLV is the scoreboard, not W/L.
- **The PAR-AUS correlated cluster failed together, as flagged.** A single 0-0 took out 4 bets (007, 008, 009, 010) at once — the materialized version of the correlation risk noted at construction. The Drawbreaker (008) softened one leg via a 1.0u bonus-bet refund. Lesson reinforced: stacking 3.0u across four correlated expressions of one game-script means one cagey game zeroes the cluster. Each was individually +EV by our math, but cluster variance is real and was underweighted in sizing.
- **"Desperation → goals" is a weaker inference than treated.** Paraguay genuinely needed to win (correct vs table), but a team needing goals can still play tight and lose 0-0. "Needs a result" raises over probability; it does not make it a lock. Future: don't let a correct qualification read inflate a separate probabilistic claim about game flow.
- **Blind/early placement has a cost:** we couldn't react to the Match O2.5 line drifting +220→+240 against us. When forced to bet early, accept we forfeit the ability to fade our own line drift.

### ⚠️ Day 2 ERROR — Sweden "must-win" thesis was WRONG (caught by user)
- Bets 005/006 were built on "Sweden must win, cannot rotate" and that was used as a robustness argument for betting blind. FALSE: the 3rd-place table showed Sweden 2nd among 3rd-place teams (3pts/GD 0), comfortably above the cut; a draw very likely advanced them (Polymarket ~92%). Fairs revised down (TT 35-47%→30-40%; Isak 31-36%→27-32%). Root cause: asserted a qualification incentive from assumption without checking the 3rd-place table.

### 🔒 STANDING RULE (2026-06-25, per user instruction)
**Never base a play on an unverified qualification claim. If a thesis depends on "must win," "already through," "a draw eliminates them," best-third positioning, or any GD/tiebreaker math — VERIFY against actual standings + the live 3rd-place table BEFORE pricing. If the data isn't in hand, ASK THE USER to retrieve it and do NOT finalize until confirmed. Directional reads (rotation, game-script) may stay flagged low-confidence; hard qualification claims must be sourced, not assumed. When uncertain on anything load-bearing, STOP and ASK.**
