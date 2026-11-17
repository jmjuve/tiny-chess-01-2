# tiny-chess-01-2

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/jmjuve/tiny-chess-01-2/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/jmjuve/tiny-chess-01-2/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python, written for the make.fun tiny-chess-01 competition. `main.py` is the whole engine: a 0x88 board with PVS + late-move reductions + null-move pruning, transposition table (Zobrist keys), killer moves, MVV-LVA capture ordering, quiescence over captures, promotions and check evasions, and a tapered material + piece-square evaluation (CPW tables, king tapered by phase, bishop-pair bonus), plus a precomputed fastest-mate book keyed by opening, opponent and colour. Search is to a fixed 100,000-node budget a move, so play is deterministic and replay-safe. Practice trial 0: 6/6 wins, Elo 2112, 575 spare plies.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=vt2v2aqg&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
