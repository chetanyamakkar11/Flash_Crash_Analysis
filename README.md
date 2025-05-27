# Flash Crash Analysis — May 6, 2010

## Overview

This project analyzes the **Flash Crash** that occurred on **May 6, 2010**, during which U.S. stock markets experienced a rapid and extreme drop in prices, followed by a swift recovery — all within less than one hour.

We use transaction-level data from two major financial instruments:
- **S&P 500 E-mini Futures (ESM10)**
- **SPDR S&P 500 ETF (SPY)**

The objective is to understand market behavior, liquidity shifts, and data anomalies during this unique market event.

---

## Dataset Description

The dataset includes four files (not publicly provided):
1. `ESM10_trades.csv` — Trade data for S&P 500 E-mini Futures
2. `ESM10_quotes.csv` — Quote data for S&P 500 E-mini Futures
3. `SPY_trades.csv` — Trade data for SPDR S&P 500 ETF
4. `SPY_quotes.csv` — Quote data for SPDR S&P 500 ETF

Each file contains nanosecond-level timestamps, price, and volume information.

---

## Project Objectives

- **Data Cleaning**
  - Fix missing or zero entries
  - Convert timestamps to New York time
  - Normalize column types
- **Statistical Analysis**
  - Compute basic stats (mean, median, std)
  - Analyze bid-ask spreads, volumes, and price volatility
- **Market Insight**
  - Visualize trade and quote activity
  - Detect irregular pricing and illiquidity
  - Compare SPY and ESM10 patterns during crash

---

## Key Insights

- Timestamps offer **nanosecond** granularity, allowing for high-frequency analysis
- Abnormal prices (e.g., 0.01 or 9999.99) are **not errors**, but signs of **liquidity collapse**
- Flash crashes highlight the fragility of algorithm-driven markets under stress

---

## Technologies Used

- Python 3
- Jupyter Notebook / Google Colab
- `pandas`, `numpy`, `matplotlib`

---

## Acknowledgment

This analysis was conducted under the guidance of **Dr. Albert S. (Pete) Kyle** as part of **BUFN400 (Spring 2024)** at the **University of Maryland**.

