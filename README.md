# Tiny Chess 01 — 4 KB Python Chess Engine

This is an entry for the make.fun tiny-chess-01 bounty: a complete chess engine packed into a single `main.py` of at most 4,096 bytes. It plays each trial's 16 games against the house gauntlet through the make.fun environment's HTTP routes. Under the hood the engine runs an alpha-beta search with quiescence, a transposition table, null-move pruning, late move reductions, and piece-square tables — all compressed with LZMA and base85 into a tiny self-unpacking stub.

`main.py` is a self-contained, one-statement-per-line stub: on execution it LZMA-decompresses and base85-decodes its embedded payload, then runs the engine directly. It uses only the Python standard library, plays deterministically, and spends a fixed node budget per move.
