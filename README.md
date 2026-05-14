# Stock Market Analysis and Prediction using Python

Analyzed real stock data using ARIMA, co-integration, AR models, and machine learning regression techniques including Linear, Polynomial, and Logistic Regression in Python.

---

## About the Project

This is a complete end-to-end Big Data Analytics project that covers time series forecasting, statistical testing, and machine learning on real stock market data. The three companies analyzed are HCA Healthcare, General Mills, and Sempra Energy using historical data from January 2022 to November 2025 fetched directly from Yahoo Finance.

---

## Project Structure

The project is divided into four main parts.

**Part 1: Data Import and Visualization**
Daily closing prices for all three stocks were downloaded using the yfinance library. The data was then plotted on a single chart to observe price trends over the three year period.

**Part 2: ARIMA Models**
An ARIMA model was built for each of the three stocks to forecast future stock prices. The data was split into 80% training and 20% testing. Model performance was measured using MAE, MSE, and RMSE. A plot of actual vs predicted prices was generated for each stock.

**Part 3A: Co-integration Testing**
The Augmented Dickey-Fuller test was applied on each stock to check whether it is stationary. Then the Engle-Granger co-integration test was used on all three pairs of stocks to find out if any long-run relationship exists between them.

**Part 3B: Autocorrelation and AR Models**
ACF plots were generated for all three stocks with 30 lags to visualize autocorrelation. An Autoregressive (AR) model with 1 lag was then trained on each stock and a full model summary was printed.

**Part 4: Supervised Learning**
A custom employee dataset was created with features like Years of Experience and Interview Score. Four machine learning models were applied on this dataset. Simple Linear Regression and Multiple Linear Regression were used to predict Salary. Polynomial Regression of degree 2 was also applied to capture non-linear patterns. Logistic Regression was used to predict whether an employee gets Promoted or not.

---

## Technologies Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- yFinance
- Statsmodels
- Scikit-learn
- SciPy

---

## Evaluation Summary

| Model | Metrics Used |
|---|---|
| ARIMA | MAE, MSE, RMSE |
| AR Model | Model Summary Table |
| Simple Linear Regression | MSE, RMSE, R² |
| Multiple Linear Regression | MSE, RMSE, R² |
| Polynomial Regression | MSE, RMSE, R² |
| Logistic Regression | Accuracy, Confusion Matrix |

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

## 📧 Author

**Fawad Saqib**  
💬 Reach out via GitHub for feedback or collaboration!
