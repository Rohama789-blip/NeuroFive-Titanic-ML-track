# NeuroFive Titanic Machine Learning Track

## Project Overview

This repository contains all Titanic Machine Learning tasks completed during the NeuroFive Solutions AI/ML Internship Program. The project demonstrates a complete machine learning workflow, including data exploration, preprocessing, visualization, classification, model evaluation, machine learning pipelines, and ensemble learning.

---

## Repository Structure

```
Titanic_EDA.ipynb
Titanic_Cleaning_Visualization.ipynb
Titanic_Classification_Model.ipynb
Titanic_Model_Evaluation.ipynb
Titanic_Pipeline_Model.ipynb
Titanic_Ensemble_Models.ipynb
README.md
```

---

# Task 1 – Exploratory Data Analysis (EDA)

## Objectives

- Load the Titanic dataset.
- Explore dataset structure.
- Check data types.
- Generate descriptive statistics.
- Identify missing values.
- Understand feature distributions.

## Analysis Performed

- Displayed the first few records.
- Examined dataset information.
- Generated summary statistics.
- Checked missing values.
- Identified numerical and categorical features.

## Outcome

The dataset contains missing values in the Age, Cabin, and Embarked columns, which require preprocessing before model training.

---

# Task 2 – Data Cleaning and Visualization

## Objectives

- Handle missing values.
- Remove unnecessary columns.
- Visualize the dataset.
- Detect outliers.

## Data Cleaning

- Filled missing Age values using the median.
- Filled missing Embarked values using the mode.
- Removed the Cabin column.
- Checked duplicate records.

## Visualizations

- Histogram
- Boxplot
- Count Plot
- Correlation Heatmap

## Outcome

The visualizations showed that passenger class, gender, and fare had a significant relationship with survival.

---

# Task 3 – Titanic Classification Model

## Model Used

- Logistic Regression

## Workflow

- Feature Selection
- Encoding Categorical Variables
- Train-Test Split
- Model Training
- Prediction

## Evaluation

- Accuracy Score
- Confusion Matrix

## Result

**Accuracy: 81.01%**

---

# Task 4 – Model Evaluation and Hyperparameter Tuning

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Hyperparameter Tuning

GridSearchCV was applied using different values of:

- C
- Solver

## Results

| Model | Accuracy |
|--------|----------|
| Original Logistic Regression | **81.01%** |
| Tuned Logistic Regression | **78.21%** |

## Outcome

The original Logistic Regression model performed better than the tuned model.

---

# Task 5 – Machine Learning Pipeline

## Pipeline Components

- ColumnTransformer
- SimpleImputer
- StandardScaler
- OneHotEncoder
- Logistic Regression

## Feature Engineering

Two new features were created:

- FamilySize
- IsAlone

## Result

**Pipeline Accuracy: 79%**

## Model Export

The trained pipeline was saved using Joblib.

**Saved File**

```
Titanic_Pipeline_Model.pkl
```

## Outcome

The pipeline automated preprocessing and model training, creating a reusable workflow while reducing the risk of data leakage.

---

# Task 6 – Ensemble Learning

## Models Implemented

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

## Model Comparison

| Model | Accuracy |
|--------|----------|
| Logistic Regression | **81.01%** |
| Random Forest | **82.12%** |
| XGBoost | **80.45%** |

## Feature Importance

The ensemble models identified the following as the most important features:

- Sex
- Fare
- Pclass
- Age
- Family Size

## Outcome

Random Forest achieved the highest accuracy among all tested models and was selected as the best-performing model for Titanic survival prediction.

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib

---

# Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# Overall Results

| Task | Result |
|------|--------|
| Exploratory Data Analysis | Completed |
| Data Cleaning & Visualization | Completed |
| Logistic Regression Model | 81.01% Accuracy |
| Model Evaluation | Completed |
| Hyperparameter Tuning | Completed |
| Machine Learning Pipeline | 79% Accuracy |
| Random Forest | 82.12% Accuracy |
| XGBoost | 80.45% Accuracy |

---

# Learning Outcomes

During this project, I learned how to:

- Perform Exploratory Data Analysis (EDA).
- Clean and preprocess real-world datasets.
- Create informative visualizations.
- Build classification models using Logistic Regression.
- Evaluate models using multiple performance metrics.
- Tune hyperparameters using GridSearchCV.
- Build reusable Scikit-learn Pipelines.
- Apply feature engineering techniques.
- Train and compare ensemble learning models.
- Select the best-performing model based on evaluation results.

---

# Author

**GitHub:** Rohama789-blip

**Internship:** NeuroFive Solutions AI/ML Internship

**Project:** Titanic Machine Learning Track
