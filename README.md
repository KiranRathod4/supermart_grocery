# supermart_grocery
## Summary:

### Data Analysis Key Findings

*   The dataset contains 9994 entries with no missing values.
*   Numerical features like 'Sales', 'Discount', and 'Profit' show varying distributions and ranges.
*   EDA revealed a negative correlation between 'Discount' and 'Profit'.
*   Sales and Profit vary significantly across different categories, subcategories, regions, and states.
*   New features were successfully engineered from the 'Order Date' column, including year, month, day of the week, day, and days since the earliest order.
*   Categorical variables were successfully one-hot encoded, and selected numerical features were scaled.
*   A Linear Regression model was trained to predict 'Sales'.
*   The Linear Regression model performed poorly, with a high Mean Squared Error (MSE) of 333887.43 and a negative R-squared (R2) of -0.01, indicating it explains almost none of the variance in sales and performs worse than predicting the mean.

### Insights or Next Steps

*   The current Linear Regression model is not suitable for predicting sales due to its poor performance. More complex models capable of capturing non-linear relationships, such as Random Forest or Gradient Boosting, should be explored.
*   Further feature engineering and selection, including exploring interaction terms and potentially incorporating external data, are necessary to improve model performance.

# Supermart Grocery Sales Analysis and Prediction

## Project Overview

This project analyzes the Supermart Grocery Sales dataset to perform exploratory data analysis (EDA), feature engineering, and build a machine learning model to predict sales or profit. The goal is to gain insights into the sales data and develop a predictive model.

## Dataset

The dataset contains information about grocery orders, including:

- Order ID
- Customer Name
- Category
- Sub Category
- City
- Order Date
- Region
- Sales
- Discount
- Profit
- State

## Project Steps

The project followed these steps:

1.  **Data Loading and Initial Exploration**: Loaded the dataset and performed initial checks for structure and missing values.
2.  **Exploratory Data Analysis (EDA)**: Conducted detailed analysis using visualizations to understand relationships between variables (Sales, Profit, Discount, Category, Region, State, etc.) and identify patterns.
3.  **Feature Engineering**: Created new features from the 'Order Date' column (year, month, day of the week, day, and days since the earliest order).
4.  **Data Preprocessing**: Handled categorical variables using one-hot encoding and scaled numerical features.
5.  **Model Selection and Training**: Selected and trained a Linear Regression model to predict 'Sales'.
6.  **Model Evaluation**: Evaluated the model's performance using Mean Squared Error (MSE) and R-squared.
7.  **Conclusion and Next Steps**: Summarized the findings, discussed the model's performance, and outlined potential future work.

## Key Findings

*   The dataset is clean with no missing values.
*   There is a negative correlation observed between 'Discount' and 'Profit'.
*   Sales and Profit show variations across different categories, subcategories, regions, and states.
*   The Linear Regression model performed poorly in predicting sales (MSE: 333887.43, R2: -0.01), indicating it is not suitable for this task.

## Next Steps

*   Explore more complex machine learning models like Random Forest, Gradient Boosting, or XGBoost.
*   Perform further feature engineering and selection to improve model performance.
*   Consider outlier detection and handling.
*   Analyze feature importances from better-performing models.
*   Investigate potential external data sources that could enhance predictions.

## Tools and Libraries

*   Python
*   Pandas
*   NumPy
*   Matplotlib
*   Seaborn
*   Scikit-learn

## How to Run the Code

1.  Ensure you have Python and the necessary libraries installed.
2.  Download the dataset.
3.  Run the code cells in the notebook sequentially.
