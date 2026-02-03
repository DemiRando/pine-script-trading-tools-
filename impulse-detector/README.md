# Impulse Detector

This indicator is designed primarily as a component but it can also be used on its own. It highlights impulsive price movement using volatility expansion, micro-structure alignment, and a candle overlap filter to avoid range-bound or choppy conditions.

The output is visual only. In this implementation impulses are reflected through the SMA color, but the same logic can be applied to other visual outputs if needed.

## Core Ideas
- Range-normalized impulse distance to adapt across regimes
- Overlap filtering to suppress compression and liquidity noise
- Simple structure confirmation to isolate displacement

## Use Case
Best suited for trending instruments during active sessions. Use impulse signals as confluence with directional bias. Less effective in tight ranges or low-volume periods where overlap filtering may suppress valid moves.

Can be integrated into entry logic, used as a filter for existing signals, or incorporated into multi-timeframe analysis.

### SMC/ICT Integration
- Filtering FVGs, order blocks, or liquidity zones to impulse-only contexts
- Identifying displacement candles before pullbacks
- Suppressing signals during compression or chop
- Acting as a regime filter for automated strategies

---

*Written in Pine Script v6*
