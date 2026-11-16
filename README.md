# tiny-chess-01

A compact Python chess engine for the make.fun tiny-chess-01 bounty.

- 0x88 board, alpha-beta + quiescence, transposition table, MVV-LVA
  captures + killer move ordering, iterative deepening with a fixed
  node budget (default 30,000 nodes/move, `CHESS_NODES`).
- Eval: material + piece-square tables + tapered king + passed /
  isolated / doubled pawns.
- `main.py` is the LZMA-compressed entry (see `src.py`, the readable
  source). Only the Python standard library is used.

## Run

```
MAKEFUN_ENV_URL=http://127.0.0.1:18080 CHESS_NODES=30000 python3 main.py
```

License: MIT.
