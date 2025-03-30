# Titanic Survival Prediction

This project focuses on predicting the survivability of Titanic passengers using machine learning techniques. The dataset is analyzed, preprocessed, and used to train a classification model.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Overview](#dataset-overview)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Key Observations](#key-observations)

## Project Overview
The goal of this project is to build a predictive model using logistic regression to determine the survival chances of passengers aboard the Titanic based on various features such as age, sex, ticket class, and more.

## Dataset Overview
The dataset is loaded from a CSV file named `titanic.csv`. It contains information about 891 passengers, structured across 12 columns. Some key statistics about the dataset include:

- **Total rows:** 891
- **Total columns:** 12
- **Missing values:** Some columns contain missing values, which are handled during preprocessing.

![Dataset Overview](https://github.com/user-attachments/assets/a640853e-635e-4d98-beee-d4f1cefdfc2c)

## Data Preprocessing
Before training the model, we perform the following data preprocessing steps:
1. **Dropping Irrelevant Columns:**
   - `PassengerId` and `Name` are removed as they do not contribute to the model’s predictive capabilities.
   - `Cabin` is dropped due to a high percentage of missing values.

   ![Dropped Columns](https://github.com/user-attachments/assets/576b6c76-9cde-43a6-8211-2ae7fd4ea613)

2. **Handling Missing Values:**
   - Missing values in columns such as `Age` are handled appropriately using imputation techniques.

3. **Feature Engineering:**
   - Categorical variables such as `Sex` and `Embarked` are encoded for compatibility with machine learning models.

## Model Training
The dataset is split into training (80%) and testing (20%) subsets. A logistic regression model from the **Scikit-learn** library is trained to classify passengers as survivors or non-survivors.

## Model Evaluation
To assess the model’s performance, we use the following evaluation metrics:
1. **Cross-validation:** Ensures model generalizability across different subsets of data.

   ![Cross-validation](https://github.com/user-attachments/assets/91a8a396-be3b-4405-b4d1-0a014cf24953)

2. **Confusion Matrix:** Provides insight into the model’s classification accuracy.

   ![Confusion Matrix](https://github.com/user-attachments/assets/7642e29c-f804-4ffb-bbdf-491a8c23372a)

3. **Classification Metrics:**
   - **Precision**
   - **Recall**
   - **Sensitivity**
   - **Specificity**

   ![Classification Metrics](https://github.com/user-attachments/assets/0fffcd5e-435e-4755-9913-27e686107f37)

## Key Observations
To understand the impact of gender on survival probability, we analyze the survival chances of two hypothetical passengers:
- **Female, 42 years old, First Class:** Higher survival probability.
- **Male, 42 years old, First Class:** Lower survival probability.

![Gender Survival Analysis](https://github.com/user-attachments/assets/27fe9db8-e940-4888-9fa3-80acdba1a598)

This analysis highlights the significant impact of gender on survival rates.

---
This project demonstrates a structured approach to data preprocessing, model training, and evaluation in predictive analytics using Python and Scikit-learn.

