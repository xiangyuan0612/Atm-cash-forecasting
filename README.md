# ATM Cash Demand Forecasting

## 📌 Project Overview
This project analyzes ATM cash demand time series data and builds forecasting models using SARIMA and ETS methods.

The goal is to understand demand patterns and support cash logistics planning.

---

## 📊 Key Insights
- Strong weekly seasonality (lag = 7)
- Structural level shifts in demand
- Seasonal patterns vary across datasets
- Missing values (~2–3%) handled using seasonal imputation

---

## 🔬 Methodology
- Exploratory Data Analysis (EDA)
- Stationarity tests (ADF & KPSS)
- ACF / PACF analysis
- Seasonal decomposition
- SARIMA & ETS modeling
- Model evaluation (RMSE, MAE, MAPE)

---

## 📈 Results
- SARIMA captures seasonality effectively
- ETS performs competitively across datasets
- Forecast aligns with real demand patterns

---

## 📉 Visualizations

<img width="844" height="233" alt="image" src="https://github.com/user-attachments/assets/6c38bce3-67c2-46e1-87d5-74f8a2c82d83" />


- Time series trend
- Decomposition results
- ACF / PACF plots
- Forecast vs actual

---

## 💡 Business Insight
- ATM cash demand is highly seasonal
- Weekly patterns can guide cash replenishment cycles
- Year-end spikes require operational planning
