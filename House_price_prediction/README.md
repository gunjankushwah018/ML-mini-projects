# House Price Prediction

## 📌 Overview

This project predicts house prices using Machine Learning regression models.

The project includes data preprocessing, exploratory data analysis, feature transformation, model training, model evaluation, and feature importance analysis.

## 📊 Dataset

The dataset contains information about houses such as:

- Bedrooms
- Bathrooms
- Living area
- Lot area
- Floors
- Waterfront
- View
- Condition
- Grade
- Year built
- Year renovated
- Basement area
- Location-related features
- Price

## 🔧 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 🔄 Project Workflow

1. Load the dataset
2. Check the dataset shape and contents
3. Check duplicate records
4. Convert date into year and month
5. Perform Exploratory Data Analysis (EDA)
6. Analyze correlations between features and price
7. Check price distribution and skewness
8. Define features (X) and target (y)
9. Split the data into training and testing sets
10. Scale numerical features
11. Encode the zipcode feature
12. Train Machine Learning models
13. Evaluate model performance
14. Analyze feature importance
15. Predict the price of a new house

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Removed the `id` column
- Converted the `date` column into datetime format
- Extracted `year` and `month` from the date
- Removed the original `date` column
- Used `StandardScaler` for numerical features
- Used `OneHotEncoder` for the `zipcode` feature
- Used a `ColumnTransformer` to apply preprocessing

## ✂️ Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

`random_state = 42` was used.

## 🤖 Machine Learning Models

Two regression models were trained and compared:

1. Linear Regression
2. Random Forest Regressor

## 📈 Model Performance

| Model | MAE | MSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 98749.43 | 29210910577.81 | 0.807 |
| Random Forest | 72446.90 | 22243073248.61 | 0.853 |

## 🏆 Best Model

The **Random Forest Regressor** performed better than Linear Regression.

It achieved:

- **MAE:** 72,446.90
- **MSE:** 22,243,073,248.61
- **R² Score:** 0.853

Therefore, Random Forest was selected as the final model.

## ⭐ Feature Importance

Feature importance was analyzed using the Random Forest model.

Some of the most important features for predicting house prices were:

- Grade
- Sqft Living
- Latitude
- Longitude
- Year Built
- Waterfront
- Sqft Living15

## 📊 Visualization

The project includes visualizations such as:

- Price distribution
- Price boxplot
- Sqft Living vs Price
- Correlation heatmap
- Actual vs Predicted house prices

## 🏠 New House Prediction

The trained Random Forest model was also used to predict the price of a new house using its features such as:

- Bedrooms
- Bathrooms
- Sqft Living
- Lot Area
- Floors
- Grade
- Location
- Year Built
- And other house-related features

## 📁 Files

- `House_price_prediction.ipynb` - Complete Jupyter Notebook
- `README.md` - Project documentation

## 🚀 Conclusion

In this project, Linear Regression and Random Forest were used to predict house prices.

Random Forest performed better than Linear Regression based on MAE, MSE, and R² score.

The Random Forest model achieved an R² score of approximately **0.853**, making it the better-performing model for this dataset.
