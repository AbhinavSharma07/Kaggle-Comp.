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

Final rankings are based on the private leaderboard.

---

## 📊 Evaluation Metric

The competition uses a **Weighted RMSE-based Skill Score**, defined as:

\[
score = \sqrt{1 - clip\left(\frac{\sum w (y - \hat{y})^2}{\sum w y^2}, 0, 1\right)}
\]

Where:
- `y` = true values  
- `ŷ` = predictions  
- `w` = weights  

Reference implementation:

```python
def _clip01(x: float) -> float:
    return float(np.minimum(np.maximum(x, 0.0), 1.0))

def weighted_rmse_score(y_target, y_pred, w) -> float:
    denom = np.sum(w * y_target ** 2)
    ratio = np.sum(w * (y_target - y_pred) ** 2) / denom
    clipped = _clip01(ratio)
    val = 1.0 - clipped
    return float(np.sqrt(val))
