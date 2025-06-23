🎬 Netflix Stock Price Prediction Using Linear Regression
📈 Project Overview
This project predicts Netflix's stock **closing price** based on historical stock market data using **Linear Regression**.

It involves:
- Data preprocessing  
- Feature engineering  
- Time-series-aware train/test split  
- Linear Regression modeling  
- Full evaluation using multiple metrics  
- Data visualization  
- (Optional) future extension to interactive dashboards or advanced models

---

🗂️ Dataset

The dataset includes historical stock data for Netflix with the following features:
- `Open` – Opening stock price  
- `High` / `Low` – Day’s price range  
- `Volume` – Number of traded shares  
- `MA50`, `MA200` – Moving averages for trend analysis  
- `Close` – Target variable (closing price of the stock)

📦 File: `archive.zip`

---

🔍 Data Preprocessing

- Handled missing values  
- Engineered technical indicators (`MA50`, `MA200`)  
- Normalized feature scales  
- Applied **time-series split** (no shuffling):
  - Training Set: 80%  
  - Test Set: 20%

---

📊 Feature Set

```python
features = ['Open', 'High', 'Low', 'Volume', 'MA50', 'MA200']
