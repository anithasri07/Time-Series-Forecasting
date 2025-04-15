# 🥛 Milk Production Forecasting using Time Series Models

This project focuses on analyzing and forecasting monthly milk production using classical time series analysis. We utilize models like SARIMA and Holt-Winters to predict future values. The dataset represents monthly milk production per cow in pounds.

---

## 📊 Dataset Overview

The dataset contains:

- Monthly observations
- Variable: **Milk Production (pounds per cow)**

---

## 🎯 Objective

- Understand trends and seasonality
- Make the time series stationary
- Forecast future values using:
  - SARIMA Model
  - Holt-Winters Exponential Smoothing

---

## 📁 Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib & Seaborn** (for visualization)
- **Statsmodels** (SARIMA, Decomposition, Holt-Winters)

---

## 📌 Key Steps

### 1. 📉 Visualizing Rolling Statistics

```python
df['rollmean'] = df['Milk_Production'].rolling(window=12).mean()
df['rollstd'] = df['Milk_Production'].rolling(window=12).std()
