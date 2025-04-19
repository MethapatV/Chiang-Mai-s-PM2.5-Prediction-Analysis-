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

## Model Detail
- **Algorithm:** XGBoost Regressor

## PM 2.5 Prediction
![PM2.5 Prediction](https://github.com/MethapatV/Chiang-Mai-s-PM2.5-Prediction-Analysis-/blob/main/download.png?raw=true)
The XGBoost model predicted PM2.5 levels in Chiang Mai with good initial accuracy, closely matching actual values. However, after February 2023, predictions slightly underestimated PM2.5 levels. Evaluation metrics showed solid performance, with an **RMSE of 13.76**, **MSE of 189.41**, **MAE of 6.27**, and **MAPE of 16.80%**, confirming the model’s reliability. Unfortunately, the prediction is slightly underestimate values after Feb 2023, likely due to external/unseen events.

## Actual VS Predicted Value

![Actual VS Predict](https://github.com/MethapatV/Chiang-Mai-s-PM2.5-Prediction-Analysis-/blob/main/actual%20vs%20predicted.png)
  
The scatter plot reveals that most predicted values are close to the ideal line, suggesting strong overall model accuracy. However, as actual PM2.5 levels rise, the predictions become more dispersed and tend to underestimate the true values. This pattern supports earlier findings that the model slightly underpredicts PM2.5 after February 2023.

## Key Insights
![Humidity](https://github.com/MethapatV/Chiang-Mai-s-PM2.5-Prediction-Analysis-/blob/main/humid.png)

The analysis reveals a moderate negative correlation between average humidity and PM2.5 levels, indicating that as humidity increases, air pollution tends to decrease. Conversely, lower humidity levels are associated with a noticeable rise in PM2.5 concentrations. **This relationship suggests that humidity plays a significant role in air quality dynamics, and understanding this pattern is essential for developing effective strategies to mitigate pollution and its health impacts.**

## Author
Methapat Vorakamolpisit  
Master's in Analytics – Northeastern University
