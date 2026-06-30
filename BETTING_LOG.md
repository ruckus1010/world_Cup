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
| 0.10u free bet | Drawbreaker on bet 014 (EGY-IRN draw) | 0.10u | ~0.07u | Deploy on a future longer-odds +EV play. |
| 1.25u free bet | Drawbreaker on bet 017 (DZA-AUT draw) | 1.25u | ~0.88u | Deploy on a longer-odds +EV play. |

## Settled Bets

| ID | Date | Match | Market | Selection | Odds | Fair % | Stake | Result | Payout (u) | Close | CLV | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 001 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia TT Over 2.5 | +154 | ~48–53% | 2.00u | WIN | +3.08u | TBD | TBD | Final 3-1. |
| 002 | 2026-06-24 | BIH–QAT | TOTAL | Bosnia −2.5 | +285 | ~38–43% | 0.50u | LOSS | −0.50u | TBD | TBD | Won by 2. |
| 003 | 2026-06-24 | SCO–BRA | PROP | Vinicius Jr anytime | +110 | ~50–55% | 1.00u | WIN | +1.10u | TBD | TBD | Usage thesis cashed. |
| 004 | 2026-06-24 | MAR–HTI | PROMO/PROP | Brahim Díaz anytime (live) | +324 | ~28–34% | 0.50u | LOSS | −0.50u | n/a | n/a | Live dart. |
| 005 | 2026-06-25 | JPN–SWE | PROMO/PROP | Isak 2+ SoT | +282 | ~27–32% | 1.00u | WIN | +2.82u | +220 | **+1.56%** | BEAT close. |
| 006 | 2026-06-25 | JPN–SWE | TOTAL | Sweden TT Over 1.5 | +230 | ~30–40% | 1.00u | LOSS | −1.00u | TBD | TBD | 1-1; SWE only 1. |
| 007 | 2026-06-25 | PAR–AUS | TOTAL | Match Over 2.5 | +286 | ~36–44% | 0.50u | LOSS | −0.50u | +240 | **−5.88%** | 0-0. WORSE than close. |
| 008 | 2026-06-25 | PAR–AUS | ML+PROMO | Paraguay ML (Drawbreaker) | +165 | ~36% | 1.00u | LOSS (refunded) | −1.00u | TBD | TBD | Drawbreaker 1.0u bonus refunded. |
| 009 | 2026-06-25 | PAR–AUS | TOTAL | Paraguay TT Over 1.5 | +255 | ~34–45% | 1.00u | LOSS | −1.00u | TBD | TBD | 0-0 cluster. |
| 010 | 2026-06-25 | PAR–AUS | SGP/PROMO | 3-leg O2.5+BTTS+Enciso | +910 | ~10–11.5% | 0.50u | LOSS | −0.50u | TBD | TBD | 0-0 cluster. |
| 011 | 2026-06-26 | URU–ESP | TOTAL | Match Over 2.5 | +156 | ~47–55% | 0.50u | LOSS | −0.50u | TBD | TBD | 1-0 final. |
| 012 | 2026-06-26 | NZL–BEL | PROMO/PROP | De Bruyne G/A | −139 | ~62–70% | 1.00u | WIN | +0.72u | TBD | TBD | BEL dominance cashed. |
| 013 | 2026-06-26 | CPV–KSA | TOTAL | Match Over 2.5 | +110 | ~50–58% | 0.50u | LOSS | −0.50u | TBD | TBD | 0-0. Second must-win to bust. |
| 014 | 2026-06-26 | EGY–IRN | ML+PROMO | Egypt ML (Drawbreaker) | +150 | ~38% | 0.10u | LOSS (refunded) | −0.10u | TBD | TBD | Draw → 0.10u bonus refunded. |
| 015 | 2026-06-26 | NOR–FRA | TOTAL | France TT Over 2.5 | +139 | ~40–50% | 0.50u | WIN | +0.70u | TBD | TBD | France 3+. |
| 016 | 2026-06-26 | URU–ESP | PROP | Oyarzabal anytime | +155 | ~43% | BONUS 1.0u | LOSS | 0.00u (bonus) | TBD | TBD | Bonus consumed. |
| 017 | 2026-06-27 | DZA–AUT | ML+PROMO | Algeria ML (Drawbreaker) | +295 | ~24% | 1.25u | LOSS (refunded) | −1.25u | TBD | TBD | Algeria led to last kick → Drawbreaker 1.25u refunded. |
| 018 | 2026-06-27 | JOR–ARG | TOTAL | Match Under 2.5 | +160 | ~37% | 1.00u | LOSS | −1.00u | TBD | TBD | Went OVER. Rotation-under MISSED. |
| 019 | 2026-06-27 | JOR–ARG | PROP/PROMO | Álvarez anytime | +113.6 | ~52% | 1.00u | LOSS | −1.00u | TBD | TBD | No goal. |
| 020 | 2026-06-27 | CRO–GHA | ML/PROMO | Draw | +273 | ~33% | 0.50u | LOSS | −0.50u | TBD | TBD | Draw until 90'+ Croatia winner. |
| 021 | 2026-06-27 | COL–POR | TOTAL | Match Under 2.5 | +105 | ~46% | 0.50u | WIN | +0.525u | TBD | TBD | Cagey-game under confirmed. |
| 022 | 2026-06-27 | PAN–ENG | SGP/PROMO | Rashford ATGS + Saka G/A + O2.5 | +436 | ~25% | 1.00u | LOSS | −1.00u | TBD | TBD | Did not hit. |
| 023 | 2026-06-27 | JOR–ARG | SGP/PROMO | U2.5 + Álvarez + ARG win | (20% boost, price not captured) | ~20% | 1.00u | LOSS | −1.00u | TBD | TBD | Correlated cluster failure. |
| **024** | **2026-06-29** | **GER–PAR** | **TOTAL** | **Match Under 2.5** | **+110** | **~45%** | **1.50u** | **WIN** | **+1.65u** | **TBD** | **TBD** | **Public-inflated-over thesis CONFIRMED. 97/3 public on GER drove over to −140, left under +110 soft. PAR bunkered, dragged to PKs, won. Cleanest pre-slate edge of the day.** |
| **025** | **2026-06-29** | **BRA–JPN** | **SGP/PROMO** | **Brazil ML + Over 2.5 + Vinicius G/A 1+** | **+410** (base ~+315 × 30% boost) | **~20%** | **1.00u** | **LOSS** | **−1.00u** | TBD | TBD | Version C of slip. Did not hit. |
| **026** | **2026-06-29** | **NED–MAR** | **PROP/PROMO** | **Brahim Díaz 2+ total shots (incl ET)** | **−176** (base −220 × 25% boost) | **~66–70%** | **0.50u** | **LOSS** | **−0.50u** | TBD | TBD | Did not hit. |
| **027** | **2026-06-29** | **NED–MAR** | **SGP/PROMO** | **NED To Qualify + U2.5 + Gakpo G/A 1+** | **+715** (base +550 × 30% boost) | **~13%** | **0.994u** ($9.94) | **LOSS** | **−0.994u** | TBD | TBD | U2.5 + Gakpo legs locked at 90' (1-1, Gakpo scored). Reduced to NED To Qualify live bet. Morocco won PKs → SGP loses. Hedged separately (028). |
| **028** | **2026-06-29** | **NED–MAR** | **ML (hedge)** | **Morocco To Qualify** | **−105** | **~52% live** (~55–58% true) | **4.151u** ($41.51) | **WIN** | **+3.951u** | TBD | TBD | LIVE HEDGE on bet 027 at end of regulation. Locked +$29.56 either way. Morocco won on PKs. Combined 027+028 net: +2.957u on the game vs −0.994u unhedged. Pure variance reduction with directional logic (stats: MAR 65% poss, 0.65 xG to NED 0.23). |

## Running Tallies

| Metric | Value |
|---|---|
| Total bets placed | 28 (all settled) |
| Win / Loss / Push | 8 / 20 / 0 |
| Units staked (cash) | 25.99u |
| Net P/L (cash) | +0.19u |
| ROI on stakes | +0.73% |
| Outstanding free bets | 1.35u (0.10u + 1.25u) (~0.95u EV) |
| **Rolling CLV (measurable)** | **−2.16% avg over 2 bets; beat close 1 of 2 (Day 3–5 closes not captured)** |

## Process Notes

### Day 1 (2026-06-24)
- CLV capture FAILED (3 bets permanent TBD).

### Day 2 (2026-06-25)
- First real CLV data. PAR-AUS correlated cluster failed together on 0-0 (4 bets).
- ERROR: Sweden "must-win" thesis was wrong (unverified qualification claim). → STANDING RULE added.

### Day 3 (2026-06-26)
- Green day: 2-4-0, +0.31u. STANDING RULE applied successfully.
- "Both must win → goals" burned AGAIN (CPV-KSA 0-0).

### Day 4 (2026-06-27)
- Worst day: 1-6-0, −5.23u. Two last-kick beats (DZA-AUT, CRO-GHA) on correct theses. JOR-ARG rotation-under genuinely missed.
- SGP clustering warning realized in JOR-ARG cluster.

### Day 5 (2026-06-29) — R32, first knockout slate
- **+3.11u day, back above 100u starting bankroll for first time since Day 3.** Two wins (GER-PAR Under, MAR hedge) outweighed three losses (Brazil SGP, Diaz shots, NED SGP).
- **GER-PAR Under +110 (bet 024) was the cleanest pre-slate edge identified all tournament** — public-inflated favorite + bunker-script underdog created standalone +EV on the under. Paraguay played exactly to script: parked the bus, took it to PKs. THESIS CONFIRMED. Pattern (NEW STANDING LESSON): heavy-public-favorite vs defensive-dog at high totals systematically softens the under.
- **NED-MAR live hedge (bet 028) is a process highlight, not a hero call.** Once Under 2.5 + Gakpo G/A were effectively locked at 90', the SGP reduced to "NED To Qualify" with Morocco *favored* live at −105 — a flip from pregame +120. Hedge locked +$29.56 either way and directionally agreed with the in-match dominance signal (MAR 65% poss, 2.8x xG, +4 SoT). Converted what would have been −0.994u into +2.957u on the game. Worth keeping the "lock the structurally-equivalent profit when the live price has materially flipped" pattern as a standing tool.
- **CRITICAL FRAMING — record vs cash divergence.** Day 5 W-L was 2-3, cash was +3.11u. The "loss" on bet 027 was structurally a profit-lock paired with bet 028. The W-L ledger is a misleading scoreboard when SGPs are combined with deliberate hedges. We're 8-20 W-L but +0.19u cash — variance has been mostly against us, hit rate consistent with edge but win-rate-of-record looks worse than the bottom line.
- Brazil SGP and Diaz shots: small−EV losses that are part of the cost of doing business. No process flaw, no thesis miss worth flagging.
- CLV STILL not captured (Days 3–5). The single biggest unresolved process gap.

### 🔒 STANDING RULE (2026-06-25)
**Never base a play on an unverified qualification claim. VERIFY against actual standings + live table BEFORE pricing.**

### 🔒 STANDING LESSON (2026-06-26)
**Mutual must-win games do NOT reliably go over.** Two-for-two busted under.

### 🔒 STANDING LESSON (2026-06-27)
**Rotation/dead-rubber is NOT automatically an under.** JOR-ARG went over despite heavy ARG rotation; talent gap > rotation effect.

### 🔒 STANDING LESSON (2026-06-27b)
**Correlated singles + overlapping SGP are ONE unit of risk, not several.** Size the cluster as a single position.

### 🔒 STANDING LESSON (2026-06-29) — NEW
**Heavy public action on a favorite + high posted total systematically softens the UNDER, especially in knockouts where the dog's modal game plan is bunker→PKs.** GER-PAR Under +110 confirmed the pattern. Recreational fav+over parlays inflate the over and leave the under priced for sharps. Look for this spot specifically: ≥80% public on fav + total at or above 2.5 + defensive-dog matchup = under is the +EV side.

### 🔒 STANDING LESSON (2026-06-29b) — NEW
**Late-in-the-game SGP hedging is a real tool when the live line has flipped vs pregame.** If the SGP's remaining-risk leg has a market price that disagrees materially with the pregame number AND the in-match data supports the flip, the hedge isn't "locking a loss" — it's monetizing a price move on the only live leg. The NED-MAR hedge converted −0.994u into +2.957u on a coherent read (Morocco dominated through 90', live price reflected it, hedge captured it). Use this when: (1) most SGP legs are effectively settled, (2) the live line on the unsettled leg has moved materially from pregame, (3) underlying match stats support the line move.
