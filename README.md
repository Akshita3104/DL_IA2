# DL_IA2

Team Member 1: Akshita Shetty - 16010422266
Team Member 2: Chaitravi Reddy - 16010422274

# 📈 TCS Stock Price Prediction using LSTM

This project implements a **Multivariate LSTM (Long Short-Term Memory)** model to predict the closing price of **Tata Consultancy Services (TCS)** stock using historical stock market data.

---

## 🔍 Project Overview

The model is trained on features like **Open**, **High**, **Low**, **Close**, and **Volume**. It uses a **sliding window** approach with a sequence length to feed the LSTM model, allowing it to learn temporal dependencies in stock price movement.

---

## 📦 Dataset

The dataset used in this project is fetched from:
https://raw.githubusercontent.com/kalilurrahman/TCSData/main/TCS_stock_history.csv

- Features used: `Open`, `High`, `Low`, `Close`, `Volume`
- The target is the `Close` price.
- Data is normalized using `MinMaxScaler`.

---

## 🧠 Model Architecture

- **Input:** Sequence of past 60 days of stock features.
- **Layers:**
  - LSTM (64–128 units)
  - Dropout (for regularization)
  - Dense (1 unit to predict the next closing price)
- **Loss Function:** Mean Squared Error (MSE)
- **Optimizer:** Adam

---

## 📊 Results

The predicted stock prices are plotted against the actual close prices to visually inspect performance.

> The model captures general trends but underfits sharp spikes and dips. Further improvements are suggested.


