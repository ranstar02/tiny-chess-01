# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ranstar02/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ranstar02/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact Python chess engine for the make.fun tiny-chess-01 bounty.

- 0x88 board, alpha-beta + quiescence, transposition table, MVV-LVA
  captures + killer move ordering, iterative deepening with a fixed
  node budget (default 30,000 nodes/move, `CHESS_NODES`).
- Eval: material + piece-square tables + tapered king + passed /
  isolated / doubled pawns.
- `main.py` is the LZMA-compressed entry (see `src.py`, the readable
  source). Only the Python standard library is used.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:18080 CHESS_NODES=30000 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=0m7x29es&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
