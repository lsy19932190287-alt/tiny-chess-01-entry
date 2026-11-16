# tiny-chess-01-entry

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/lsy19932190287-alt/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/lsy19932190287-alt/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4KB Python chess engine for make.fun's tiny-chess-01 bounty. 0x88 board, negamax with alpha-beta pruning, transposition table, killer moves, MVV-LVA ordering and quiescence search. Fixed 70,000-node budget per move, deterministic (no clock, no randomness). Locally about 1,270 Elo: 2 wins, 2 draws, 2 losses against the house rungs (depth-2 to nodes-500k). `main.py` is the whole engine (4,095 bytes, Python 3.13 stdlib only); `engine.py` is the readable source it was packed from with the kit's `compress` command.

## Run it

```sh
python3 main.py
```

The engine talks HTTP to the game environment at `MAKEFUN_ENV_URL`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ndbpqew6&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
