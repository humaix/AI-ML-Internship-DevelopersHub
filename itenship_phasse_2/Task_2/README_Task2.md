# Task 2: End-to-End ML Pipeline with Scikit-learn

This project implements a robust **End-to-End Machine Learning Pipeline** to predict **Telco Customer Churn**. It leverages the Scikit-learn `Pipeline` API to streamline data preprocessing, feature engineering, and model training.

## 📌 Objective
To build a reproducible and production-ready machine learning pipeline that handles missing values, encodes categorical features, scales numerical data, and trains a Random Forest classifier.

## 📂 Dataset
**Source**: [Telco Customer Churn Dataset](https://github.com/IBM/telco-customer-churn-on-icp4d)

The dataset includes customer demographics, services, account information, and the target variable **`Churn`** (Whether the customer left or not).

## 🛠️ Tech Stack
-   **Python 3.8+**
-   **Pandas & NumPy**: For data manipulation and cleaning.
-   **Scikit-learn**:
    -   `Pipeline`: For chaining steps.
    -   `ColumnTransformer`: For applying different transformations to numeric/categorical columns.
    -   `StandardScaler` & `OneHotEncoder`: For feature scaling and encoding.
    -   `RandomForestClassifier`: The predictive model.
    -   `GridSearchCV`: For hyperparameter optimization.

## 🚀 How to Run

1.  **Install Dependencies**:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```

2.  **Run the Notebook**:
    Open `Task_2End-to-End ML Pipeline with Scikit-learn Pipeline API.ipynb`.

3.  **Pipeline Steps**:
    1.  **Data Loading**: Fetches CSV from a raw URL.
    2.  **Cleaning**: Handles non-numeric `TotalCharges` and fills missing values.
    3.  **Preprocessing**:
        -   **Numeric**: Standard Scaling.
        -   **Categorical**: One-Hot Encoding.
    4.  **Modeling**: Trains a Random Forest Classifier.
    5.  **Tuning**: Optimizes hyperparameters (`n_estimators`, `max_depth`) using Grid Search.
    6.  **Evaluation**: Reports Accuracy and other metrics.

## 🧠 Model Architecture
The entire workflow is encapsulated in a single `Pipeline` object:
```python
feature_preprocessor = ColumnTransformer(...)
pipeline = Pipeline([
    ('preprocessor', feature_preprocessor),
    ('classifier', RandomForestClassifier())
])
```
This ensures no data leakage and makes the model easy to deploy.

## 📊 Results
The notebook outputs the best hyperparameters found via Grid Search and evaluates the model's performance on the test set.
