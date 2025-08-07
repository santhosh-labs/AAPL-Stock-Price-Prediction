# 📈 Apple Stock Price Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![ML Model](https://img.shields.io/badge/Model-XGBoost-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)


This project predicts Apple Inc.'s future stock prices using historical data and advanced features, trained on an XGBoost regression model. It involves data cleaning, feature engineering, model building, and performance evaluation.

---

## 📚 Table of Contents
- Project Introduction  
- What This Does  
- Source of Data  
- Model Testing & Comparisons  
- Clone This Repository  
- Author  

---

## 🧠 Project Introduction

Predict Apple's stock prices using XGBoost regression on historical data. The project includes preprocessing, feature engineering, model training, and evaluation using RMSE and R² metrics, with result visualization.

---

## 🔍 What This Does

- Loads historical Apple Inc. stock data  
- Generates advanced technical indicators and lag features  
- Trains XGBoost models for multiple target variables  
- Evaluates model performance using RMSE and R²  
- Visualizes predicted vs actual stock price trends  

---

## 📂 Source of Data

The dataset includes original and engineered features:

### 🔢 Original Features
- `Date`: Trading day in YYYY-MM-DD format  
- `Open`: Opening price of the day  
- `High`: Highest price of the day  
- `Low`: Lowest price of the day  
- `Close`: Closing price of the day  
- `Adj Close`: Adjusted close price (for dividends, splits)  
- `Volume`: Number of shares traded  

### 🧠 Engineered Features
- `DayOfWeek`: Day of the week (0 = Monday, ..., 6 = Sunday)  
- `Month`: Numeric month of the year  
- `Daily Return`: Percentage return from the previous close  
- `Close Prev-1/Prev-2`: Lagged close values from 1 and 2 days before  
- `High Prev-1/Prev-2`, `Open Prev-1/Prev-2`: Lagged values of other features  
- `Price_Range`: Difference between high and low price  
- `Daily_Change`: Change between open and close  
- `Volume_Change`: Percent change in volume  
- `RSI`: Relative Strength Index (momentum indicator)  
- `SMA10`, `SMA20`: 10-day and 20-day Simple Moving Averages  
- `Target High/Low/Close/Open`: Future values (used for supervised prediction targets)  

---

## 📊 Model Testing & Comparisons

Each model is trained for predicting different targets (`Target Close`, `Target High`, etc.).

| Target        | RMSE     | R²       |
|---------------|----------|----------|
| Target High   | 0.004571 | 0.999517 |
| Target Low    | 0.003980 | 0.999629 |
| Target Open   | 0.003832 | 0.999659 |
| Target Close  | 0.005269 | 0.999356 |

---

## 🚀 Clone This Repository

```bash
git clone https://github.com/santhosh-labs/AAPL-Stock-Price-Prediction
```
---
## 👤 Author

Santhosh S — Data Analyst, Focused on deriving actionable insights, simplifying complex data challenges, and delivering data-driven solutions across domains.

💼 LinkedIn: [Santhosh S](https://www.linkedin.com/in/santhosh-portfolio)  
- Let’s connect professionally and grow your data career


