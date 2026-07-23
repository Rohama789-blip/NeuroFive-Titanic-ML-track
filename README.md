#  Titanic Survival Analysis

## Project Overview

This project was completed as part of the NeuroFive ML Internship. It demonstrates the complete machine learning workflow using the Titanic dataset, starting from Exploratory Data Analysis (EDA) to Data Cleaning, Visualization, and finally building a Classification Model using Logistic Regression.

---

## Tools & Libraries Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Task 1: Exploratory Data Analysis (EDA)

### Objectives
- Load the Titanic dataset
- Explore the dataset structure
- Display the first five rows
- Check dataset information
- Generate descriptive statistics
- Identify numerical and categorical columns
- Detect missing values
- Summarize key findings

### Findings
- The dataset contains both numerical and categorical features.
- Missing values were found in the Age, Cabin, and Embarked columns.
- The dataset is suitable for machine learning after preprocessing.

---

# Task 2: Data Cleaning & Visualization

### Data Cleaning
- Filled missing values in the Age column using the median.
- Filled missing values in the Embarked column using the mode.
- Removed the Cabin column because it contained a large number of missing values.

### Visualizations Created
- Histogram
- Boxplot (Outlier Detection)
- Survival Bar Chart
- Correlation Heatmap

### Observation
The visualizations indicate that passenger gender and passenger class have a significant impact on survival.

---

# Task 3: Titanic Survival Prediction

### Machine Learning Steps
- Prepared the cleaned dataset
- Encoded categorical variables using `pd.get_dummies()`
- Split the dataset into training and testing sets
- Trained a Logistic Regression model
- Predicted passenger survival
- Evaluated the model using Accuracy Score
- Generated a Confusion Matrix

---

## Task 5: Model Evaluation & Hyperparameter Tuning

### Evaluation Metrics

The Logistic Regression model was evaluated using multiple classification metrics instead of relying only on accuracy.

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Hyperparameter Tuning

GridSearchCV was used to tune the Logistic Regression model using different values of **C** and **solver**.

### Results

| Model | Accuracy |
|--------|----------|
| Original Logistic Regression | **81.00%** |
| Tuned Logistic Regression | **78.21%** |

### Conclusion

The original Logistic Regression model achieved better accuracy than the tuned model. This demonstrates that hyperparameter tuning does not always improve model performance, and the best model should be selected based on evaluation results rather than assumptions.

### Model Performance

**Algorithm:** Logistic Regression

**Accuracy:** **81%**

### Conclusion

The Logistic Regression model achieved an accuracy of **81%**, demonstrating good performance for a baseline classification model. The analysis suggests that passenger gender and passenger class were among the most influential factors affecting survival.

---

## Repository Contents

- Titanic_EDA.ipynb
- Titanic_Cleaning_Visualization.ipynb
- Titanic_Classification_Model.ipynb
- README.md

---

## Author

Completed as part of the **NeuroFive ML Internship Program** using **Google Colab** and **Python**.
