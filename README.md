# House_Price_Prediction:A Regression Analysis

This project focuses on predicting residential home prices using Supervised Machine Learning. It involves a comprehensive end-to-end pipeline, from deep exploratory data analysis to model evaluation using robust regression metrics.

📋 Project Overview
The goal is to develop a predictive model that estimates the SalePrice of houses based on various features such as location, square footage, and year built. 
This is a Regression task where the target variable is continuous.
🚀 Key Features
1.Correlation Analysis: Identifying top predictors (e.g., TotalBsmtSF, YearBuilt) using Pearson Correlation Heatmaps.
2.Categorical Distribution: Visualizing the distribution of features like MSZoning and BldgType to understand data frequency and cardinality.
3.Automated Visualization: Implementation of dynamic subplot grids for high-cardinality categorical data.
4.Model Evaluation: Utilizing Mean Absolute Error (MAE) to ensure the model is robust against outliers.

📊 Exploratory Data Analysis (EDA)
1. Feature CorrelationWe utilized a heatmap to analyze the linear relationships between numerical features. Features showing a high correlation with SalePrice (e.g., coefficients > 0.5) were prioritized for model training.
2. Categorical DistributionsTo understand the data's composition, we analyzed the unique counts and distributions of categorical variables using Seaborn bar plots. This helped identify features that required encoding or grouping.

📉 Evaluation Metric
The primary metric used to evaluate model performance is the Mean Absolute Error (MAE).
This represents the average of the absolute differences between the predicted values and actual market prices.
            $$MAE = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$
Why MAE? Unlike Mean Squared Error, MAE is more robust to outliers, providing a clearer picture of the model's typical prediction error in real-world currency terms.

🛠️ Tech StackLanguage: 
    PythonLibraries:Pandas for data manipulation
    Seaborn & Matplotlib for advanced data visualization
    Scikit-learn for machine learning algorithms and evaluation
📂 Folder Structure
housePricePrediction
├── HousePricePrediction.xlsx          # Raw and processed datasets
├── housePricePrediction.ipynb         # Jupyter notebooks for EDA and Modeling
└── README.md                          # Project documentation
