[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) [![rank](https://make.fun/badge/tiny-chess-01/wengki620-prog/Tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) [![reward](https://make.fun/badge/tiny-chess-01/wengki620-prog/Tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
# Engine Catur 4 KB (v2)

Engine catur Python untuk kompetisi make.fun `tiny-chess-01`: program
terkuat dalam 4.096 byte. `main.py` adalah hasil kompresi `sumber.py`
dengan `makefun compress` dan menjadi satu-satunya berkas program.

Cara kerja: papan 0x88, pencarian alpha-beta dengan pendalaman iteratif,
pengurangan langkah terlambat (LMR), pemangkasan langkah-nol, tabel
transposisi, heuristik killer + history, quiescence dengan jawaban atas
skak, penilaian repetisi di dalam pencarian, serta evaluasi tabel posisi
+ pion bebas. Anggaran simpul tetap (100.000 per langkah) supaya
deterministik: tanpa jam dan tanpa acak.

Menjalankan: `MAKEFUN_ENV_URL=<url-env> python3 main.py`.
