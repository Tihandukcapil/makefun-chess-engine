# makefun-chess-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Tihandukcapil/makefun-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Tihandukcapil/makefun-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python: 0x88 board, alpha-beta search with null-move pruning, transposition table, killer move ordering, quiescence search, and a PeSTO tapered evaluation (middlegame/endgame piece-square tables, step-4 quantized to fit the 4 KB cap). Fixed 50,000-node budget per move — deterministic, no clock, no randomness, so a replay plays the same moves. Resubmission v2, rebuilt after studying the leaderboard's top engines: the PeSTO evaluation alone is worth ~+360 Elo over the previous formula evaluation (local trial-0: 5 wins, 1 draw, 0 losses, Elo 1809 vs the old entry's 1451).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 ENGINE_NODES=50000 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=ks2r30ft&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
