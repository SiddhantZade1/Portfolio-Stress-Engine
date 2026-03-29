# Portfolio Stress Testing

## Overview

This project builds a portfolio stress testing framework using Python, historical market data, and a basic machine learning stress detection layer.

Instead of focusing only on return, the project evaluates how different portfolio strategies behave during crisis periods, inflation shocks, recessionary environments, and equity drawdowns.

## What this project highlights

This project highlights four key ideas:

- Multi-portfolio construction across different market views
- Historical crisis testing using the Global Financial Crisis and COVID crash
- Scenario analysis under shock environments
- Machine learning based stress regime detection using return and rolling volatility

## Portfolios included

The notebook compares the following portfolio styles:

- Conservative
- Balanced
- Aggressive
- Inflation Hedge
- Recession Defense
- All Weather
- Concentrated Equity
- Custom 100K Portfolio

## Assets used

The framework uses ETFs representing major asset classes:

- SPY for broad US equities
- QQQ for growth equities
- TLT for long duration US Treasury bonds
- IEF for intermediate duration US Treasury bonds
- GLD for gold
- USO for oil exposure
- HYG for high yield credit
- DBC for commodities
- SHY for short term Treasury exposure

## Project workflow

The notebook follows this process:

1. Download historical market data from 2007 onward
2. Build portfolio returns for multiple allocation styles
3. Compare cumulative portfolio growth
4. Calculate risk and performance metrics
5. Test behavior during historical crisis periods
6. Run shock based scenario analysis
7. Apply a machine learning classification model to identify stress regimes

## Key metrics evaluated

The project evaluates each portfolio using:

- Annualized return
- Annualized volatility
- Sharpe ratio
- Maximum drawdown

## Historical stress periods used

- Global Financial Crisis from October 2007 to March 2009
- COVID Crash from February 2020 to April 2020

## Machine learning approach

The machine learning section uses a classification framework to identify stress regimes.

Stress is defined using the worst 10 percent of forward 20 day returns, which makes the target data driven rather than based on an arbitrary threshold.

The model uses:

- Daily returns
- Rolling volatility

This section is intended as a prototype that shows how machine learning can be layered onto a portfolio risk framework.

## Sample output

### Portfolio growth comparison

Add a screenshot here of your cumulative portfolio growth chart.

![Portfolio Growth](images/portfolio_growth.png)

### Risk metric comparison

Add a screenshot here of your summary ranking table or metric comparison output.

![Risk Metrics](images/risk_metrics.png)

### Crisis period analysis

Add a screenshot here of your crisis performance table or chart.

![Crisis Analysis](images/crisis_analysis.png)

### Machine learning stress detection

Add a screenshot here of the ML output, class distribution, threshold logic, or stress classification results.

![ML Stress Detection](images/ml_stress_detection.png)

## Key takeaways

- Portfolio behavior changes significantly across market regimes
- Diversification improves stability, but crisis drawdowns still differ sharply by allocation
- Defensive and inflation focused portfolios respond differently under stress
- Historical stress testing reveals weaknesses that average return analysis can miss
- Machine learning can be used as an early step toward identifying downside risk conditions

## Tools and libraries

- Python
- pandas
- numpy
- matplotlib
- yfinance
- scikit-learn

## Repository file

- ml_portfolio_stress_testing.ipynb

## How to use

1. Open the notebook in Jupyter Notebook or Google Colab
2. Run all cells in order
3. Review the portfolio comparison, crisis analysis, scenario testing, and ML stress detection outputs

## Project positioning

This project demonstrates practical skills in:

- Portfolio construction
- Risk analysis
- Stress testing
- Scenario modeling
- Applied machine learning in finance
