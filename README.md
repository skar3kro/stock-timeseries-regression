# BHEL Intraday Time Series Regression Models

This repository contains machine learning models built to predict the **next-candle close price** for **BHEL** using minute-level data sourced from the Kaggle dataset:

**`algo-trading-data-nifty-100-data-with-indicators`**

The project focuses on transforming minute-level OHLCV data into **15-minute and 30-minute candles**, followed by building regression models with feature engineering and lag-based predictors.

---

## 📌 Project Highlights

- Resampled minute data into **15m** and **30m** intervals  
- Built **Linear Regression**, **Ridge**, **Lasso**, and **ElasticNet** models  
- Added engineered features such as:
  - Spread (High − Low)  
  - Body (Close − Open)  
  - Percentage returns  
  - Rolling mean & volatility  
  - Lag features (1, 2, 3, 5, 10 periods)  
- Applied **time-based train–test split** (no shuffling)
- Achieved **very high R² scores** with low prediction error
- All work developed and tested using **Kaggle Notebooks**

---

## 📁 Files Included

- `bhel_15min_30min_regression.ipynb`:  
  Full notebook with data prep, feature engineering, and regression models.

---

## 🚀 Next Steps (Future Work)

- Build and tune **Random Forest** and **XGBoost** models  
- Compare different stocks using the same modeling pipeline  
- Add ARIMA/LSTM models for hybrid forecasting  
- Create reusable Python modules (`src/` folder) for model automation  

---

## 🛠 Environment

- Python  
- Pandas, NumPy  
- scikit-learn  
- Matplotlib  
- Kaggle Notebook runtime  

---

## 📊 Dataset Reference

Kaggle Dataset:  
**algo-trading-data-nifty-100-data-with-indicators**  
(Contains minute-level data for multiple NSE stocks.)

---

Feel free to clone, modify, and build upon this project.
