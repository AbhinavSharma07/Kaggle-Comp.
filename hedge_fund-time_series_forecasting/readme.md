# 📈 Sequential Time Series Forecasting – Out-of-Sample Robust Prediction

This repository contains my solution for a community time-series forecasting competition, where the objective is to predict continuous numerical values for multiple hierarchical combinations:

- `code`
- `sub-code`
- `sub-category`
- `forecast_horizon`
- `ts_index` (time index)

The challenge emphasizes **strict sequential prediction**, **no look-ahead bias**, and **robust out-of-sample generalization**.

---

## 🚀 Competition Overview

Participants receive an integer-indexed time series dataset.  
Each record is uniquely identified by:

- Code
- Sub-code
- Sub-category
- Forecast horizon
- Time index (`ts_index`)

The task is to train a model that:

- Predicts a continuous target variable
- Processes data strictly sequentially
- Uses only information available up to time `t` when predicting at time `t`
- Avoids all forms of data leakage

Public leaderboard: ~25% of test data  
Private leaderboard: ~75% of hidden test data  


