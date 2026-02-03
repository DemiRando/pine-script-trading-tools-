# Supply/Demand Zone Builder

Identifies potential supply and demand zones based on reversal candle sequences with momentum confirmation. Zones are drawn from the base reversal candle and extended until invalidated by price.

## Core Logic
- Detects bear-to-bull or bull-to-bear candle reversals as zone candidates
- Confirms zones when continuation candles meet minimum count and optional ATR threshold
- Limits active zones per side, automatically pausing oldest when limit reached
- Invalidates zones when price wicks through (not just closes)

## Use Case
Useful for traders who mark institutional supply/demand levels. Works best on higher timeframes (H1+) where reversal patterns are more reliable. Zones can be used as confluence with other entry methods or as standalone areas of interest.

**Zone Management:**
- Set max active zones to reduce visual clutter
- Body-based zones provide tighter, more accurate levels
- Live extension keeps zones current but may repaint

## Configuration
- **ATR Multiplier**: Higher values require stronger momentum for confirmation
- **Min Continuation Candles**: More candles = more conservative zone creation
- **Body-Based Zones**: Uses candle bodies instead of wicks for tighter zones
- **Max Active Zones**: Limits how many zones per side stay active

---

*Pine Script v6. Refactored zone detection logic with managed invalidation and extension.*
