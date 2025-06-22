Big Mart Sales Prediction
This project focuses on building a regression model to predict the sales of items across various Big Mart outlets. It involves data preprocessing, feature engineering, and advanced machine learning modeling to improve the prediction accuracy.

Project Objective
To develop a machine learning model that can accurately predict the Item_Outlet_Sales variable using historical sales data provided by Big Mart. This helps in demand forecasting and inventory management.

Dataset
Source: Big Mart Sales data (structured CSV format)

Target Variable: Item_Outlet_Sales

Features: Includes item attributes (e.g., weight, type, MRP), and outlet details (e.g., location, size, type)

Steps Implemented
1. Data Preprocessing
Handled missing values in Item_Weight and Outlet_Size
Replaced zeros in Item_Visibility with mean values
Standardized category labels in Item_Fat_Content

2. Feature Engineering
Derived new variables: Outlet_Age, Item_Type_Combined, MRP_Bins
Created categorical bins and frequency-based transformations
Applied log transformation to skewed target variable

3. Encoding
LabelEncoded and OneHotEncoded categorical features
Removed high-cardinality or non-numeric columns as needed

4. Modeling
Baseline models: Linear Regression, Ridge, Lasso
Tree-based models: Random Forest, XGBoost
Final model: Voting Regressor combining Ridge, Lasso, and Random Forest
Evaluated models using RMSE and cross-validation

5. Evaluation
Plotted Actual vs Predicted sales
Extracted and analyzed feature importance
Achieved significant reduction in error via ensemble techniques

Technologies Used
Python 3
Pandas, NumPy for data manipulation
Matplotlib, Seaborn for visualization
Scikit-learn for modeling and preprocessing
XGBoost for gradient boosting models

Output
Final trained model
Evaluation plots and metrics
CSV export of predictions for all items

How to Run
Clone the repository
Upload Train.csv file to your environment
Run bigmart_sales_prediction.ipynb in Jupyter or Google Colab

The notebook will generate the predictions and evaluate model performance
