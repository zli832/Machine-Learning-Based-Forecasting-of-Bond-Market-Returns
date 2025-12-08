# Machine-Learning-Based-Forecasting-of-Bond-Market-Returns

Project Overview
This project applies machine learning techniques to forecast bond market returns. Unlike stocks, bonds are harder to predict because they don't trade as openly and price information is less available. This project explores whether modern machine learning models can extract useful signals from historical bond-index data and improve short-term return forecasts.

Goals

- Predict how the corporate bond index will perform
- Compare model performance (Random Forest, LightGBM, Logistic Regression)
- Identify the most important predictive features
- Evaluate whether ML improves forecast accuracy vs. naive benchmark
- Support better investment and risk-management decisions

How It Works
We test several different machine learning methods:

-Random Forest
-LightGBM(Gradient Boosting)
-Logistic Regression

Feature Engineering:

Return Transformations

-raw daily return
-continuously compounded annual rate of change
-continuously compounded rate of change
-percent change (pct_change)
-natural log return (log_return)
-change from year ago
-percent change from year ago
-compounded annual rate of change

Lagged Returns

1-day lag
2-day lag
3-day lag
5-day lag
10-day lag


Moving Averages and Trend Indicators

1-day moving average
3-day moving average
moving-average difference


Volatility Measures
3-day rolling volatility
5-day rolling volatility
exponentially weighted volatility (4-period)

Technical Indicators
RSI (Relative Strength Index)

Dataset

Source: BofA Merrill Lynch Corporate Bond Total Return Index

Frequency: Daily

Time Period: (Add your full date range here—e.g., 2010–2024)

Size: (Add number of observations, e.g., ~3,500 rows after cleaning)

The dataset includes both raw bond index values and engineered features created for machine-learning modeling.


Model Evaluation
The models are evaluated using:
Accuracy
Precision
Recall
AUC (ROC)
Confusion Matrix
Feature Importance (LightGBM / Random Forest)


This project additionally compares model performance across:
Naive baseline (predict “no change”)
Logistic Regression benchmark
Tree-based ML models
