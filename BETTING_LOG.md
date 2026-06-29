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
| 0.10u free bet | Drawbreaker on bet 014 (EGY-IRN draw) | 0.10u | ~0.07u | Refund scaled to the 0.10u stake. Deploy on a future longer-odds +EV play. |
| 1.25u free bet | Drawbreaker on bet 017 (DZA-AUT draw) | 1.25u | ~0.88u | Algeria led to the last kick, drew. Refund as bonus bet. Deploy on a longer-odds +EV play. |

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
| 013 | 2026-06-26 | CPV–KSA | TOTAL | Match Total Over 2.5 | +110 | ~50–58% | 0.50u | **LOSS** | −0.50u | TBD | TBD | CPV-KSA 0-0. SECOND must-win game to bust 0-0 (after PAR-AUS). "Both must win→goals" inference burned again — sized small for exactly this reason. |
| 014 | 2026-06-26 | EGY–IRN | ML+PROMO | Egypt ML (Drawbreaker) | +150 | ~38% | 0.10u | **LOSS (refunded)** | −0.10u | TBD | TBD | Draw (as the thesis expected). ML loses but Drawbreaker refunded 0.10u free bet. The happy-draw read was CORRECT — expressed via the one leg (ML) that doesn't cash on a draw. |
| 015 | 2026-06-26 | NOR–FRA | TOTAL | France Team Total Over 2.5 | +139 | ~40–50% | 0.50u | **WIN** | +0.70u | TBD | TBD | France 3+ vs weakened Norway. Team-level play (immune to attacker toss-up) cashed. |
| 016 | 2026-06-26 | URU–ESP | PROP | Oyarzabal anytime | +155 | ~43% | BONUS 1.0u | **LOSS** | 0.00u (bonus) | TBD | TBD | No goal. Bonus bet (house money) — zero cash impact. |
| 017 | 2026-06-27 | DZA–AUT | ML+PROMO | Algeria ML (Drawbreaker) | +295 | ~24% | 1.25u | **LOSS (refunded)** | −1.25u | TBD | TBD | Algeria LED until the last kick; late equalizer → draw. Drawbreaker refunds 1.25u bonus bet. Win-equity/equilibrium thesis correct through 89'; lost to last-minute variance. |
| 018 | 2026-06-27 | JOR–ARG | TOTAL | Match Under 2.5 | +160 | ~37% | 1.00u | **LOSS** | −1.00u | TBD | TBD | Went OVER. Rotated Argentina still outscored expectation; talent gap > rotation effect. Thesis missed (not pure variance). |
| 019 | 2026-06-27 | JOR–ARG | PROP/PROMO | Julián Álvarez anytime | +113.6 (base −110 ×25% boost) | ~52% | 1.00u | **LOSS** | −1.00u | TBD | TBD | No goal. Backup-9 thesis didn't cash. |
| 020 | 2026-06-27 | CRO–GHA | ML/PROMO | Draw | +273 (base +210 ×30% boost) | ~33% | 0.50u | **LOSS** | −0.50u | TBD | TBD | Draw until a LAST-MINUTE Croatia winner. Mutual-content thesis correct through 89'; late variance. |
| 021 | 2026-06-27 | COL–POR | TOTAL | Match Under 2.5 | +105 | ~46% | 0.50u | **WIN** | +0.525u | TBD | TBD | Under cashed. Cagey controlled-game thesis confirmed. Day's lone winner. |
| 022 | 2026-06-27 | PAN–ENG | SGP/PROMO | Rashford ATGS + Saka G/A + Match O2.5 | +436 (base +335 ×30% boost) | ~25% | 1.00u | **LOSS** | −1.00u | TBD | TBD | Did not hit. |
| 023 | 2026-06-27 | JOR–ARG | SGP/PROMO | Match U2.5 + Álvarez ATGS + ARG win | boosted (20%), price not captured | ~20% | 1.00u | **LOSS** | −1.00u | TBD | TBD | Did not hit; correlated with 018/019 — all three died on the over + no Álvarez goal (warned-about clustering). |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 23 (all settled) |
| Win / Loss / Push | 6 / 17 / 0 |
| Units staked (cash) | 17.85u |
| Net P/L (cash) | −2.92u |
| ROI on stakes | −16.4% |
| Outstanding free bets | 1.35u (0.10u + 1.25u) (~0.95u EV) |
| **Rolling CLV (measurable)** | **−2.16% avg over 2 bets; beat close 1 of 2 (Day 3–4 closes not captured)** |

## Process Notes

### Day 1 (2026-06-24)
- CLV capture FAILED (3 bets permanent TBD). Promo conversion clean. Move faster on lineup-driven plays.

### Day 2 (2026-06-25)
- First real CLV data: Isak +1.56% (beat close, won), Match O2.5 −5.88% (worse, lost) — CLV agreed with both outcomes.
- PAR-AUS correlated cluster failed together on a 0-0 (4 bets). "Desperation→goals" is a weak inference.
- ERROR: Sweden "must-win" thesis was wrong (built on unverified qualification claim). → STANDING RULE added.

### Day 3 (2026-06-26)
- **Green day: 2-4-0, +0.31u cash.** Two winners (KDB G/A, France TT) outweighed four small losers.
- **STANDING RULE applied successfully** — EGY-IRN/CPV-KSA theses verified vs 3rd-place table before sizing.
- **"Both must win → goals" burned AGAIN:** CPV-KSA 0-0, second consecutive must-win game to bust under (after PAR-AUS). PATTERN, not one-off.
- **France TT O2.5 cashed; passing the France ML −175 was still correct** — took the +EV team-total instead of the efficient ML.

### Day 4 (2026-06-27) — final group matchday
- **Brutal day: 1-6-0, −5.23u cash.** Worst day of the tournament. Bankroll 102.31u → 97.08u.
- **Two last-minute beats define the day.** DZA-AUT: Algeria LED until the final kick, conceded → draw (bet 017 ML lost, Drawbreaker refunded 1.25u). CRO-GHA: level until a last-minute Croatia winner (bet 020 draw lost). BOTH theses were correct through 89 minutes and lost to stoppage-time variance. This is what holding the +EV side feels like on the wrong tail — do not over-correct the process off two late goals.
- **The one thesis that genuinely MISSED: JOR-ARG under (018).** Predicted rotated Argentina = quieter game; it went OVER. LESSON: even a rotated A-list side vs an outmatched, eliminated opponent is NOT a reliable under — talent gap can outweigh the motivation/rotation gap.
- **SGP clustering warning realized:** bets 018/019/023 all keyed on the same JOR-ARG script (under + Álvarez goal) and died together. The 20% SGP (023) added correlated exposure to legs we already held.
- **COL-POR U2.5 (021) was the lone winner** — the cagey controlled-game read (happy-draw Colombia + Portugal needs one goal) cashed.
- CLV not captured again (Days 3–4). The CLV scoreboard is still stuck at 2 measurable bets — the real gap in the process.

### 🔒 STANDING RULE (2026-06-25)
**Never base a play on an unverified qualification claim. If a thesis depends on "must win," "already through," "a draw eliminates them," best-third positioning, or any GD/tiebreaker math — VERIFY against actual standings + the live table BEFORE pricing. If the data isn't in hand, ASK. Directional reads may stay flagged low-confidence; hard qualification claims must be sourced.**

### 🔒 STANDING LESSON (2026-06-26)
**Mutual must-win games do NOT reliably go over. Two-for-two (PAR-AUS 0-0, CPV-KSA 0-0) busted under. Fear of losing makes these games tight. Treat "both must win" as neutral-to-under and require an independent reason for any over.**

### 🔒 STANDING LESSON (2026-06-27)
**Rotation/dead-rubber is NOT automatically an under. JOR-ARG went over despite heavy Argentina rotation — a large talent gap can produce goals regardless of motivation. Require the opponent's defense to be a real factor, not just "the favorite is resting," before backing an under on a rotation thesis.**

### 🔒 STANDING LESSON (2026-06-27b)
**Correlated singles + an overlapping SGP are ONE unit of risk, not several. When an SGP shares legs with bets already in the suite, size the whole correlated cluster as a single position. Day 4 ran ~3u of effectively the same JOR-ARG bet across three tickets.**
