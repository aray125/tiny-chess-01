# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/aray125/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/aray125/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python: 0x88 board, negamax
alpha-beta with a transposition table, quiescence search, null-move
pruning, MVV-LVA / killer / history move ordering, and a tapered
piece-square evaluation. It searches to a fixed node budget per move
(deterministic, no clock), playing the house gauntlet through the
make.fun env.

`main.py` is an LZMA-packed entrypoint made with `makefun compress`
from the readable source `src.py` (kept beside it, uncommitted);
the packed bytes are what count toward the 4,096-byte cap.

The piece-square tables use the same formulas as the house gauntlet
engines published in the competition kit (MIT licensed).

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
