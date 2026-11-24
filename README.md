# Backtest Overfitting Detector

A quantitative Python framework for detecting statistical overfitting and false discoveries in algorithmic trading backtests.

## Overview
Backtesting hundreds of trading strategies on historical data inevitably produces "profitable" strategies purely by chance—a phenomenon known as selection bias under multiple testing. This tool quantifies the probability that a seemingly profitable backtest is statistical noise rather than genuine alpha.

## Tech Stack
- **Language:** Python 3
- **Libraries:** `pandas`, `numpy`, `scipy`, `matplotlib`
- **Core Concepts:** In-sample vs. out-of-sample validation, Monte Carlo simulation, Deflated Sharpe Ratio, Combinatorially Symmetric Cross-Validation (CSCV)

## Methodology
1. **Strategy Generation:** Simulates a large family of parameterized trading strategies over historical price data.
2. **Validation Split:** Selects top-performing strategies in-sample and evaluates performance degradation out-of-sample.
3. **Statistical Diagnostics:** Visualizes performance collapse and computes overfitting probability metrics.

