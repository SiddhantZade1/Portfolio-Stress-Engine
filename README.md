Portfolio Stress Testing

Overview

This project builds a portfolio stress testing framework using Python and historical market data. The goal is to evaluate how different portfolio strategies perform during market crises, under simulated shock scenarios, and through a basic machine learning approach to stress detection.

The focus of this project is not only on return, but on understanding portfolio resilience, drawdowns, and behavior during difficult market conditions.

Objective

The objective of this project is to compare how different portfolio constructions respond to stress environments. It also explores whether simple machine learning features can help identify periods of market stress in advance.

Portfolios Included

The project compares multiple portfolio styles representing different investment approaches:

Conservative
Balanced
Aggressive
Inflation Hedge
Recession Defense
All Weather
Concentrated Equity
Custom 100K Portfolio

Assets Used

The portfolio framework uses exchange traded funds representing different asset classes:

SPY for broad US equities
QQQ for growth oriented equities
TLT for long duration US Treasury bonds
IEF for intermediate duration US Treasury bonds
GLD for gold
USO for oil exposure
HYG for high yield credit
DBC for commodities
SHY for short term Treasury exposure

What the Project Does

Downloads historical adjusted price data starting from 2007

Constructs multiple portfolios using different asset allocations

Calculates daily returns and cumulative growth of portfolios

Evaluates key performance metrics including annualized return, annualized volatility, Sharpe ratio, and maximum drawdown

Analyzes portfolio performance during major crisis periods

Simulates hypothetical stress scenarios such as equity crashes and inflation shocks

Builds a machine learning based stress detection model using return and rolling volatility

Historical Stress Periods

Global Financial Crisis from October 2007 to March 2009

COVID Crash from February 2020 to April 2020

Machine Learning Approach

The project uses a simple classification model to detect stress regimes. Stress is defined based on the worst 10 percent of forward 20 day returns, allowing for a data driven identification of extreme downside periods.

The model uses features such as daily returns and rolling volatility to classify whether the market is entering a stress regime.

Key Insights

Portfolio performance varies significantly across market regimes

Diversification improves stability but does not eliminate drawdowns during crises

Portfolios designed for inflation or recession behave differently under stress

Scenario testing provides additional insight beyond historical analysis

Machine learning can be used as an initial step toward identifying forward looking stress signals

Tools and Libraries

Python
Pandas
NumPy
Matplotlib
yfinance
scikit learn

File in Repository

ml_portfolio_stress_testing.ipynb

How to Use

Open the notebook in Jupyter Notebook or Google Colab

Run all cells in order

Review portfolio performance, risk metrics, crisis analysis, scenario testing, and machine learning outputs

Project Positioning

This project demonstrates practical skills in portfolio construction, risk analysis, stress testing, and the application of machine learning in financial analysis. It is designed to reflect how portfolios behave under real world conditions rather than only in average market environments.
