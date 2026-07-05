

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

## 1️⃣ Exploratory Data Analysis

Understanding the overall structure and behavior of ATM cash demand time series.

<img width="844" alt="EDA" src="https://github.com/user-attachments/assets/6c38bce3-67c2-46e1-87d5-74f8a2c82d83" />

---

## 2️⃣ Missing Value Treatment (Linear Interpolation)

Handling missing observations using interpolation to preserve time series continuity.

<img width="861" alt="Missing Data Imputation" src="https://github.com/user-attachments/assets/b8c9e670-3add-4385-9559-b68c747d8178" />

---

## 3️⃣ Seasonality Analysis

Identification of strong weekly patterns and seasonal structure in cash demand.

<img width="767" alt="Seasonality" src="https://github.com/user-attachments/assets/53e0462a-ef4e-41fc-995d-73f4bdca4e6c" />

---

## 4️⃣ Statistical Tests (ADF & KPSS)

Testing stationarity to determine appropriate time series modeling strategy.

<img width="804" alt="Statistical Tests" src="https://github.com/user-attachments/assets/0dfa0dcf-5965-4da1-a8c5-1d2c09deae6b" />

---

## 5️⃣ Differenced Time Series

Transformation applied to achieve stationarity before modeling.

<img width="886" alt="Differenced Data" src="https://github.com/user-attachments/assets/b561778a-f19a-4126-aa93-297119f0d5a6" />

---

## 6️⃣ ACF / PACF Analysis

Autocorrelation diagnostics used for SARIMA model identification.

<img width="869" alt="ACF PACF 1" src="https://github.com/user-attachments/assets/e08ab70a-9078-493c-957e-f5f5acc8405d" />

<img width="819" alt="ACF PACF 2" src="https://github.com/user-attachments/assets/eb1c335f-baf8-4372-b18c-c708cc9dcf15" />

---

## 7️⃣ Time Series Decomposition

Decomposing trend, seasonality, and residual components.

<img width="801" alt="Decomposition 1" src="https://github.com/user-attachments/assets/bc813e96-dd6c-4e1f-8523-db514a06bf86" />

<img width="800" alt="Decomposition 2" src="https://github.com/user-attachments/assets/fffb94b8-b157-4afc-8330-e884c9de605a" />

---

## 8️⃣ Forecasting Results

Model-based prediction of future ATM cash demand using SARIMA models.

<img width="834" alt="Forecast 1" src="https://github.com/user-attachments/assets/43f94060-fe98-4cdf-9b7f-172e927be77f" />

<img width="575" alt="Forecast 2" src="https://github.com/user-attachments/assets/2679504b-4057-4a0e-bd34-061207f2beed" />

<img width="757" alt="Forecast 3" src="https://github.com/user-attachments/assets/186f0f42-96ac-43b8-9f1f-eb2a2123f904" />

---

## 📌 Overall Conclusion

The dataset exhibits:

- A slight increasing trend over time  
- A significant structural level shift  
- Strong multiplicative seasonality (seasonal effect increases with demand level)  

The average cash demand in 1997–1998 is significantly higher than in 1996, indicating a structural change in demand behavior.

Both **ADF and KPSS tests** were used to evaluate stationarity and guide model selection.

### 📈 Final Model Selection

Two SARIMA models are identified as optimal based on performance metrics:

- SARIMA(0,0,1)(0,1,1)
- SARIMA(3,0,1)(4,1,1)

These models provide the best trade-off across:
- AIC
- RMSE
- MAE
- MAPE

---



---

## 💡 Business Insight
- ATM cash demand is highly seasonal
- Weekly patterns can guide cash replenishment cycles
- Year-end spikes require operational planning
