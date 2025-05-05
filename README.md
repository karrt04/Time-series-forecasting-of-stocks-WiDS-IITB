# Stock Price Forecasting – WiDS 2023

This repository contains the solution submitted for the **Winter in Data Science (WiDS) Hackathon 2024**, focused on forecasting the stock price of Tata Motors using classical time series modeling techniques.

## Problem Statement

The task was to predict future stock prices using historical data from Tata Motors. The goal was to build interpretable and statistically sound models for short-term stock forecasting.

## Approach

Our approach involved the following steps:

- **Data Cleaning and Preprocessing**:
  - Parsed and aligned timestamps
  - Removed missing entries
  - Inferred frequency and ensured temporal regularity

- **Exploratory Data Analysis**:
  - Visual inspection of stock trends
  - First-order differencing to achieve stationarity
  - ACF/PACF plots for parameter selection

- **Modeling**:
  - **ARIMA Model**: Used for modeling the "Open" stock prices after differencing
  - **SARIMA Model**: Considered for incorporating seasonality
  - **Residual Modeling**: ARIMA model fit on residuals for improving forecast quality

- **Evaluation**:
  - Actual vs. Predicted plots
  - RMSE and visual inspection for accuracy

> **Note**: Though deep learning models like LSTM were considered, they were not implemented in this submission. They remain a promising direction for future work.

## Results

- The ARIMA model demonstrated strong performance on short-term forecasting
- Residual analysis indicated potential for hybrid models
- Time-series decomposition and evaluation were visualized effectively


