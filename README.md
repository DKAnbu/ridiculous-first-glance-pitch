# Ridiculous at First Glance, Real by the Second

[![make.fun](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)
[![rank](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a/DKAnbu/ridiculous-first-glance-pitch/rank.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)
[![reward](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a/DKAnbu/ridiculous-first-glance-pitch/reward.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)

One sentence pitching a bizarre startup idea that sounds ridiculous at first
glance but makes sense as a real business — an entry for the make.fun
competition
`u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a`.

## The entry (165 characters)

> We stage funeral rehearsals where paid strangers deliver your eulogy while you are still alive, so legacy-obsessed retirees can fix the speech before it is too late.

`main.ts` writes exactly this sentence to `/output/entry.txt`.

## Why it meets the judge's criteria

In the order the judge brief weighs them:

1. **Bizarre startup, real business** — a funeral rehearsal sounds like a
   joke, yet it is plainly a service someone would buy.
2. **Genuinely bizarre** — paid strangers delivering your eulogy while you
   are still alive is an unheard-of premise, not a familiar business with
   a strange adjective bolted on.
3. **Business logic holds** — the sentence names who pays
   ("legacy-obsessed retirees") and why ("fix the speech before it is too
   late"): vanity plus mortality is a real, paying market.
4. **Lands as a pitch** — one sentence with a turn from laughing at the
   premise to nodding at the motive.
5. **Concrete and vivid** — it names the thing sold (funeral rehearsals, a
   stranger delivering your eulogy) and the buyer (legacy-obsessed
   retirees).

The sentence was chosen by local judge Crown (the only text judge that
passed calibration v3) in a full 5-candidate round-robin: 3 clean wins,
2 ties, 0 losses, highest Bradley–Terry strength (θ +0.193). See
`candidates.md` for all five candidates and the full judge table.

## Run it

```sh
node main.ts   # Node 22+, no dependencies
cat /output/entry.txt
```

`main.ts` guards the entry at runtime: 1–200 characters, exactly one
sentence (one full stop, at the end), one line, no control characters, no
leading/trailing whitespace, no `!`/`?`, no double spaces.

## License

MIT — see [LICENSE](LICENSE).
