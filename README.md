# Customer Spending Score Prediction

## **Overview**

This project leverages **supervised learning techniques** to predict **Spending Scores** of customers based on key features such as **Age**, **Annual Income**, and **Gender**. By analyzing customer spending behavior, the project aims to enable businesses to make **data-driven decisions** to:

- Optimize marketing strategies.
- Improve customer retention.
- Allocate resources more efficiently.

---

## **Objectives**

1. Develop a **predictive model** to estimate customer Spending Scores.
2. Provide **insights** into relationships between customer demographics and spending behavior.
3. Lay the groundwork for **personalized marketing strategies** and **customer segmentation**.

---

## **Problem Statement**

Understanding customer spending behavior is crucial for businesses to:
- **Optimize marketing efforts** by targeting the right customer segments.
- **Identify high-value customers** for loyalty programs or premium services.
- **Maximize ROI** by focusing resources on impactful strategies.

Predicting Spending Scores helps solve the challenge of effectively targeting customer groups and improving overall business decision-making.

---

## **Approach**

1. **Exploratory Data Analysis (EDA)**:
    - Analyzed the distribution of features such as Age, Gender, Annual Income, and Spending Score.
    - Visualized relationships and trends using **histograms**, **scatterplots**, and a **correlation heatmap**.

2. **Data Preprocessing**:
    - Verified data quality and handled missing values (none in this dataset).
    - Converted the categorical feature **Gender** into numerical format.
    - Normalized continuous variables like **Age** and **Annual Income** to improve model performance.

3. **Model Building**:
    - Implemented a **Linear Regression** model as a baseline.
    - Compared results from:
        - **Manual implementation** using the Normal Equation.
        - **Scikit-learn's Linear Regression**.
    - Enhanced model performance by testing **polynomial regression** (quadratic and cubic).

4. **Model Evaluation**:
    - Evaluated the model using:
        - **Mean Squared Error (MSE)**.
        - **R-squared (R²)**.
    - Compared model performance to the baseline (mean prediction).

---

## **Key Findings**

### **Model Performance**
- **Variance of Spending Score**: `663.52`
- **Baseline MSE**: `663.52`
- **Linear Model MSE**: `480.67`
- **R² (Linear Regression)**: `0.0255`

### **Insights**
1. **Linear Regression**:
    - Reduced MSE compared to the baseline, capturing some relationships between features and Spending Scores.
    - Low R² value indicates limited explanatory power and the need for additional features.
2. **Polynomial Regression**:
    - Quadratic and cubic models captured **non-linear trends**, improving fit to the data.
    - **Cubic regression** performed best, with an R² of `0.073` and MSE of `460.12`.

---

## **Features in Dataset**

- **CustomerID**: Unique identifier for each customer (not used in modeling).
- **Gender**: Male (`1`) or Female (`0`).
- **Age**: Customer age in years.
- **Annual Income**: Annual income in thousands of dollars.
- **Spending Score**: A score from 1-100 representing spending habits (target variable).

---

## **Visualizations**

1. **Age Distribution**:
    - Histogram revealing age concentration in the 30-50 range.
2. **Spending Score Distribution**:
    - Violin plot showcasing spending behavior variability across ages.
3. **Spending Score by Gender**:
    - Boxplot comparing spending patterns between males and females.
4. **3D Scatterplot**:
    - Visualized Spending Score trends across **Age** and **Annual Income**.
5. **Correlation Heatmap**:
    - Revealed weak correlations between Spending Score and demographic features.

---

## **How to Use**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spending-score-prediction.git
   cd spending-score-prediction

