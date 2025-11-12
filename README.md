# Car-Price-Prediction
A data science project to predict vehicle MSRP using linear regression, exploratory data analysis (EDA), and forward/backward feature selection with scikit-learn and mlxtend.

🚗 Car Price Prediction Project
This repository contains a data science project to predict the Manufacturer's Suggested Retail Price (MSRP) of vehicles. The entire workflow, from data cleaning to modeling and interpretation, is documented in the Car_Price_Prediction.ipynb Jupyter Notebook.

The project uses a dataset of over 11,000 vehicles and 16 features (such as Engine HP, highway MPG, and Vehicle Size) to build a linear regression model.

workflow Overview
The notebook follows a complete data science pipeline:

Problem Definition: Defines the problem (regression), stakeholders (consumers, dealerships, insurance), and data.

Data Cleaning:

Handles missing values by imputing with median (for numeric features) and mode (for categorical features).

Drops columns with excessive missing data (Market Category).

Removes duplicate records.

Feature Engineering:

Applies One-Hot Encoding to nominal features (Driven_Wheels).

Applies Ordinal Encoding to features with an inherent order (Vehicle Size).

Drops high-cardinality features like Make and Model for the baseline model.

Exploratory Data Analysis (EDA):

Visualizes target variable (MSRP) and key feature (Engine HP) distributions with histograms.

Generates a correlation heatmap to understand relationships between numeric features.

Uses a boxplot to compare MSRP across different Vehicle Size categories.

Modeling & Evaluation:

Splits the data into 80% training and 20% test sets.

Establishes several simple linear regression baselines.

Implements forward and backward stepwise feature selection using the mlxtend library to identify the most predictive set of features.

Conclusion:

Provides a full business-facing interpretation of the final model's performance (R², MAE, MSE).

Discusses the model's limitations (high MAE) and provides clear next steps for improvement, such as log-transforming the skewed MSRP target and applying non-linear models (e.g., Random Forest, XGBoost).

🛠️ Core Libraries Used
Pandas: For data manipulation and cleaning.

Scikit-learn: For data splitting, preprocessing, and linear regression modeling.

Mlxtend: For sequential forward and backward feature selection.

Matplotlib & Seaborn: For exploratory data analysis and visualization.
