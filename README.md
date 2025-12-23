# Portfolio-Optimization-using-Modern-Portfolio-Theory

**Portfolio Optimization Using Modern Portfolio Theory
Overview

This project implements a portfolio optimization model using Modern Portfolio Theory (MPT) to determine the optimal allocation of capital across a set of publicly traded equities. The goal is to maximize risk-adjusted return while respecting real-world investment constraints.

The model is trained on historical market data from January 1, 2019 to December 31, 2023, and evaluated using out-of-sample data from 2024 to assess generalization and performance.

Objectives

Apply Modern Portfolio Theory to a real-world financial dataset

Optimize portfolio weights using historical return and risk estimates

Evaluate model robustness through backtesting on unseen data

Analyze whether theoretical optimal portfolios translate to real market performance

Dataset

Assets: 9 publicly traded equities

Training Period: January 1, 2019 – December 31, 2023

Evaluation Period: January 1, 2024 – December 31, 2024

Data Source: Historical adjusted closing prices retrieved programmatically

Methodology
1. Data Collection & Preprocessing

Retrieved historical price data for all assets

Calculated daily returns from adjusted close prices

Cleaned and aligned time-series data across all equities

2. Risk & Return Estimation

Computed:

Expected returns

Volatility (standard deviation)

Covariance matrix

Annualized metrics for interpretability

3. Portfolio Optimization

Formulated a constrained optimization problem:

Objective: Maximize Sharpe Ratio

Constraints:

Full investment (weights sum to 1)

No short selling (non-negative weights)

Solved using numerical optimization techniques

4. Backtesting & Evaluation

Applied optimized portfolio weights to 2024 data

Compared:

Predicted vs. realized returns

Expected vs. realized volatility

Evaluated model performance relative to equal-weight baselines

Results

Generated an optimal portfolio allocation that improved risk-adjusted returns compared to naive equal-weight strategies.

Visualized the efficient frontier, portfolio risk-return tradeoffs, and asset weight distributions.

Observed differences between in-sample optimization and out-of-sample performance, highlighting real-world limitations of theoretical models.

Technologies Used

Python

pandas – data manipulation and analysis

NumPy – numerical computations

Matplotlib – data visualization

SciPy – optimization routines

Jupyter Notebook – experimentation and analysis
