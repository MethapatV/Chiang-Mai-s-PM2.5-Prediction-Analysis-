# Chiang Mai's PM2.5 Prediction Analysis

## Project Overview
This project investigates air quality in Chiang Mai, Thailand, by predicting PM2.5 levels using historical weather data and machine learning techniques. PM2.5, a dangerous air pollutant, has impacted public health in Northern Thailand for nearly a decade. Using XGBoost and lag feature engineering, this project builds a predictive model to support environmental decision-making.

## Dataset
- Time range: **July 11, 2016 – June 30, 2023**
- Features: date, humidity, wind speed, temperature, precipitation, evaporation, atmospheric pressure, sunshine duration, PM2.5
- Target variable: **PM2.5**
- Data split: 
  - Training set: data before 2022
  - Testing set: data from 2022 onward

## ⚙️ Model Details
- **Algorithm:** XGBoost Regressor
- **Evaluation Metrics:**
  - RMSE: 13.76
  - MAE: 6.27
  - MAPE: 16.80%
  - MSE: 189.41

## 🔍 Key Insights
- Strong seasonal pattern: PM2.5 peaks in early months of each year
- Humidity shows a **negative correlation** with PM2.5. This suggests that as humidity increases, there is a tendency for PM 2.5 concentrations to decrease.
- Predictions slightly underestimate values after Feb 2023, likely due to external/unseen events
