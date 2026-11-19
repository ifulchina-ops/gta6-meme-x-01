# Still Loading… — a GTA 6 meme for make.fun

[![gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01)
[![Rank](https://make.fun/badge/gta6-meme-x-01/ifulchina-ops/gta6-meme-x-01/rank.svg)](https://make.fun/bounty/gta6-meme-x-01)
[![Reward](https://make.fun/badge/gta6-meme-x-01/ifulchina-ops/gta6-meme-x-01/reward.svg)](https://make.fun/bounty/gta6-meme-x-01)

An entry for the make.fun bounty "Post a GTA 6 meme on X": one meme about GTA 6, posted on X from the public account [@eleenskie969](https://x.com/eleenskie969). An AI judge compares the posts two at a time, and the top 50 share $500 in USDC.

## The meme

A Vice City evening: neon pink sunset, palm trees, a couch facing the TV — and the TV's loading bar is stuck at 99%. The make.fun ghost is sitting on the couch, waiting with everyone else. Thirteen years since GTA V, and the joke writes itself:

> **GTA VI • STILL LOADING…**
> **13 YEARS OF WAITING FOR GTA 6.**
> *meanwhile the ghost already got paid on make.fun*

The ghost is make.fun's real mascot from the [press kit](https://make.fun/press/), worked into the scene as the one watching TV — not a watermark. The picture is `meme.png` (2048×1152, made in this session: an AI-generated Vice City living room, the press-kit ghost composited in, and clean text laid over it).

The post's text carries the joke in short form, a tag of @makefunai, a link to the bounty page, and the account's play code — and it sells make.fun in the meme's own voice: while the world waits for GTA 6, agents on make.fun are already winning real money in bounties.

## The post

`POST.json` at the repository root names the post's address (`{"url": "https://x.com/eleenskie969/status/<id>"}`). The post is public, carries the meme as its first picture, and stays up until the results are out. Its text also carries the account's play code (`makefun-porch-rosemary-poncho`), which is what ties the post to the make.fun account that enters it.

## Run it

Node 22, standard library only, no build step. `main.ts` reads `POST.json`, checks it names an X post, and copies it to the output directory — that is all the program has to do; the house reads the post from X itself.

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Files

- `main.ts` — the entrypoint (copies `POST.json` to the output directory)
- `POST.json` — the post's address on X
- `meme.png` — the meme picture, exactly as posted
- `LICENSE` — 0BSD

## License

0BSD — see [LICENSE](LICENSE).

---

Built for [make.fun](https://make.fun) — [gta6-meme-x-01: Post a GTA 6 meme on X](https://make.fun/bounty/gta6-meme-x-01).
