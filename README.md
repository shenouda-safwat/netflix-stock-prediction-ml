# 🎬 Netflix Stock Price Prediction Using Linear Regression

---

## 📈 Project Overview

This project predicts the **closing stock price** of Netflix using **Linear Regression** based on historical stock data.  
It includes **data preprocessing**, **technical feature engineering**, **time-series modeling**, and comprehensive evaluation using multiple **regression metrics**.  
The model provides accurate predictions and can serve as the base for more complex forecasting systems.

---

## 🗂️ Dataset

The dataset contains daily historical stock data for Netflix:

### **Price & Technical Features**
- `Open`  
- `High`  
- `Low`  
- `Volume`  
- `MA50` – 50-day Moving Average  
- `MA200` – 200-day Moving Average  

### **Target Variable**
- `Close`: Closing stock price (regression target)

📦 Dataset File: `archive.zip`

---

## 🔍 Data Preprocessing

- Handled missing values (if any)  
- Created moving averages: **MA50**, **MA200**  
- Scaled features if necessary  
- Applied **time-series split** (no shuffling):  
  - **Training set**: 80%  
  - **Test set**: 20%

---

## 📊 Feature Selection

features = ['Open', 'High', 'Low', 'Volume', 'MA50', 'MA200']


## 🤖 Model Training
Used Linear Regression from scikit-learn:


from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
##🧮 Model Performance
Metric	Value
R² Score	0.9987
Mean Absolute Error (MAE)	4.72
Mean Squared Error (MSE)	40.05
Root Mean Squared Error	6.33
Median Absolute Error	3.39
Max Error	26.25
Explained Variance Score	0.9987
Mean Squared Log Error	0.0001 ✅

📊 The model achieved very high accuracy and low error, making it suitable for financial forecasting tasks.

## 📈 Visualization
📉 Actual vs Predicted Closing Price plot

📋 Top Prediction Errors table

📊 Bar Chart for error metrics

🥧 Pie Chart for variance distribution

(Optional) Residual plots or trend comparison

## 🚀 How to Run
Clone the repository and install dependencies:


git clone https://github.com/shenouda-safwat/netflix-stock-prediction-ml.git
cd netflix-stock-prediction-ml
pip install -r requirements.txt
Then open the notebook:


jupyter notebook "Netflix Stock Price Prediction using Linear Regression.ipynb"
## 🔮 Future Enhancements
Use advanced models like Random Forest, XGBoost, or LSTM

Add more technical indicators: MACD, RSI, Bollinger Bands

Deploy a Streamlit dashboard for real-time stock input and prediction

Integrate live stock data APIs (e.g., Yahoo Finance, Alpha Vantage)

👨‍💻 Author
## Eng. Shenouda Safwat
📌 LinkedIn
🐙 GitHub

