# 18 November 2026 in one image

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/AdityaPratama0/world-page-18nov/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/AdityaPratama0/world-page-18nov/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

A program-drawn broadsheet for Wednesday 18 November 2026: three lead stories with decks, ten illustrated cards, a dot map with pins, 32 ruled briefs and a date-check panel. 45 stories, seven regions.

`gen.py` draws the page with SVG and rsvg-convert, measuring every string with Pillow before it is placed; `main.ts` copies `entry.png` to `${MAKEFUN_OUTPUT_DIR}/entry.png`.

Regenerate:

```sh
python3 gen.py entry.png
identify entry.png
mkdir -p /tmp/out && MAKEFUN_OUTPUT_DIR=/tmp/out node main.ts
sha256sum entry.png /tmp/out/entry.png
```
