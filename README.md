```
╔══════════════════════════════════════════════════════════════╗
║       Stock Market Analysis and Prediction using Python      ║
╚══════════════════════════════════════════════════════════════╝
```

```
Analyzed real stock data using ARIMA, co-integration, AR models,
and machine learning regression techniques including Linear,
Polynomial, and Logistic Regression in Python.
```

---

## About the Project

```
This is a complete end-to-end Big Data Analytics project that covers
time series forecasting, statistical testing, and machine learning
on real stock market data.

Stocks Analyzed  :  HCA Healthcare (HCA)
                    General Mills (GIS)
                    Sempra Energy (SRE)

Data Source      :  Yahoo Finance (via yfinance)
Date Range       :  January 1, 2022 to November 30, 2025
```

---

## Project Structure

```
BDA_Project/
│
├── BDA_Project.ipynb        # Main Jupyter Notebook
│
├── Part 1  →  Data Import and Visualization
├── Part 2  →  ARIMA Models
├── Part 3A →  Co-integration Testing
├── Part 3B →  Autocorrelation and AR Models
└── Part 4  →  Supervised Learning (Regression)
```

---

## Part 1: Data Import and Visualization

```python
# Tickers used
tickers = ["HCA", "GIS", "SRE"]

# Date range
start = 2022-01-01
end   = 2025-11-30

# What was done
- Downloaded daily closing prices using yfinance
- Plotted all three stocks on a single line chart
- Observed price trends over 3 years
```

---

## Part 2: ARIMA Models

```python
# Model used
ARIMA(order=(10, 0, 1))   # ARMA (no differencing)

# Train/Test Split
train = 80%
test  = 20%

# Applied on
- HCA Healthcare Inc  (HCA)
- General Mills Inc   (GIS)
- Sempra Energy       (SRE)

# Evaluation Metrics
MAE   →  Mean Absolute Error
MSE   →  Mean Squared Error
RMSE  →  Root Mean Squared Error

# Output
- Actual vs Predicted stock price plots for each stock
```

---

## Part 3A: Co-integration Testing

```python
# Tests Applied
ADF Test (Augmented Dickey-Fuller)
  → Checks if each stock is stationary
  → p-value < 0.05  =>  Stationary
  → p-value > 0.05  =>  Non-Stationary

Engle-Granger Co-integration Test
  → Checks long-run relationship between stock pairs
  → p-value < 0.05  =>  Stocks are Co-integrated
  → p-value > 0.05  =>  Stocks are NOT Co-integrated

# Pairs Tested
- HCA  vs  GIS
- HCA  vs  SRE
- GIS  vs  SRE
```

---

## Part 3B: Autocorrelation and AR Models

```python
# ACF Plot
plot_acf(series, lags=30)
  → Plotted for HCA, GIS, and SRE

# AutoReg (AR) Model
AutoReg(series, lags=1).fit()
  → Trained on 80% data
  → Full model summary printed for each stock
```

---

## Part 4: Supervised Learning

```python
# Dataset (Custom Employee Data)
Columns:
  Years_Experience  →  Independent Variable
  Interview_Score   →  Additional Feature
  Salary            →  Target (Regression)
  Promoted          →  Target (Logistic: 0=No, 1=Yes)

# Models Applied

1. Simple Linear Regression
   X = Years_Experience
   y = Salary
   Metrics: MSE, RMSE, R²

2. Multiple Linear Regression
   X = [Years_Experience, Interview_Score]
   y = Salary
   Metrics: MSE, RMSE, R²

3. Polynomial Regression  (degree=2)
   X = Years_Experience
   y = Salary
   Metrics: MSE, RMSE, R²

4. Logistic Regression
   X = Years_Experience
   y = Promoted
   Metrics: Accuracy, Confusion Matrix
```

---

## Technologies Used

```
Language    :  Python 3
Libraries   :  pandas
               numpy
               matplotlib
               seaborn
               yfinance
               statsmodels
               scikit-learn
               scipy
```

---

## Evaluation Summary

```
Model                    Metrics Used
─────────────────────────────────────────────
ARIMA                    MAE, MSE, RMSE
AR Model                 Model Summary Table
Simple Linear Reg.       MSE, RMSE, R²
Multiple Linear Reg.     MSE, RMSE, R²
Polynomial Regression    MSE, RMSE, R²
Logistic Regression      Accuracy, Confusion Matrix
```

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/BDA_Project.git
   ```

2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn yfinance statsmodels scikit-learn scipy
   ```

3. Open the notebook:
   ```bash
   jupyter notebook BDA_Project.ipynb
   ```

4. Run all cells from top to bottom.

---

## 📝 License

This project is intended for **academic and non-commercial use only**.

---

## 📝 License
 
This project is intended for **academic and non-commercial use only**.
 
---

## 📧 Author

**Fawad Saqib**  
💬 Reach out via GitHub for feedback or collaboration!
