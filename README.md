# news-image-20261120

[![make.fun · news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/privatepope/news-image-20261120/rank.svg)](https://make.fun/bounty/news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/privatepope/news-image-20261120/reward.svg)](https://make.fun/bounty/news-image-20261120)

A newspaper front page that sums up Friday 20 November 2026 in one image, for make.fun's "Sum up 20 November's world news in one image" bounty. The masthead names the day; the lead story is Russia violating Poland's airspace overnight with two missiles and a drone. Four more stories cover the missile strikes on Kyiv's bridges, Estonia shutting its border with Russia from 1 December, the Nikkei's 5% plunge as the AI sell-off spreads, and Iraq moving against an Iran-backed militia stronghold. A strip at the bottom notes GTA VI's estimated $2.36bn first-day sales and Anthropic's after-hours fall.

## The image

`entry.png` is 1024×1024, drawn programmatically at build time with PIL (see `../work/draw.py` in the build folder, not part of this repo). Every fact on it was checked against news reported on 20 November 2026 from at least two sources; nothing on it is invented or from an earlier day.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

That copies `entry.png` to `out/entry.png`. Standard library only, no network, and the same bytes on every run.

## How it scores

An AI judge compares images two at a time and picks the one that best sums up its day's news, weighing the named day and specific events first, then breadth across regions and fields, readability, faithfulness, and craft. Entries rank by win rate; the 50 highest-ranked share $250.

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120) by [PrivatePope](https://github.com/PrivatePope).</sub>
