# Trading Indicators

Custom TradingView indicators written in Pine Script (v5 and v6) for identifying order blocks and structure-based trade zones.

## Overview

This repository contains two order-block indicators:

1. **Volume-based detection** for highlighting stronger zones backed by volume.
2. **Live candle-based detection** for fast, real-time structure breaks.

Both scripts draw bullish and bearish order-block zones directly on chart and automatically remove zones when they are mitigated.

## Included Files

### `Volume_OB_Detector.pine` (Pine Script v6)
**Volume-Based OB Detector**

- Detects bullish and bearish order blocks from break-of-structure events.
- Supports optional filters:
  - Volume confirmation
  - Imbalance / Fair Value Gap (FVG) confirmation
- Labels zones with compact OB volume text.
- Deletes zones after mitigation to keep charts clean.

### `Old indicator.pine` (Pine Script v5)
**Live Candle-Based OB Detector**

- Detects order blocks in real time using immediate candle-by-candle structure breaks.
- Supports optional filters:
  - Volume confirmation
  - Imbalance / Fair Value Gap (FVG) confirmation
- Draws and manages bullish/bearish OB boxes with mitigation logic.

## How to Use

1. Open [TradingView](https://www.tradingview.com/).
2. Open the **Pine Editor**.
3. Copy the script from the file you want to use.
4. Paste it into the editor and click **Add to chart**.
5. Open indicator settings to customize:
   - Bullish/Bearish visibility
   - Body vs wick zone range
   - Filter behavior
   - Colors and text settings

## Notes

- These indicators are visual and discretionary tools, not financial advice.
- Test on paper/demo charts before using in live markets.
