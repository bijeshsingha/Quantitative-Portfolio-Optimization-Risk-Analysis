# Quantitative Portfolio Optimization and Risk Analysis Model

## Overview
This project implements a multi-asset portfolio optimization and risk assessment model to maximize risk-adjusted returns and quantify tail risk.

The model uses statistical methods, Minimum Variance optimization, and out-of-sample validation to ensure realistic and unbiased performance.

---

## Key Features
- Multi-asset portfolio including equities, ETFs, and currencies
- Covariance-based risk modeling
- Monte Carlo simulation for return distribution
- Value at Risk (VaR) estimation
- Train-test split for backtesting
- Benchmark comparison with equal-weight portfolio

---

## Methodology

### 1. Data Architecture and Backtesting
- Collected daily closing prices for 20 assets
- Assets include Indian equities, ETFs, and currencies

Time split:
- Training set: Oct 2022 to Nov 2024
- Test set: Dec 2024 to Dec 2025

This prevents data leakage and ensures realistic evaluation.

---

### 2. Statistical Modeling
- Calculated daily returns, expected returns, and excess returns
- Built a 20 x 20 covariance matrix to measure correlations and volatility

---

### 3. Portfolio Optimization
- Implemented Mean-Variance Optimization

Constructed:
- Minimum Variance Portfolio (lowest risk)
- Multiple portfolios for different risk levels
- Equal Weight Portfolio (1/n) as baseline

---

### 4. Monte Carlo Simulation
- Simulated thousands of return paths
- Based on historical mean and standard deviation
- Generated probabilistic performance outcomes

---

### 5. Value at Risk (VaR) - 99 percent confidence
- Historical VaR: based on worst 1 percent returns
- Parametric VaR: using normal distribution
- Monte Carlo VaR: from simulated outcomes

---

### 6. Out-of-Sample Validation
- Applied optimized weights to unseen test data
- Recomputed returns and risk metrics

This ensures the model is not overfitted.

---

## Final Output
- Expected returns
- Portfolio volatility
- Risk-adjusted performance
- Monte Carlo projections
- VaR estimates

Compared against equal-weight portfolio to measure performance improvement.

---

## Skills Used
- Modern Portfolio Theory (MPT)
- Portfolio Optimization
- Monte Carlo Simulation
- Value at Risk (VaR)
- Covariance Modeling
- Statistical Backtesting

---

## Use Cases
- Portfolio construction
- Risk management
- Quantitative finance projects
- Investment strategy testing
