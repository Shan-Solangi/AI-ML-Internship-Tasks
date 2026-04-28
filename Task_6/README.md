# Task 6: Housing Price Prediction (Advanced ML Pipelines)

## 📌 Project Overview
This project focuses on predicting real estate market values using a dataset of housing features. Unlike basic regression tasks, this project implements a professional **Machine Learning Pipeline** to automate the transformation of both numerical and categorical data, ensuring a clean and reproducible workflow.



## 🎯 Objectives
* **Modular Preprocessing**: Build a `ColumnTransformer` to handle scaling for numerical data and encoding for categorical data in one step.
* **Pipeline Integration**: Use Scikit-Learn `Pipelines` to prevent data leakage and simplify the model training process.
* **Model Comparison**: Evaluate and compare **Linear Regression** and **Random Forest Regressor** to determine the best fit for housing data.
* **Feature Importance**: Analyze which features (area, bathrooms, location) have the highest impact on property value.

## 📊 Methodology
1.  **Exploratory Data Analysis (EDA)**: Analyzed price distributions and correlations. Identified strong linear relationships between house area and price.
2.  **Automated Transformation**:
    * **Numerical Features**: Standardized using `StandardScaler`.
    * **Categorical Features**: Transformed using `OneHotEncoder` (dropping the first category to avoid the dummy variable trap).
3.  **Pipeline Construction**: Created separate pipelines for Linear Regression and Random Forest to ensure identical preprocessing for both.
4.  **Diagnostic Plotting**: Generated **Residual Plots** and **Error Distribution Histograms** to verify model assumptions and accuracy.

## 🛠️ Tech Stack
* **Python**: Core programming language.
* **Scikit-Learn**: For the full pipeline, transformers, and regression models.
* **Pandas/NumPy**: For data structure and numerical operations.
* **Matplotlib/Seaborn**: For plotting residuals and feature importance.

## 🔍 Key Findings & Insights
* **Top Predictors**: "Area" was identified as the single most important feature, followed by the number of bathrooms and furnishing status.
* **Model Accuracy**: The Random Forest model generally captured the variance in high-end housing prices more effectively than the standard Linear Regression model.
* **Residual Analysis**: The error distribution plots confirmed that the models maintain a relatively low Mean Absolute Error (MAE) across the majority of the test samples.

## 🚀 How to Run
1.  Required libraries: `pip install pandas scikit-learn seaborn matplotlib`.
2.  Place the `Housing.csv` file in the same directory as the notebook.
3.  Open and run `Task_6_Housing_Prediction.ipynb`.

---
**Prepared by:** Shan Ali
**Internship Task:** AI/ML Internship - Phase 6
