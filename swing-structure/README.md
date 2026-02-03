# Swing Structure Tracker

Identifies swing highs/lows with pivot detection and tracks market structure (HH, HL, LH, LL). Horizontal swing lines project from pivot formation and auto-extend to current price, making it easy to spot when price revisits previous swing levels.

## Core Features
- Configurable pivot detection with left/right bar lookback
- Market structure classification (Higher Highs, Lower Lows, etc.)
- Dynamic swing lines that extend from pivot to current bar
- Optional maximum line length to reduce visual clutter
- Pivot confirmation delay to reduce repainting

## Use Case
Useful for structure-based trading where swing point identification and level tracking matter. Works on any timeframe but most effective on H1+ where swing structure is cleaner.

Lines auto-extend until the next pivot forms or maximum length is reached. Helpful for identifying when price returns to key swing levels.

## Configuration
- **Left/Right Bars**: Controls pivot sensitivity (lower = more pivots, higher = only major swings)
- **Wait for Candle Close**: Enables confirmation delay to reduce repainting
- **Max Line Length**: Limits how long swing lines persist (0 = unlimited)

---

*Pine Script v5. Refactored from legacy community pivot script with modernized structure tracking and dynamic level projection.*
