# tiny-chess-01 entry

A compact Python chess engine (alpha-beta + quiescence, transposition table,
null-move pruning, LMR, piece-square tables). Reads positions from the
make.fun env at `MAKEFUN_ENV_URL` and plays the 16-game gauntlet.

`main.py` is a self-contained stub: it decompresses and runs the engine
(standard library only, deterministic, fixed node budget per move).
