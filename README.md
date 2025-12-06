NVIDIA Stock Price Predictor + Dashboard
Author: Satya Vemulakonda

Tech Stack: Python, Dash, Scikit-Learn, Plotly

📖 Project Overview
This project is a full-stack stock price prediction and visualization tool focused on NVIDIA (NVDA). It pulls historical daily stock data using the Alpha Vantage API, trains a Random Forest regression model to forecast future closing prices, and displays the results in an interactive Dash dashboard with Plotly visualizations.

Unlike simple scripts, this project demonstrates a secure production workflow using environment variables for API key management and modular functions for data processing.

🚀 Features
Real-time Data Fetching: Pulls daily NVDA stock price and volume data via Alpha Vantage.

Advanced Feature Engineering: Calculates Lagged Prices, Moving Averages (MA10, MA50), Volatility, Momentum, and Volume Change.

Time-Series Modeling: Uses a Random Forest Regressor trained on an 80/20 chronological split to respect time-series constraints.

Interactive Dashboard:

Trend Analysis: Line chart comparing Actual vs. Forecasted closing prices.

Future Simulation: A generated candlestick chart simulating the next 60 business days.

Performance Metrics: automatically calculates and displays Mean Absolute Error (MAE).

🛠️ Getting Started
1. Prerequisites

Python 3.x

A free API key from Alpha Vantage

2. Installation

Clone the repository and install the dependencies:

Bash
git clone https://github.com/yourusername/nvda-stock-predictor.git
cd nvda-stock-predictor
pip install -r requirements.txt
3. Security Setup

Create a file named .env in the root directory. This keeps your API key secure and out of the source code:

Plaintext
ALPHA_VANTAGE_KEY=your_actual_api_key_here
4. Run the Dashboard

Bash
python app.py
Open your web browser to http://127.0.0.1:8051/ to view the live dashboard.

⚠️ Disclaimer
This project is for educational and portfolio purposes. It uses lagging technical indicators for prediction and should not be used for financial trading decisions.
