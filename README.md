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

## PM2.5 Actual vs Predicted
![PM2.5 Prediction]("download.png")
**Evaluation Metrics:**
  - RMSE: 13.76
  - MAE: 6.27
  - MAPE: 16.80%
  - MSE: 189.41
