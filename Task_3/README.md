# Task 3: Heart Disease Prediction & Data Cleaning

## 📌 Project Overview
This project involves a comprehensive health data analysis aimed at predicting the presence of heart disease in patients. It combines intensive data preprocessing (cleaning, renaming, and outlier management) with machine learning classification to create a reliable diagnostic tool.



## 🎯 Objectives
* **Data Refinement**: Clean the dataset by renaming technical column names for better readability and removing duplicate records.
* **Outlier Management**: Use statistical methods (IQR) to identify and cap outliers in critical health metrics.
* **Feature Engineering**: Transform categorical data into numerical format and scale variables for optimized model performance.
* **Comparative Modeling**: Train and compare **Logistic Regression** and **Decision Tree** models to find the most accurate classifier.

## 🛠️ Tech Stack
* **Python**: Core logic.
* **Pandas/NumPy**: For data manipulation and IQR calculations.
* **Seaborn/Matplotlib**: For correlation heatmaps and confusion matrices.
* **Scikit-Learn**: For One-Hot Encoding, scaling, and classification algorithms.

## 📊 Data Processing Workflow
1.  **Cleaning**: Removed duplicate entries and renamed columns (e.g., `trestbps` to `RestingBP`) to ensure clinical clarity.
2.  **Outlier Handling**: Applied the **Interquartile Range (IQR)** method to cap extreme values in blood pressure and cholesterol, ensuring they don't skew the model results.
3.  **Encoding & Scaling**: 
    * Converted categorical variables (like Thalassemia and Chest Pain type) using **One-Hot Encoding**.
    * Normalized numerical features using **StandardScaler** to give all health metrics equal weight.
4.  **Evaluation**: Used **Confusion Matrices** and **Classification Reports** (Precision, Recall, F1-Score) to assess model reliability.

## 🔍 Key Findings & Insights
* **Feature Relationships**: The correlation heatmap revealed which factors (such as Maximum Heart Rate and ST Depression) have the strongest impact on heart disease probability.
* **Model Accuracy**: Logistic Regression provided a solid baseline, while the Decision Tree offered a clear hierarchical view of the most critical health markers.
* **Data Quality**: Handling outliers significantly reduced the "noise" in the dataset, leading to more generalized and trustworthy predictions.

## 🚀 How to Use
1.  Install dependencies: `pip install pandas numpy seaborn scikit-learn matplotlib`.
2.  Open the Jupyter Notebook: `Task_3_Heart_Disease.ipynb`.
3.  Follow the step-by-step cleaning and training process to see the final model comparison.

---
**Prepared by:** Shan Ali
**Internship Task:** AI/ML Internship - Phase 3
