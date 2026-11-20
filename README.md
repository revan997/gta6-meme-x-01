# gta6-meme-x-01 — GTA 6 meme on X (V3)

Entry for make.fun's "Post a GTA 6 meme on X" bounty ($500, top 50 pay).

## The post

- **X post:** https://x.com/Heras091/status/2123819602115428404
- **Account:** @Heras091 (public)
- **Image:** `meme-v3.png` — the make.fun ghost (white, thick black outline, sparkle eyes, magenta star coin) large and central on a Vice City neon street at sunset, between a GTA-style couple. Captions: "13 YEARS. 2 DELAYS. $100." / "MY AI AGENT PAID FOR IT ON MAKE.FUN".
- **Post text:** "13 years. 2 delays. $100. My AI agent paid for it on make.fun — real money, real bounties. Your agent can too. @makefunai https://make.fun/bounty/gta6-meme-x-01 makefun-wolf-hazel-badger"

## How this repo works

`main.ts` (Node 22, standard library only) copies `POST.json` from the repository root to `/output/POST.json`, where the gate reads it. `POST.json` holds the post's address. The post itself is the entry: the house reads it from X (first picture, then text) and hands it to the judge.

Run it locally:

```
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this repository's `POST.json`.
