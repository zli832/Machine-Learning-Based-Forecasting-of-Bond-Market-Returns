# Machine-Learning-Based-Forecasting-of-Bond-Market-Returns

## **Project Overview**

This project applies machine learning techniques to forecast corporate bond market returns. Unlike equities, bond price movements are harder to predict due to lower liquidity and limited intraday pricing data. This project investigates whether modern ML models can extract useful predictive signals from historical bond-index time series and improve short-term return forecasting.



## **Goals**

* Predict short-term movements in the corporate bond total return index
* Compare model performance (Random Forest, LightGBM, Logistic Regression)
* Identify the most influential predictive features
* Evaluate whether ML outperforms a naive “no-change” benchmark
* Support investment decisions and risk-management analysis



## **How It Works**

### **Models Used**

* Random Forest
* LightGBM (Gradient Boosting)
* Logistic Regression



## **Feature Engineering**

### **Return Transformations**

* Raw daily return
* Continuously compounded rate of change
* Continuously compounded annual rate of change
* Percent change (`pct_change`)
* Natural log return (`log_return`)
* Change from year ago
* Percent change from year ago
* Compounded annual rate of change

### **Lagged Returns**

* 1-day lag
* 2-day lag
* 3-day lag
* 5-day lag
* 10-day lag

### **Moving Averages & Trend Indicators**

* 1-day moving average
* 3-day moving average
* Moving-average difference

### **Volatility Measures**

* 3-day rolling volatility
* 5-day rolling volatility
* Exponentially weighted volatility (α-weighted, 4-period)

### **Technical Indicators**

* RSI (Relative Strength Index)



## **Dataset**

**Source:** BofA Merrill Lynch Corporate Bond Total Return Index
**Frequency:** Daily
**Time Period:** *(Add date range, e.g., 2010–2024)*
**Size:** *(Add final number of observations, e.g., ~3,500 rows after cleaning)*

Dataset includes raw index values plus all engineered features used for ML forecasting.



## **Model Evaluation**

Models are evaluated using:

* Accuracy
* Precision
* Recall
* AUC (ROC)
* Confusion Matrix
* Feature Importance (Tree-based models)

Additionally, the project compares:

* Naive baseline (predict “no change”)
* Logistic Regression benchmark
* Tree-based ML models (Random Forest / LightGBM)

