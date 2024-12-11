# Credit_EDA

## Overview
This project demonstrates **Exploratory Data Analysis (EDA)** on a credit dataset. The dataset contains over **300,000 rows** and **122 columns**, making it a massive dataset ideal for showcasing robust preprocessing and analytical techniques.

The project involves exhaustive data preprocessing, visualization, and analysis. Finally, a **Logistic Regression model** is trained to verify the effectiveness of the data preprocessing steps.

---

## Important Note
Please **download the raw code file** to run this project locally. The file cannot render properly on GitHub due to the inclusion of multiple charts and images.

---

## Project Workflow

1. **Data Loading and Initial Cleaning:**
    - Columns with more than **47% null values** are removed.

2. **Exploratory Data Analysis:**
    - Distributions of numerical columns are plotted to identify columns for potential modifications.

3. **Outlier Treatment:**
    - Outliers are detected and clipped using the **IQR method**.
    - Null values in nearly normally distributed columns are filled with their **medians**.

4. **Handling Categorical Data:**
    - Null values in categorical columns are filled with their **mode**.
    - **Binning** is performed on categorical columns where applicable.

5. **Bivariate and Multivariate Analysis:**
    - Relationships between columns are explored.
    - Correlation analysis is performed to determine relationships with the **TARGET** and **NAME_CONTRACT_STATUS** columns.

6. **Feature Selection and Dimensionality Reduction:**
    - Highly correlated columns are identified.
    - **Principal Component Analysis (PCA)** is performed to reduce dimensionality and speed up model training.

7. **Logistic Regression Modeling:**
    - Logistic Regression is applied to predict the **NAME_CONTRACT_STATUS** of the previous application.

---

## Logistic Regression Model Results

- **Output Classes:** [\"Approved\", \"Canceled\", \"Refused\", \"Unused offer\"]

- **Performance Metrics:**
  - **Accuracy:** 98% (using K-Fold Cross-Validation)
  - **Confusion Matrix:** Excellent
  - **Precision:** >= 0.95 (for all classes)
  - **Recall:** >= 0.98 (for all classes)
  - **Macro ROC AUC:** 0.998

---

## Key Features of the Project
- Comprehensive preprocessing for handling missing values, outliers, and categorical data.
- Insightful visualizations for better data understanding.
- Advanced feature selection and dimensionality reduction techniques.
- High-performing Logistic Regression model with exceptional metrics.

---

## Future Scope
- Extending analysis to include additional machine learning models.
- Hyperparameter tuning for improved model performance.
- Deployment of the model as a web application.

---

Feel free to reach out for any queries or feedback!
