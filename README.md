# Algorithmic Trading & ML — Weekly Movement Prediction (NVDA)

## Executive summary
This project builds and evaluates machine learning models to predict weekly market movements on NVDA.
The focus is on time-series correctness (temporal splits), model comparison, threshold optimization, and rolling backtesting.

## Data and target
- Market data transformed into weekly observations
- Target: direction / movement prediction (classification) and/or value prediction (regression)
- Emphasis: no look-ahead bias, time-aware validation

## Method
1) Data prep + exploratory analysis
2) Feature engineering (returns, rolling indicators, volatility proxies, etc.)
3) TimeSeriesSplit validation
4) Models compared
   - Linear regression (baseline)
   - Logistic regression (baseline classifier)
   - XGBoost regression
   - XGBoost classification
5) Threshold optimization (probability-to-decision)
6) Rolling backtest (2023–2024)

## Key results 
- Cross-validation metrics table (Accuracy / Precision / Recall / F1 for classifiers; MAE/MSE for regressors)
- Rolling backtest summary (2023–2024)
- Clear comparison vs a baseline strategy

## Limitations and next steps
- Add transaction costs, slippage, and realistic execution constraints
- Add risk metrics: max drawdown, Sharpe, volatility of returns
- Perform robustness checks across different time windows and assets


