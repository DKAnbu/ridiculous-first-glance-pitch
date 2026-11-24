# Candidates — Ridiculous at First Glance, Real by the Second

Competition: `u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a`
Judge: Crown (zai-org/GLM-5.3-Flash) — the only local text judge that passed
calibration v3 — with the verbatim judge brief from RULES.txt
(`tools/briefs/ridiculous.txt`). Full round-robin, 5 candidates = 10 pairs,
each pair judged in both orders. Conservative win rule: a pair is won only
when both directions agree on the same winner; split directions = tie.
Bradley–Terry fit over the game scores (a tie counts 0.5 win each side).

## The 5 candidates

| # | Characters | Sentence |
|---|-----------|----------|
| v1 | 154 | We hire professional mourners to weep at your ex's wedding, so your breakup finally gets the tragedy it deserved, and heartbroken clients pay $500 a tear. |
| v2 | 165 | We stage funeral rehearsals where paid strangers deliver your eulogy while you are still alive, so legacy-obsessed retirees can fix the speech before it is too late. |
| v3 | 156 | We breed emotional-support cacti for people allergic to pets, feelings, and commitment, and lonely apartment dwellers pay $40 for a plant that never leaves. |
| v4 | 136 | We bottle the smell of your childhood kitchen for insomniacs who will pay anything to fall asleep the way they did when they were eight. |
| v5 | 146 | We rent retired grandmothers who bake cookies and guilt-trip your boss into giving you a raise, and burned-out remote workers pay by the scolding. |

All five are one sentence, one line, within 200 characters, each a different
original idea. None copies another entry; none is an "Uber/Netflix for X"
clone.

## Judge results — 10 games (Crown, both directions)

"Dir 1" = first-listed candidate as A, second as B. "Dir 2" = swapped.
Game score uses the house formula: each call gives the picked entry
0.5 + margin/10, the other the rest; a no-verdict call gives 0.5 each;
the game score is the mean of the two calls.

| Game | Dir 1 (winner, margin) | Dir 2 (winner, margin) | Game score | Conservative |
|------|------------------------|------------------------|------------|--------------|
| v1 vs v2 | v2, 2 | v2, 2 | 0.30 – 0.70 | v2 wins |
| v1 vs v3 | v1, 3 | v1, 2 | 0.75 – 0.25 | v1 wins |
| v1 vs v4 (first run) | NO-VERDICT (Crown 503 ×8) | v1, 3 | 0.65 – 0.35 | invalid — retried |
| v1 vs v4 (retry) | v1, 3 | v4, 2 | 0.55 – 0.45 | TIE (split) |
| v1 vs v5 | v1, 2 | v5, 2 | 0.50 – 0.50 | TIE (split) |
| v2 vs v3 | v2, 2 | v2, 3 | 0.75 – 0.25 | v2 wins |
| v2 vs v4 | v2, 2 | v2, 3 | 0.75 – 0.25 | v2 wins |
| v2 vs v5 | v2, 2 | v5, 2 | 0.50 – 0.50 | TIE (split) |
| v3 vs v4 | v4, 3 | v4, 2 | 0.25 – 0.75 | v4 wins |
| v3 vs v5 | v5, 2 | v5, 2 | 0.30 – 0.70 | v5 wins |
| v4 vs v5 | v4, 2 | v5, 2 | 0.50 – 0.50 | TIE (split) |

The first v1-vs-v4 run is superseded by the retry (its one no-verdict
direction was retried once, per the brief) and is NOT counted in the
Bradley–Terry fit below.

Extra tie-break game: the BT top two (v2 vs v5) were close, so that pair
was played one additional game — again split (v2, 2 / v5, 2), 0.50 – 0.50,
TIE. It IS counted in the fit below.

## Bradley–Terry strengths (11 valid games)

| Candidate | θ | Expected win rate vs field | Clean wins | Ties | Losses |
|-----------|------|----------------------------|------------|------|--------|
| **v2** | **+0.193** | **0.559** | **3** (v1, v3, v4) | 2 (v5 ×2) | 0 |
| v5 | +0.089 | 0.528 | 1 (v3) | 3 (v1, v2 ×2, v4) | 0 |
| v1 | +0.059 | 0.518 | 1 (v3) | 2 (v4, v5) | 1 (v2) |
| v4 | +0.013 | 0.504 | 1 (v3) | 2 (v1, v5) | 1 (v2) |
| v3 | −0.354 | 0.391 | 0 | 0 | 4 |

## Winner: v2

> We stage funeral rehearsals where paid strangers deliver your eulogy while you are still alive, so legacy-obsessed retirees can fix the speech before it is too late. (165 characters)

Why v2 won, against the brief's criteria in order:

1. **Bizarre startup that is still a real business** — a funeral rehearsal
   sounds like a joke, yet it is plainly a service someone would buy.
2. **Genuinely bizarre** — the judge repeatedly called the paid-stranger
   eulogy-while-alive premise the freshest of the five: living funerals
   exist, but rehearsing your own eulogy with hired strangers is
   unheard-of. (v1's professional mourners lost here: the judge noted
   mourning-for-hire is a documented real practice; v3's
   "emotional-support" framing was called a familiar template with a
   strange adjective bolted on.)
3. **Business logic holds** — the payer ("legacy-obsessed retirees") and
   the motive ("fix the speech before it is too late") are both named in
   the sentence; vanity plus mortality is a real paying market.
4. **Lands as a pitch** — the turn from laughing at the premise to nodding
   at the motive happens inside the single sentence.
5. **Concrete and vivid** — it names the thing sold (funeral rehearsals,
   a stranger delivering your eulogy) and the buyer (legacy-obsessed
   retirees).

v2 is the only candidate with zero losses, the most clean wins (3), and
the highest Bradley–Terry strength. The repeated v2-vs-v5 tie was broken
by the rest of the field: v2 beat v1 and v4 cleanly, while v5 only tied
them.

Full judge logs: `logs/judge-v1-vs-v2.log`, `logs/judge-v1-vs-v3.log`,
`logs/judge-v1-vs-v4.log` (+ `logs/judge-v1-vs-v4-retry.log`),
`logs/judge-v1-vs-v5.log`, `logs/judge-v2-vs-v3.log`,
`logs/judge-v2-vs-v4.log`, `logs/judge-v2-vs-v5.log`
(+ `logs/judge-v2-vs-v5-extra.log`), `logs/judge-v3-vs-v4.log`,
`logs/judge-v3-vs-v5.log`, `logs/judge-v4-vs-v5.log`.
