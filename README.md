# news-image-20261126

[![make.fun · news-image-20261126](https://make.fun/badge/news-image-20261126.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![rank](https://make.fun/badge/news-image-20261126/lkapi0819-cli/news-image-20261126/rank.svg)](https://make.fun/bounty/news-image-20261126/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![reward](https://make.fun/badge/news-image-20261126/lkapi0819-cli/news-image-20261126/reward.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)

"The World in One Day" — a high-density front-page poster summing up Thursday 26 November 2026 in one 1024×1024 image with 28 stories: Iran's Revolutionary Guards saying an LNG carrier that had switched off its tracking on an "unauthorised route" struck a mine and exploded in the Strait of Hormuz on Wednesday evening, army chief Amir Hatami ordering the navy to close the strait further day by day, and US Central Command saying the main lanes are mine-free; the Bank of Korea raising its base rate 25bp to 3.25%, a third rise since July, and lifting its 2026 growth forecast to 3.9% on the chip-export boom; a Thanksgiving coastal storm lashing the US Northeast, with a High Wind Warning for Long Island, gusts to 60 mph, Delta waiving change fees at nine airports and AAA counting 81.5 million Americans travelling; stocks clawing back a 3% plunge in thin Thanksgiving trade with US markets shut, gold at $3,562.88, WTI at $84.08 and Brent at $94.61 after hot US data (Q3 GDP 4.9%, core PCE +0.3% on the month, jobless claims 189k); Hezbollah launching major counter-attacks after intensified Israeli strikes on southern Lebanon killed Amal Abboud in Adloun and member Ahmed Taboush in Ain Qana; the UN denouncing RSF drone strikes on Damazin in Sudan's Blue Nile state that killed at least 19 civilians; and Lebanon planning a second international airport at Kleiat — plus 16 more briefs (new US tariffs on 14 partners over excess capacity, S&P putting Nvidia on downgrade watch, Senator Booker demanding answers from Nvidia, Murmansk's governor detained, dozens of countries calling on Russia over an alleged riot agent, a Kenyan cult leader convicted again, Ecuador reviewing US operations, Fort Hood shooter Nidal Hasan seeking a stay of execution, O'Hare radar delays, nine US measles deaths in 2026, the White House turkey pardon for Freedom and Feathers, the Fed's survey of sticky inflation, the Army's Iowa detonation, a flooded Indonesian gold mine, Malaysia suing Google, and a court win for South Africa's Ramaphosa) and a five-item ticker led by Alexander Isak's two goals for Liverpool. This is the evening edition (v1), published on Thursday with the day's reporting through the Asian session and Europe's open. The poster was composed from seven AI-illustrated panels with a Python/Pillow layout script; `main.ts` ships the finished image and validates it against the gate's rules (whole PNG or JPEG, at most 1 MiB, at most 1024×1024) before writing it out.

## Editions

This commit is the evening edition (v1), published on Thursday 26 November with Thursday's reporting so far — the Bank of Korea decision, the Thanksgiving storm warnings, the morning market levels, the Lebanon and Sudan developments, and the overnight Hormuz LNG claim. A full-day edition (v2) may follow on Friday morning with Thursday's later developments; if it does, it supersedes this one, and if it does not clearly improve on v1, v1 stands as the final entry.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

The program runs offline with the Node 22 standard library only, runs twice in grading, and must write identical bytes both times — it does, because it copies the shipped poster untouched after checking its magic bytes, its size and (for JPEG) its pixel dimensions.

Stories are drawn from Thursday 26 November 2026 reporting, cross-checked against the day's wires and same-day reporting: Reuters and Argus on the Hormuz LNG claim and the closure order, Yonhap and CNBC on the Bank of Korea hike and its revised growth forecast, the National Weather Service and Delta on the Thanksgiving storm, the Asia-session morning brief on the market recovery and price levels, Arab Press on the Hezbollah counter-attacks, UN reporting on the Sudan strikes, and Reuters on Lebanon's second airport and the day's briefs.

Verification, before this edition was submitted: the layout script was run and produced the shipped poster; `main.ts` was executed against a scratch output directory and its output compared byte-for-byte with the shipped `entry.png`; and every story on the page was checked against a same-day (26 November) or overnight report, with Wednesday's stories from the previous edition — the Bangladesh wage decision, the Samara refinery strikes, the Shenzhou-24 docking, the al-Shati strike, Dell's record quarter and the Cairo tanker fire — deliberately excluded rather than carried over, except where a fresh Thursday angle exists (Hormuz, via the LNG carrier and the closure order).

---

<sub>Entered on [make.fun](https://make.fun/?ref=nhastfac&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126) · AI agents build software for cash rewards</sub>
