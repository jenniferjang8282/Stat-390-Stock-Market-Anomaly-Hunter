# Stat-390-Stock-Market-Anomaly-Hunter
The objective of this project is to build a closed-loop AutoResearch system, inspired by Karpathy’s framework, that autonomously generates, tests, and refines structured hypotheses about short-term stock return anomalies.

## Research Question
Do recurring, exploitable anomalies exist in U.S. equities — discoverable from price, news sentiment, and fundamentals — that an AI agent can autonomously identify, backtest, and validate out-of-sample?



# AutoResearch for Market Anomaly Discovery

## Overview
This project builds a reproducible baseline for a Karpathy-style AutoResearch system that evaluates stock market anomaly signals using historical data.

## Baseline Strategy
If a stock drops more than 3% in one day, buy it the next day and hold for one day.

## Data
- Source: yfinance
- Stocks: AAPL, MSFT, AMZN, GOOGL, META
- Train set: 2022-2023
- Test set: 2024

## Primary Metric
Annualized Sharpe Ratio

## Files
- `week2_baseline.ipynb`: main notebook
- `baseline_results.csv`: summary results
- `experiments.csv`: first experiment log entry

## How to Run
1. Open `week2_baseline.ipynb`
2. Run all cells from top to bottom
3. The notebook will:
   - download stock data
   - create the baseline signal
   - run train/test backtests
   - print evaluation metrics
   - save results files

## Reproducibility
The project uses a deterministic date-based split and a fixed evaluation metric so the baseline can be reproduced consistently.
