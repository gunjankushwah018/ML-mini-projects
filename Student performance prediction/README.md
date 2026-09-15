# Student Performance Prediction

## 📌 Overview

This project predicts students' exam scores using Machine Learning.

The dataset contains different factors related to students, such as study hours, attendance, previous scores, parental involvement, motivation level, internet access, and other student-related information.

## 📊 Dataset

The dataset contains **6607 records and 20 columns**.

### Features include:

- Hours Studied
- Attendance
- Parental Involvement
- Access to Resources
- Extracurricular Activities
- Sleep Hours
- Previous Scores
- Motivation Level
- Internet Access
- Tutoring Sessions
- Family Income
- Teacher Quality
- School Type
- Peer Influence
- Physical Activity
- Learning Disabilities
- Parental Education Level
- Distance from Home
- Gender

### Target

- Exam Score

## 🔧 Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

## 🔄 Project Workflow

1. Load the dataset
2. Explore the dataset
3. Check data types and categorical values
4. Handle missing values
5. Encode categorical features
6. Define features (X) and target (y)
7. Split the data into training and testing sets
8. Train Machine Learning models
9. Evaluate model performance
10. Select the best-performing model

## 🧹 Data Preprocessing

Missing values were present in:

- Teacher Quality
- Parental Education Level
- Distance from Home

These missing values were filled using the mode.

Categorical features were converted into numerical values using:

- Ordinal Encoding
- Binary Encoding
- One-Hot Encoding

After preprocessing, there were no remaining object-type columns.

## ✂️ Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

`random_state = 42` was used.

## 🤖 Machine Learning Models

The following regression models were tested:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor

## 📈 Model Performance

| Model | MAE | MSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 0.446 | 3.241 | 0.771 |
| Random Forest Regressor | 1.073 | 4.656 | 0.671 |
| Gradient Boosting Regressor | 0.794 | 3.773 | 0.733 |

## 🏆 Best Model

Among the tested models, **Linear Regression** performed the best.

It achieved an **R² score of approximately 77.1%**, along with the lowest MAE and MSE among the three tested models.

## 📁 Files

- `Student_performance_prediction.ipynb` - Complete Jupyter Notebook
- `README.md` - Project documentation

## 🚀 Conclusion

In this project, we used student-related information to predict exam scores.

We compared Linear Regression, Random Forest Regressor, and Gradient Boosting Regressor.

Among these models, Linear Regression gave the best results with an R² score of approximately 77.1%.

Therefore, Linear Regression was selected as the best-performing model for this project.
