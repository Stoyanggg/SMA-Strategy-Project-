# SMA Trading Strategy Analyzer


## Overview

The SMA Trading Strategy Analyzer is a Python tool crafted to facilitate the analysis of Simple Moving Average (SMA) trading strategies, leveraging historical price data obtained from Yahoo Finance. This tool enables users to quickly assess and visualize the performance of SMA-based trading strategies for a variety of financial instruments.

## Features

- **Data Retrieval:** Fetches historical price data from Yahoo Finance for specified financial instruments.
- **SMA Calculation:** Computes and visualizes Simple Moving Averages (SMAs) for user-defined short and long periods.
- **Strategy Testing:** Evaluates the performance of SMA-based trading strategies, generating insights into cumulative returns and strategy outperformance.
- **User-Friendly Interface:** Offers a straightforward interface for users to test and analyze SMA strategies with minimal code.

## Getting Started

### Prerequisites

Ensure you have the following prerequisites installed:

- Python 3.x
- Required libraries:
  ```bash
  pip install pandas numpy yfinance matplotlib
from trading_strategy_analyzer import SMA

# Create SMA object
strategy = SMA(ticker='btc-usd', sma_s=20, sma_l=50, start='2019-01-01', end='today')

# Plot results and analyze performance
strategy.plot_results()

strategy.plot_strategy()

print('Total Returns:', strategy.total_returns())

strategy.plot_total_returns()
