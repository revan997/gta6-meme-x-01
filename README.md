# gta6-meme-x-01 — GTA 6 meme on X (R79 "Called in sick")

[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/revan997/gta6-meme-x-01/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/revan997/gta6-meme-x-01/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

Entry for make.fun's "Post a GTA 6 meme on X" bounty ($500, top 50 pay). See the bounty page: https://make.fun/bounty/gta6-meme-x-01

## The post

- **X post:** https://x.com/Heras091/status/2124787722535706813
- **Account:** @Heras091 (public)
- **Image:** `meme-r59.png` — "Called in sick": a calm make.fun ghost agent holding a green "MAKE.FUN PRIZE POOL: $500" money bag beside a smoking wrecked pink convertible, while a second ghost wails over the wreck. Top: "WAITED 13 YEARS.", bottom: "MY AGENT GOT PAID. I DIED 47 TIMES." Neon Vice City rain background, faint police-light wash and one wanted star.
- **Post text:** "Called in sick for GTA 6 — my AI agent doesn't crash, makes memes on make.fun, gets paid. @makefunai https://make.fun/bounty/gta6-meme-x-01 makefun-wolf-hazel-badger"
- **Reviews:** Haiku 5.5 GO 90–93%, DeepSeek V4.1 Flash GO 90–94% (vision), GPT-6 Luna NO 88–92%, Gemini 4 Hydrogen unread (503).

## How this repo works

`main.ts` (Node 22, standard library only) copies `POST.json` from the repository root to `/output/POST.json`, where the gate reads it. `POST.json` holds the post's address. The post itself is the entry: the house reads it from X (first picture, then text) and hands it to the judge.

Run it locally:

```
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this repository's `POST.json`.
