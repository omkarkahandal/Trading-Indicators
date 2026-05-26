# Trading Indicators

This repository contains custom indicators for the TradingView website, written in Pine Script version 6 (and v5). These scripts are designed to detect structural market changes, order blocks, volume footprints, and utilize astrological cycle confluences to deliver high-probability trading signals.

## Description
It's built for the TradingView website and includes the following indicators:

## Included Files and Their Use

### `Volume_OB_Detector.pine`
**Volume-Based OB Detector**
An indicator dedicated exclusively to finding high-volume Order Blocks.
- **What it accomplishes**: It helps traders identify strong reversal zones by spotting candles that led to a Break of Structure (BOS) with above-average volume. It visually draws these zones on the chart and cleans them up once the price mitigates (closes beyond) them.

### `Old indicator.pine` (formerly version4.pine)
**Live Candle-Based OB Detector**
- **What it accomplishes**: Real-time order block detection based on immediate breaks of structure on a candle-by-candle basis. It provides live visual boxes for Bullish and Bearish order blocks. Traders can optionally enable volume and Fair Value Gap (FVG) filters to increase the accuracy of the detected zones.

## How to Use
1. Open [TradingView](https://www.tradingview.com/).
2. Open the Pine Editor at the bottom of chart.
3. Copy the code from the desired file in this repository and paste it into the editor.
4. Click "Add to Chart" or "Save".
5. Customize the settings (such as colors, filters, and lookback periods) via the indicator settings menu.
