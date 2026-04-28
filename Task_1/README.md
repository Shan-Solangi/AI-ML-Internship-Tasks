# Task 1: Exploratory Data Analysis on Iris Dataset

## 📌 Project Overview
This project focuses on performing a comprehensive Exploratory Data Analysis (EDA) on the classic Iris dataset. The primary goal is to understand the relationships between various physical measurements of three flower species—Setosa, Versicolor, and Virginica—and identify which features are most significant for classification.



## 🎯 Objectives
* Perform initial data inspection and statistical summaries.
* Visualize relationships between sepal and petal features using scatter plots.
* Analyze feature distributions through histograms and density plots.
* Identify outliers within the species using box plots.
* Determine feature importance for distinguishing between species.

## 📊 Dataset Description
The dataset contains 150 samples with 4 features:
1.  **Sepal Length** (cm)
2.  **Sepal Width** (cm)
3.  **Petal Length** (cm)
4.  **Petal Width** (cm)
**Target Variable:** Species (*setosa, versicolor, virginica*)

## 🛠️ Tools & Libraries
* **Python**: Core programming language.
* **Pandas**: For data manipulation and loading.
* **Seaborn/Matplotlib**: For advanced statistical visualizations.

## 🔍 Key Findings & Observations
1.  **Species Separation**: *Setosa* is highly distinct and easily separable from the other two species based on any feature, particularly petal measurements.
2.  **Feature Importance**: Petal Length and Petal Width are far superior predictors for classification compared to Sepal measurements.
3.  **Data Distribution**: 
    * Sepal Width follows a normal distribution.
    * Petal Length and Width exhibit bimodal distributions, highlighting the distinct gap between species.
4.  **Outliers**: The dataset is exceptionally clean. Only minor outliers were detected in the Sepal Width and Petal Length columns, which do not significantly impact analysis.

## 🚀 How to Run
1.  Ensure you have Python installed.
2.  Install required libraries: `pip install pandas seaborn matplotlib`.
3.  Open the Jupyter Notebook `Task_1_Iris_EDA.ipynb`.
4.  Run all cells to generate the analysis and visualizations.

---
**Prepared by:** Shan Ali
**Internship Task:** AI/ML Internship - Phase 1
