## NVIDIA Stock Price Predictor + Dashboard

**Author:** Satya Vemulakonda  
**Date:** July 2025  

---

## Project Overview

This project is a full-stack stock price prediction and visualization tool focused on NVIDIA (NVDA). It pulls historical daily stock data using the Alpha Vantage API, trains a Random Forest regression model to forecast future closing prices, and displays the results in an interactive Dash dashboard with Plotly visualizations.

The entire pipeline — from data collection and processing to modeling and dashboard display — is contained within a single Python script, making it easy to run without additional setup.

---

## Features

- Fetches daily NVDA stock price and volume data from Alpha Vantage  
- Performs feature engineering with lagged prices, moving averages, volatility, momentum, and volume change  
- Splits data into training and testing sets based on date  
- Trains a Random Forest Regressor to predict next-day closing prices  
- Generates rolling predictions on the test set  
- Forecasts stock prices for the next 60 business days  
- Visualizes results with two dashboard tabs:  
  - Line chart comparing actual vs. forecasted closing prices  
  - Candlestick chart simulating 60-day forecast  
- Displays model performance using Mean Absolute Error (MAE)  

---

## Getting Started

### Prerequisites

- Python 3.x  
- Packages: `pandas`, `numpy`, `scikit-learn`, `plotly`, `dash`, `alpha_vantage`  

Install required packages via pip:
```bash
pip install pandas numpy scikit-learn plotly dash alpha_vantage
