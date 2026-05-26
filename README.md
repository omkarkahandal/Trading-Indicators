# Trading Indicators

This repository contains custom indicators for the TradingView website, written in Pine Script version 6 (and v5). These scripts are designed to detect structural market changes, order blocks, volume footprints, and utilize astrological cycle confluences to deliver high-probability trading signals.

## Description
It's built for the TradingView website and includes various versions and combined strategies. Below is a breakdown of the different versions and what they accomplish.

## Included Files and Their Use

### `Combined_Strategy.pine`
**Combined OB + Astro Strategy**
A powerful confluence strategy merging Order Block (OB) detection and Astro indicators. 
- **What it accomplishes**: It dynamically detects bullish and bearish order blocks in real-time, verifying them against volume and imbalance (FVG) filters. Simultaneously, it calculates an "Astro Score" based on planetary cycles and moon phases. Signals are strictly filtered so that a Buy or Sell is only plotted when there's a strong alignment of market structure, volume, and timing.

### `Volume_OB_Detector.pine`
**Volume-Based OB Detector**
An indicator dedicated exclusively to finding high-volume Order Blocks.
- **What it accomplishes**: It helps traders identify strong reversal zones by spotting candles that led to a Break of Structure (BOS) with above-average volume. It visually draws these zones on the chart and cleans them up once the price mitigates (closes beyond) them.

### `version4.pine`
**Live Candle-Based OB Detector [v4]**
- **What it accomplishes**: Real-time order block detection based on immediate breaks of structure on a candle-by-candle basis. It provides live visual boxes for Bullish and Bearish order blocks. Traders can optionally enable volume and Fair Value Gap (FVG) filters to increase the accuracy of the detected zones.

### `version1.txt` & `version3.txt`
**Omkar's Clear BUY SELL Strategy [SMC + Astro] FIXED**
- **What it accomplishes**: A complete strategy combining Smart Money Concepts (SMC) and Astro cycles. It looks for strong momentum candles (CRT) aligning with calculated astrological scores to produce clear, actionable BUY and SELL labels on the chart. It also plots Swing Highs and Swing Lows for stop-loss placement and calculates automated Take Profit targets based on a predefined Risk-to-Reward ratio.

### `version2.txt`
An empty placeholder file for future experimental versions.

## How to Use
1. Open [TradingView](https://www.tradingview.com/).
2. Open the Pine Editor at the bottom of the chart.
3. Copy the code from the desired file in this repository and paste it into the editor.
4. Click "Add to Chart" or "Save".
5. Customize the settings (such as colors, filters, and lookback periods) via the indicator settings menu.