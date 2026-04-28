# Task 2: Apple (AAPL) Stock Price Prediction

## 📌 Project Overview
This project focuses on time-series forecasting using historical market data. The objective is to build and evaluate machine learning models capable of predicting the **next day's closing price** for Apple Inc. (AAPL) based on daily Open, High, Low, and Trading Volume statistics.



## 🎯 Objectives
* Fetch real-time historical data using the `yfinance` API.
* Perform feature engineering by creating a "Next_Close" target variable.
* Compare the performance of a baseline **Linear Regression** model against a non-linear **Random Forest Regressor**.
* Evaluate model performance using regression metrics (MAE, RMSE, R2 Score).

## 📊 Methodology
1.  **Data Acquisition**: Downloaded 4 years of historical AAPL data (2020–2024).
2.  **Preprocessing**: Engineered the target variable using the `.shift(-1)` method and normalized data using `StandardScaler`.
3.  **Splitting**: Implemented a **chronological train-test split** (`shuffle=False`) to ensure the models do not "peek" into future data during training.
4.  **Modeling**: Trained a linear model to capture linear trends and an ensemble model to capture complex, non-linear market patterns.

## 🛠️ Tools & Libraries
* **Python**: Core programming language.
* **yfinance**: Used to fetch live stock market data.
* **Scikit-Learn**: For data splitting, scaling, and training regression models.
* **Matplotlib/Seaborn**: For plotting actual vs. predicted price trends.

## 🔍 Key Findings & Insights
1.  **Trend Awareness**: Both models successfully captured the general upward trajectory of AAPL stock prices during the testing period.
2.  **Model Performance**: Random Forest generally provided better accuracy in capturing local price fluctuations compared to Linear Regression.
3.  **Data Integrity**: Using `shuffle=False` is critical in time-series forecasting; shuffling would have artificially inflated accuracy by leaking future price information into the training set.
4.  **Metrics**: The **R2 Score** provided a clear indication of how much variance in the closing price our models could explain, while **MAE** gave a clear dollar-value representation of the prediction error.

## 🚀 How to Run
1.  Ensure you have the required libraries installed: `pip install yfinance pandas numpy matplotlib seaborn scikit-learn`.
2.  Open the Jupyter Notebook `Task_2_Stock_Prediction.ipynb`.
3.  Execute the cells to fetch the data and generate the comparison visualizations.

---
**Prepared by:** Shan Ali
**Internship Task:** AI/ML Internship - Phase 2
