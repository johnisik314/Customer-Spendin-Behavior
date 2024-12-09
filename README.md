# Customer Spending Score Prediction

## Overview

This project leverages supervised learning techniques to predict **Spending Scores** of customers based on features like **Age**, **Annual Income**, and **Gender**. By understanding customer spending behavior, businesses can make data-driven decisions to optimize marketing strategies, improve customer retention, and allocate resources more efficiently.

---

## Objectives

The primary goal of this project is to:

1. Develop a predictive model to estimate Spending Scores.
2. Provide insights into the relationships between customer demographics and spending behavior.
3. Lay the groundwork for personalized marketing strategies and customer segmentation.

---

## Problem Statement

Understanding customer spending behavior is crucial for:

- Optimizing marketing strategies.
- Identifying high-value customers.
- Improving ROI on marketing campaigns.

By predicting Spending Scores, this project aims to solve the challenge of targeting customer segments effectively.

---

## Approach

1. **Exploratory Data Analysis**:
    - Analyzed features such as Age, Gender, Annual Income, and Spending Score.
    - Visualized data distributions and relationships using histograms, scatterplots, and heatmaps.

2. **Data Preprocessing**:
    - Handled missing values (none in this dataset).
    - Converted categorical data (Gender) into numerical format.
    - Normalized relevant features for consistency.

3. **Model Building**:
    - Used **Linear Regression** as a baseline supervised learning model.
    - Manually implemented the Normal Equation method for comparison with Scikit-learn's Linear Regression.
    - Evaluated model performance using:
        - **Mean Squared Error (MSE)**
        - **R-squared (R²)**

4. **Model Evaluation**:
    - Compared model predictions to baseline predictions (mean Spending Score).
    - Analyzed performance metrics to assess model effectiveness.

---

## Key Findings

1. **Model Performance**:
    - **Variance of Spending Score**: 663.52
    - **Baseline MSE**: 663.52
    - **Model MSE**: 480.67
    - **R² (Scikit-learn)**: 0.0255

2. **Insights**:
    - The model captures some relationship between features and Spending Scores, as indicated by the reduction in MSE compared to the baseline.
    - However, the low R² value suggests limited explanatory power, indicating the need for:
        - Additional features (e.g., purchase history, geographic location).
        - Nonlinear models or transformations to capture complex relationships.

---

## Features in Dataset

- **CustomerID**: Unique identifier for each customer (not used in the model).
- **Gender**: Male (1) or Female (0).
- **Age**: Customer age in years.
- **Annual Income**: Annual income in thousands of dollars.
- **Spending Score**: A score between 1-100 representing customer spending habits.

---

## Visualizations

1. **Age Distribution**:
    - A histogram showing the distribution of customer ages.
2. **Annual Income by Gender**:
    - A boxplot comparing income distributions for males and females.
3. **Spending Score vs Age**:
    - A scatterplot with gender as a hue to visualize spending trends by age.
4. **Correlation Heatmap**:
    - Highlights relationships between Age, Annual Income, Gender, and Spending Score.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spending-score-prediction.git
   cd spending-score-prediction
