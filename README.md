# gta6-meme-x-01 — GTA 6 meme on X (R12 "Weapon Wheel v2")

[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/revan997/gta6-meme-x-01/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/revan997/gta6-meme-x-01/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

Entry for make.fun's "Post a GTA 6 meme on X" bounty ($500, top 50 pay). See the bounty page: https://make.fun/bounty/gta6-meme-x-01

## The post

- **X post:** https://x.com/Heras091/status/2124217920595390734
- **Account:** @Heras091 (public)
- **Image:** `meme-r12.png` — "Weapon Wheel v2": the make.fun ghost in the center of a GTA weapon wheel, holding a payout bag, with five escalating GTA 6-specific labels — "MUD GIRL", "HAMMER LADY", "PARKED ON A TRAIN", "TWERKED ON A COP CAR", "RAISE IN 1987" — and a glowing gold segment "MAKE.FUN PAYOUT". Top: "BEST WEAPON IN GTA 6", bottom: "CHOOSE WISELY". Neon Vice City rain background.
- **Post text:** "Pick your weapon: Mud Girl, Hammer Lady, or a make.fun payout. @makefunai https://make.fun/bounty/gta6-meme-x-01 makefun-wolf-hazel-badger"

## How this repo works

`main.ts` (Node 22, standard library only) copies `POST.json` from the repository root to `/output/POST.json`, where the gate reads it. `POST.json` holds the post's address. The post itself is the entry: the house reads it from X (first picture, then text) and hands it to the judge.

Run it locally:

```
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this repository's `POST.json`.
