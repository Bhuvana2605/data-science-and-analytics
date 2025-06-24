# 📈 Stock Price Forecasting: ARIMA, SARIMA, Prophet & LSTM

This project demonstrates stock price trend forecasting using both statistical and deep learning-based time series models. Historical stock data of Apple Inc. (AAPL) was collected from Yahoo Finance and analyzed using ARIMA, SARIMA, Prophet, and LSTM.

---

## 🧰 Tools & Libraries

- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Plotly  
- **Models**: 
  - ARIMA, SARIMA (via `statsmodels`)
  - Prophet (by Facebook)
  - LSTM (via TensorFlow/Keras)
- **Others**: scikit-learn for evaluation, yFinance for data collection

---

## 📊 Dataset

- **Source**: Yahoo Finance  
- **Ticker**: `AAPL`  
- **Timeframe**: 2020-01-01 to 2024-12-31  
- **Features Used**: `Close` price  

---

## 🧹 Preprocessing

- Removed missing values
- Converted index to datetime format
- Normalized values for LSTM using `MinMaxScaler`
- Split data into training and test sets

---

## 🧠 Models Implemented

### 🔢 ARIMA
- Manual order tuning
- Short-term forecasting with trend modeling

### 🔄 SARIMA
- Extended ARIMA with seasonality detection
- Auto-tuned using `auto_arima`

### 🔮 Prophet
- Handled trends and seasonality with built-in holidays support
- Used Stan-based backend

### 🤖 LSTM
- Deep learning model for capturing sequential dependencies
- Trained on scaled sequences using `TensorFlow/Keras`

---

## 📈 Forecasting Visuals

Each model’s predictions were plotted alongside actual values to compare accuracy and trend capture.

---

## 📏 Evaluation Metrics

Each model was evaluated using:
- **MAE** (Mean Absolute Error)
- **RMSE** (Root Mean Squared Error)

---

### 📋 Model Comparison Table (Before Tuning)

| Model    | MAE     | RMSE    | Notes                            |
|----------|---------|---------|----------------------------------|
| ARIMA    | 24.83   |  29.26  | Basic p,d,q values               |
| SARIMA   | 15.78   | 18.26   | Default seasonal settings        |
| Prophet  | 5.09    | 6.62    | Default parameters               |
| LSTM     | 7.90    | 9.76    | Basic model structure            |

---

### 📋 Final Model Comparison Table (After Hyperparameter Tuning)

| Model    | MAE     | RMSE    | Notes                                      |
|----------|---------|---------|--------------------------------------------|
| ARIMA    | 15.26   | 18.26   | Tuned (p, d, q) values manually             |
| SARIMA   | 15.78   | 18.26   | Seasonal tuning with `auto_arima`          |
| Prophet  |  4.39   |  5.74   | Tuned `changepoint_prior_scale`, holidays  |
| LSTM     | 6.81    | 7.77    | Tuned epochs, neurons, and batch size      |

---

## 🎯 Key Takeaways

- ARIMA & SARIMA are fast and interpretable, good for basic trends
- Prophet handles seasonal changes and trends automatically
- LSTM performs well on nonlinear patterns but needs tuning and scaling
- Tuning significantly improves model performance in all cases

---

## 🧪 Learning Outcomes

- Collected and preprocessed financial time series data
- Implemented and compared four forecasting models
- Visualized model performance
- Evaluated models using standard regression metrics
- Tuned models for improved forecasting accuracy

---


---

## 💻 How to Run

1. Clone the repo or download the files
2. Open the notebook with Jupyter or Google Colab
3. Run all cells to view predictions and performance

---

## 👨‍🎓 Created For

This project was created as part of a data science internship and serves as a portfolio-ready example of financial time series forecasting using both statistical and deep learning techniques.


