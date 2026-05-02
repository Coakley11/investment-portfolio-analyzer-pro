# investment-portfolio-analyzer-pro
Streamlit app for portfolio analysis using real market data, Monte Carlo simulation and optimization. 
# Investment Portfolio Analyzer Pro

## Description

Investment Portfolio Analyzer Pro is a Streamlit web app that analyzes investment portfolios using real market ticker data. The app allows users to enter a custom portfolio of stocks, ETFs, bonds, REITs, dividend funds, and short-term Treasury-style investments, then evaluate the portfolio using financial metrics such as annualized return, volatility, Sharpe ratio, correlation, Monte Carlo simulation, and efficient frontier analysis.

The goal of the project is to compare risk, return, diversification, and long-term growth potential across different asset allocations.

---

## Features

- Real ticker input using Yahoo Finance data
- Custom portfolio allocation percentages
- Historical return analysis
- Annualized return calculation
- Annualized volatility calculation
- Sharpe ratio calculation
- Correlation matrix
- Portfolio growth chart
- Scenario analysis:
  - Bear case
  - Base case
  - Bull case
- Monte Carlo simulation
- Portfolio optimizer
- Best Sharpe ratio portfolio
- Minimum volatility portfolio
- Efficient frontier chart
- Support for multiple asset types:
  - S&P 500 ETF
  - Nasdaq/growth ETF
  - bond ETF
  - short-term T-bill ETF
  - REIT ETF
  - dividend ETF

---

## Default Tickers Used

| Ticker | Description |
|---|---|
| SPY | S&P 500 ETF / broad U.S. stock market |
| QQQ | Nasdaq-100 / growth and technology ETF |
| AGG | Aggregate bond ETF / fixed income |
| BIL | Short-term Treasury bill ETF |
| VNQ | Real estate investment trust ETF |
| VIG | Dividend growth ETF |

Users can replace these tickers with their own.

---

## Technologies Used

- Python
- Streamlit
- Pandas
- NumPy
- yFinance

---

## Financial Concepts Used

This project includes several finance and quantitative analysis concepts:

- Asset allocation
- Historical returns
- Volatility
- Risk-adjusted return
- Sharpe ratio
- Correlation matrix
- Diversification
- Monte Carlo simulation
- Efficient frontier
- Portfolio optimization
- Fixed income and short-term investments

---

## How the App Works

1. The user enters a list of tickers and allocation percentages.
2. The app downloads historical market data using `yfinance`.
3. Daily returns are calculated from price data.
4. The app annualizes return and volatility.
5. The portfolio is evaluated based on allocation weights.
6. The app calculates portfolio return, volatility, Sharpe ratio, and projected value.
7. Monte Carlo simulation estimates thousands of possible future outcomes.
8. The optimizer generates many random portfolios and identifies:
   - the highest Sharpe ratio portfolio
   - the minimum volatility portfolio
9. The efficient frontier chart visualizes risk-return tradeoffs across simulated portfolios.

---

## Installation

Install the required libraries:

```bash
pip install streamlit pandas numpy yfinance
