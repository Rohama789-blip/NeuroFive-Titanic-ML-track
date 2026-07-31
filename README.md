# Titanic Machine Learning Project – NeuroFive ML Internship

## Project Overview

This repository contains all Titanic-based tasks completed as part of the **NeuroFive Machine Learning Internship**. The project follows a complete machine learning workflow, starting from data exploration and preprocessing to model building, evaluation, and deployment using a Scikit-learn Pipeline.

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

# Task 1: Exploratory Data Analysis (EDA)

### Objectives

- Load the Titanic dataset
- Explore the dataset structure
- Display the first five rows
- Analyze dataset information
- Generate descriptive statistics
- Identify numerical and categorical features
- Detect missing values
- Summarize key insights

### Key Findings

- The dataset contains both numerical and categorical features.
- Missing values were found in the **Age**, **Cabin**, and **Embarked** columns.
- The dataset is suitable for machine learning after preprocessing.

---

# Task 2: Data Cleaning & Visualization

### Data Cleaning

- Filled missing values in **Age** using the median.
- Filled missing values in **Embarked** using the mode.
- Removed the **Cabin** column because of excessive missing values.

### Visualizations

- Histogram
- Boxplot
- Survival Count Bar Chart
- Correlation Heatmap

### Observation

The analysis showed that **Gender (Sex)** and **Passenger Class (Pclass)** strongly influence survival.

---

# Task 3: Titanic Survival Prediction

### Machine Learning Workflow

- Data preprocessing
- Handling missing values
- Encoding categorical variables
- Train/Test Split
- Logistic Regression model
- Prediction
- Model evaluation

### Model Performance

- **Algorithm:** Logistic Regression
- **Accuracy:** **81.01%**

### Conclusion

The Logistic Regression model successfully predicted passenger survival with an accuracy of approximately **81%**.

---

# Task 4: Model Evaluation & Hyperparameter Tuning

### Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Hyperparameter Tuning

GridSearchCV was applied using different values of:

- C
- Solver

### Results

| Model | Accuracy |
|--------|----------|
| Original Logistic Regression | **81.01%** |
| Tuned Logistic Regression | **78.21%** |

### Conclusion

The tuned model achieved slightly lower accuracy than the original model. This demonstrates that hyperparameter tuning does not always improve performance and that models should always be evaluated on unseen test data.

---

# Task 5: Feature Engineering & Machine Learning Pipeline

### Feature Engineering

Two new features were created:

- FamilySize
- IsAlone

### Pipeline Components

- SimpleImputer
- StandardScaler
- OneHotEncoder
- ColumnTransformer
- Logistic Regression

### Model Performance

- **Pipeline Accuracy:** **79%**

### Model Export

The trained pipeline was saved using **Joblib**.

File:

```
Titanic_Pipeline_Model.pkl
```

### Conclusion

Using a Scikit-learn Pipeline automates preprocessing and model training, making the workflow reusable, consistent, and less prone to data leakage.

---

# Repository Contents

```
Titanic_EDA.ipynb
Titanic_Cleaning_Visualization.ipynb
Titanic_Classification_Model.ipynb
Titanic_Model_Evaluation.ipynb
Titanic_Pipeline_Model.ipynb
Titanic_Pipeline_Model.pkl
README.md
```

---

# Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Data Visualization
- Feature Engineering
- Logistic Regression
- Model Evaluation
- Hyperparameter Tuning
- Scikit-learn Pipeline
- Feature Encoding
- Model Serialization using Joblib

---

# Final Project Summary

This repository demonstrates a complete end-to-end Machine Learning workflow using the Titanic dataset. It covers data exploration, preprocessing, visualization, feature engineering, model development, evaluation, hyperparameter tuning, and pipeline creation. The project follows industry-standard practices using Scikit-learn and provides a reusable machine learning solution for predicting Titanic passenger survival.

---

## Author

**NeuroFive Machine Learning Internship Project**

Developed using **Python**, **Google Colab**, and **Scikit-learn**.
