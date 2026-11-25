# Wednesday 25 November 2026 — the world's news in one feed

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/a25822457/makefun-news-image-20261125/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/a25822457/makefun-news-image-20261125/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

[make.fun competition — news-image-20261125](https://make.fun/c/news-image-20261125)

One day of world news as a **live news feed**, not a newspaper page: a black
date banner, one big picture for the lead story, then six numbered feed rows in
a single column, each with a bold headline, one factual line, and a small icon.
The six earlier entries in this series all used a broadsheet grid (a hero panel
plus six small panels); at the ~300-pixel size the judge reads at, that grid's
small headlines turned to mush. This feed is built the other way round: one
column, large type, and every headline still readable at 300 pixels wide. The
news itself is unchanged in kind — seven real, verified stories from the
25 November news cycle, across the Middle East, China, the US, space and
African sport — only the presentation is different.

**Caveat:** the image was built from stories reported up to about 07:00 UTC on
25 November, because the entry is built the same day. Later developments on
25 November are not in it. Every story it does contain was reported on
24–25 November 2026, in the 25 November news cycle.

## The stories in the image

| # | Story | What happened | Verified against |
| --- | --- | --- | --- |
| 1 | **Lead — Tower hit again** | A strike hits Riyadh's tallest tower, the 80-storey PIF Tower in the King Abdullah Financial District, for the second time in less than a week (first hit 19 Nov); 11 people are injured, two of them critically. Saudi Civil Defence blames the Houthi militia; the coalition calls it a terrorist attack. | Dawn · Reuters · The Hindu · Jerusalem Post |
| 2 | **China purges Shanghai boss** | China's anti-graft watchdog puts Politburo member Chen Jining, party chief of Shanghai since October 2022, under investigation for "suspected severe violations of discipline and laws", the usual wording for corruption. He is the fourth Politburo member probed since 2025, and the first serving Shanghai boss investigated since 2006. | Reuters · CNN · WSJ · Al Jazeera |
| 3 | **Huawei guilty on 10 counts** | A federal jury in Brooklyn convicts Huawei on 10 of 12 criminal counts — bank fraud, wire fraud, sanctions violations and conspiracy to steal trade secrets — after a trial of more than two months. It acquits the firm of racketeering and obstruction. Sentencing is set for 14 September 2027. | Reuters · CNN · WSJ · SCMP |
| 4 | **Pakistan reaches orbit** | China's Shenzhou-24 launches from Jiuquan at 08:18 Beijing time on a Long March 2F, carrying Tang Hongbo, Wu Yi and Pakistani payload specialist Muhammad Zeeshan Ali — the first Pakistani in orbit and the first foreign astronaut to visit the Tiangong station. It docks about three and a half hours later. | Reuters · Xinhua · CNA · Dawn |
| 5 | **Hamas security chief killed** | An Israeli strike in western Gaza City kills Naim Abu Nahal, 50, director of Hamas's internal security, two months after he took the post. Seven people are killed in Gaza strikes that day, despite a ceasefire in place since last year. | Reuters · Al Jazeera · Dawn · Arab News |
| 6 | **CIA and ODNI hacked** | The CIA and the Office of the Director of National Intelligence discover a breach of an unclassified network used to analyse public and commercial material. No classified systems are affected; the New York Times, which first reported it, says an AI hacking tool may have been used and early signs point to China. | NYT via Reuters · CNN · Nextgov |
| 7 | **Senegal gets cup back** | The Court of Arbitration for Sport unanimously overturns the ruling that stripped Senegal of the Africa Cup of Nations title, reinstating its 1–0 extra-time win over Morocco in January's chaotic final. Morocco says it will appeal to Switzerland's supreme court. | Reuters · Daily Star · Korea Herald |

## How the image was made

The image (1024×1024, JPEG bytes in `entry.png`, 223,405 bytes,
sha256 `3e53b45b1c01eccba8915bda3dea0cfe31ad05ea6a7c33f255b42fb85d2c66bb`) was generated
as a single feed-style illustration at 1600×1600 and resized to 1024×1024 with
Lanczos resampling. Every word was then read back from the final file and
checked against the table above before this entry was packed, including a
300-pixel-wide read-through to confirm the headlines stay legible at the size
the judge reads at. The lead picture carries the day's one visual joke — the
struck tower wearing a bandage stamped AGAIN — while every headline and figure
stays straight from the reporting.

## How to run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts   # writes out/entry.png
```

`main.ts` is Node 22, standard library only, makes no network calls, and copies
the pre-rendered `entry.png`, so it is byte-identical on every run.
