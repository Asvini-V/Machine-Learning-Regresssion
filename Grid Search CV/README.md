This file contains regression models built using GridSearchCV to predict insurance charges. The goal is to understand hyperparameter tuning and model comparison using cross-validation.

Algorithms Used

Support Vector Regression (SVR)

Decision Tree Regression

Random Forest Regression

📁 Code Explanation

For each algorithm, two versions of code are provided for learning and comparison:

🔹 Version 1: Manual Split + GridSearchCV

Uses train_test_split

Applies StandardScaler where required (SVR)

Evaluates performance using R² score on test data

Represents the traditional machine learning workflow

🔹 Version 2: GridSearchCV with Cross-Validation

No manual train-test split

GridSearchCV internally handles data splitting using cross-validation

Entire dataset is used for training and validation

Focuses purely on hyperparameter tuning
