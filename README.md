# Predicting Calories Burnt Using Machine Learning

This Jupyter notebook predicts calories burnt during physical activities using features such as age, gender, height, weight, exercise duration, heart rate, and body temperature. It covers data loading, preprocessing, model building, evaluation, and GUI creation.

## Notebook Highlights

### 1. Data Loading and Exploration
- **Data Loading**: Data from two CSV files are loaded and merged for comprehensive analysis.
- **Exploratory Data Analysis (EDA)**: Conducted using **Seaborn** and **Matplotlib**, including distribution plots for numerical features and count plots for categorical features.

### 2. Data Preprocessing
- **Handling Categorical and Numerical Features**:
  - Categorical variables like `Gender` are encoded using **OrdinalEncoder**.
  - Numerical variables such as `Age`, `Height`, `Weight`, etc., are standardized using **StandardScaler**.
- **ColumnTransformer**: Used to automate the preprocessing of both categorical and numerical features in a pipeline-friendly manner.
- Features like `User_ID` are dropped as they do not contribute to the prediction task.

### 3. Model Building
- Implements and compares several machine learning models:
  - **Linear Regression**
  - **Random Forest Regressor**
  - **XGBoost Regressor**
- Models are trained and evaluated using metrics such as **R² Score** and **Mean Absolute Error (MAE)**.

### 4. Cross-Validation & Model Comparison
- **K-Folds Cross-Validation**: Applied to assess model performance with multiple folds.
- **Best Model**: Identified through comparison of cross-validation scores, with **XGBoost** performing the best.

### 5. Machine Learning Pipeline
- A **Pipeline** is created to combine preprocessing and modeling steps, ensuring clean and efficient model training.
- The final trained model is saved using **pickle** for future predictions.

### 6. Graphical User Interface (GUI)
- A simple **Tkinter-based GUI** allows users to input new data and get predictions on calories burnt in real-time using the saved model.

## Features Included
- **Pandas**: Data manipulation and analysis.
- **Seaborn & Matplotlib**: Data visualization for exploratory analysis.
- **Scikit-learn & XGBoost**: Model training, evaluation, and cross-validation.
- **Tkinter**: GUI for real-time predictions.
