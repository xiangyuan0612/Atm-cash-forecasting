<img width="757" height="258" alt="image" src="https://github.com/user-attachments/assets/88a2408a-bfbc-4ce0-986b-ac789880609d" /><img width="804" height="176" alt="image" src="https://github.com/user-attachments/assets/e4d4f221-85b6-4fe5-b948-3cb2b4198dc3" /># ATM Cash Demand Forecasting

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

1. Exploratory Data Analysis

<img width="844" height="233" alt="image" src="https://github.com/user-attachments/assets/6c38bce3-67c2-46e1-87d5-74f8a2c82d83" />

2.Linear interpolation for missing values

<img width="861" height="373" alt="image" src="https://github.com/user-attachments/assets/b8c9e670-3add-4385-9559-b68c747d8178" />
3.Seasonality analysis

<img width="767" height="319" alt="image" src="https://github.com/user-attachments/assets/53e0462a-ef4e-41fc-995d-73f4bdca4e6c" />
4. Statistical tests
<img width="804" height="176" alt="image" src="https://github.com/user-attachments/assets/0dfa0dcf-5965-4da1-a8c5-1d2c09deae6b" />
5. Differenced data
<img width="886" height="549" alt="image" src="https://github.com/user-attachments/assets/b561778a-f19a-4126-aa93-297119f0d5a6" />
6.ACF Analysis
<img width="869" height="291" alt="image" src="https://github.com/user-attachments/assets/e08ab70a-9078-493c-957e-f5f5acc8405d" />
<img width="819" height="390" alt="image" src="https://github.com/user-attachments/assets/eb1c335f-baf8-4372-b18c-c708cc9dcf15" />
7. Time Series Decomposition
<img width="801" height="462" alt="image" src="https://github.com/user-attachments/assets/bc813e96-dd6c-4e1f-8523-db514a06bf86" />
<img width="800" height="306" alt="image" src="https://github.com/user-attachments/assets/fffb94b8-b157-4afc-8330-e884c9de605a" />

8. Forecasting Model
<img width="834" height="326" alt="image" src="https://github.com/user-attachments/assets/43f94060-fe98-4cdf-9b7f-172e927be77f" />
<img width="575" height="182" alt="image" src="https://github.com/user-attachments/assets/2679504b-4057-4a0e-bd34-061207f2beed" />

<img width="757" height="258" alt="image" src="https://github.com/user-attachments/assets/186f0f42-96ac-43b8-9f1f-eb2a2123f904" />

Overall
There is a slight increasing trend in the dataset, a significant level shift and a multiplicative
seasonality since when cash demand volume grows, the seasonal effect gets bigger. The average cash
money demand in 1997 and 1998 almost doubled compared with the average cash money demand of
1996. KPSS and ADF tests are also used to test whether the original and differenced data are
stationary or not, which is helpful for manual order selection in SARIMA models. Finally, SARIMA
(0,0,1)(0,1,1) and SARIMA(3,0,1)(4,1,1) models could be used to predict future values as these two
models has the lowest AIC, and RMSE, MAPE, and MAE, respectively.



---

## 💡 Business Insight
- ATM cash demand is highly seasonal
- Weekly patterns can guide cash replenishment cycles
- Year-end spikes require operational planning
