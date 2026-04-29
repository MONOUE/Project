## 📊 Project Overview

This project is based on stock ranking methods inspired by existing literature. The model learns at each time \( t \) to predict the ranking of stocks at time \( t+1 \). It assigns a score to each stock, where higher scores correspond to higher expected future returns.

---

## 📁 Dataset

We use daily stock data from a Kaggle challenge covering S&P 500 companies from 2010 to 2022. The dataset includes stocks listed on the NASDAQ exchange, and we remove stocks with missing daily observations.

For each stock, we use the following price data:
- Open price  
- Close price  
- High price  
- Low price  
- Adjusted close price  

---

## 🛠 Feature Engineering

We construct additional features to improve model performance:
- Moving averages over 5, 12, 26, 30, and 50-day windows  
- Daily returns  

---

## 📈 Evaluation

The model is evaluated using the Normalized Discounted Cumulative Gain (NDCG), which compares the predicted ranking with the actual ranking of stocks.