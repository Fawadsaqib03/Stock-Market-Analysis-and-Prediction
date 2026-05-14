# Stock Market Analysis and Prediction using Python
 
Analyzed real stock data using ARIMA, co-integration, AR models, and machine learning regression techniques including Linear, Polynomial, and Logistic Regression in Python.
 
---
 
## About the Project
 
This project is a complete end-to-end Big Data Analytics project that covers time series forecasting, statistical testing, and machine learning on real stock market data. The stocks analyzed are HCA Healthcare (HCA), General Mills (GIS), and Sempra Energy (SRE) using historical data from January 2022 to November 2025 pulled directly from Yahoo Finance.
 
The project also includes a supervised learning section using a custom employee dataset to predict salary and promotion probability.
 
---
 
## Project Structure
 
The project is divided into four parts.
 
**Part 1: Data Import and Visualization**
Downloaded historical closing prices for HCA, GIS, and SRE using the yfinance library and plotted daily stock prices over 3 years to understand trends.
 
**Part 2: ARIMA Models**
Built ARIMA(10, 0, 1) models for each of the three stocks. Split data into 80% training and 20% testing and evaluated model performance using MAE, MSE, and RMSE. Visualized actual vs predicted stock prices.
 
**Part 3A: Co-integration Testing**
Used the Augmented Dickey-Fuller (ADF) test to check stationarity of each stock. Applied the Engle-Granger co-integration test on all three pairs of stocks to find out if any long-run relationship exists between them.
 
**Part 3B: Autocorrelation and Autoregressive (AR) Models**
Plotted ACF (Autocorrelation Function) graphs for all three stocks with 30 lags. Built AR(1) models using AutoReg for each stock and printed full model summaries.
 
**Part 4: Supervised Learning**
Used a custom employee dataset with features like Years of Experience and Interview Score.
Applied four models:
- Simple Linear Regression to predict Salary
- Multiple Linear Regression using two features
- Polynomial Regression (degree 2) to capture non-linear patterns
- Logistic Regression to predict Promotion (Yes or No)
Evaluated all models using MSE, RMSE, R² Score, Accuracy, and Confusion Matrix.
 
---
 
## Technologies Used
 
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Scikit-learn
- yFinance
- SciPy
---
 
## How to Run
 
1. Clone this repository
2. Install the required libraries using the command below
3. Open the notebook and run all cells from top to bottom
```bash
pip install pandas numpy matplotlib seaborn yfinance statsmodels scikit-learn scipy
```
 
---
 
## Dataset
 
Stock data is fetched live from Yahoo Finance using the yfinance library for the following tickers:
 
| Ticker | Company |
|--------|---------|
| HCA | HCA Healthcare Inc |
| GIS | General Mills Inc |
| SRE | Sempra Energy |
 
Date Range: January 1, 2022 to November 30, 2025
 
---
 
## Models and Evaluation Metrics
 
| Model | Metric Used |
|-------|-------------|
| ARIMA | MAE, MSE, RMSE |
| AR Model | Model Summary |
| Linear Regression | MSE, RMSE, R² |
| Polynomial Regression | MSE, RMSE, R² |
| Logistic Regression | Accuracy, Confusion Matrix |
 
---
 
## Author
 
Feel free to connect on LinkedIn or raise an issue if you have any questions about the project.
 
