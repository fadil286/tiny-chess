# Tiny Chess

[![Bounty](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![Rank](https://make.fun/badge/tiny-chess-01/fadil286/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![Reward](https://make.fun/badge/tiny-chess-01/fadil286/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in under 4,096 bytes of Python. Original work, MIT licensed.

## Engine

`main.py` is a self-contained chess engine (4,022 bytes): 0x88 board, negamax
with alpha-beta, quiescence search (captures, with check handling), tapered
PeSTO-style piece-square evaluation, and a fixed node budget for deterministic
play. It speaks the make.fun environment protocol (`MAKEFUN_ENV_URL`) and plays
a full game through `/game`, `/move`, `/resign`.

Local practice trial-0 (6 games vs the house gauntlet): 0.5/6, practice Elo 708.

## Files

- `main.py` — the engine (≤4,096 bytes, Python 3.13 stdlib only)
- `LICENSE` — MIT
- `.makefun/owner.json` — payout wallet
