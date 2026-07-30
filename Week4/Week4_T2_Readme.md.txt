# Week 4 – Task 2: Ensemble Learning – Random Forest vs XGBoost

## Introduction

This project is the second task of **Week 4** in the **Neurofive Machine Learning Fundamentals Track**. The objective is to explore ensemble learning techniques by comparing the performance of **Random Forest** and **XGBoost** with a baseline **Logistic Regression** model on the Titanic dataset.

Ensemble learning combines multiple models to improve prediction accuracy, reduce overfitting, and increase model robustness. In this project, the Titanic dataset was used to train three different classification models, evaluate their performance, analyze feature importance, and understand the differences between bagging and boosting techniques.

---

# Objectives

The objectives of this project are to:

- Reuse the Titanic dataset from previous tasks.
- Preprocess the dataset for machine learning.
- Train a Logistic Regression model as the baseline.
- Train a Random Forest Classifier.
- Train an XGBoost Classifier.
- Compare the performance of all three models.
- Visualize feature importance for Random Forest and XGBoost.
- Explain the differences between Random Forest and XGBoost.

---

# Folder Contents

| File | Description |
|------|-------------|
| Week4_Task2_Ensemble_Learning.ipynb | Complete Jupyter Notebook |
| Week4_Task2_Ensemble_Learning.pdf | PDF version of the notebook |
| README.md | Documentation for Week 4 Task 2 |
| train.csv | Titanic dataset |

---

# Software Used

- Python 3
- Jupyter Notebook

---

# Python Libraries Used

The following libraries were used in this project:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

# Dataset Information

### Dataset Name

Titanic – Machine Learning from Disaster

### Dataset Source

Kaggle

### Problem Type

Binary Classification

### Target Variable

**Survived**

- 1 → Passenger Survived
- 0 → Passenger Did Not Survive

---

# Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Checked dataset information and missing values.
- Filled missing values in the Age column using the median.
- Filled missing values in the Embarked column using the most frequent value.
- Removed unnecessary columns:
  - PassengerId
  - Name
  - Ticket
  - Cabin
- Encoded categorical variables using LabelEncoder.
- Split the dataset into training and testing sets.

---

# Machine Learning Models

Three classification models were implemented and compared.

## Logistic Regression

Logistic Regression was used as the baseline model because it is simple, fast, and widely used for binary classification problems.

---

## Random Forest Classifier

Random Forest is an ensemble learning algorithm that constructs multiple decision trees using random subsets of the training data. The final prediction is obtained through majority voting among all trees, making the model more robust and less prone to overfitting.

---

## XGBoost Classifier

XGBoost is an advanced gradient boosting algorithm that builds trees sequentially. Each new tree focuses on correcting the mistakes made by previous trees, resulting in improved predictive performance and better handling of complex datasets.

---

# Model Evaluation

Each model was evaluated using:

- Accuracy Score
- Classification Report
- Precision
- Recall
- F1-Score
- Confusion Matrix

The evaluation metrics were compared to determine which model achieved the best performance on the Titanic dataset.

---

# Feature Importance Analysis

Feature importance was analyzed for both ensemble models.

## Random Forest

Feature importance values were extracted using:

```
feature_importances_
```

A bar chart was created to visualize the contribution of each feature.

---

## XGBoost

Feature importance values were also extracted using:

```
feature_importances_
```

The resulting visualization highlights the features that contributed most to the model's predictions.

---

# Model Comparison

The performance of the three models was summarized in a comparison table containing:

- Model Name
- Accuracy Score

This comparison provides an overview of how ensemble methods perform relative to a traditional machine learning model.

---

# Random Forest vs XGBoost

Random Forest builds many independent decision trees in parallel using different subsets of the training data and combines their predictions through majority voting. This bagging approach reduces variance and improves model stability.

XGBoost builds trees sequentially, where each new tree learns from the errors of previous trees. This boosting strategy often achieves higher predictive accuracy by minimizing residual errors during training.

While both are powerful ensemble algorithms, XGBoost generally provides better predictive performance but requires more computational resources and careful parameter tuning.

---

# Learning Outcomes

After completing this project, I learned how to:

- Apply ensemble learning techniques to a classification problem.
- Train and evaluate Random Forest and XGBoost models.
- Compare multiple machine learning algorithms.
- Interpret feature importance generated by ensemble models.
- Understand the differences between bagging and boosting.
- Select appropriate models based on predictive performance.

---

# Project Structure

```
Week4/
│
├── README.md
├── Week4_Task1_ML_Pipeline.ipynb
├── Week4_Task1_ML_Pipeline.pdf
├── Week4_Task2_Ensemble_Learning.ipynb
├── Week4_Task2_Ensemble_Learning.pdf
└── train.csv
```

---

# How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/neurofive-ml-track.git
```

## 2. Navigate to the Week 4 Folder

```bash
cd neurofive-ml-track/Week4
```

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

## 4. Launch Jupyter Notebook

```bash
python -m notebook
```

Open:

```
Week4_Task2_Ensemble_Learning.ipynb
```

Run all notebook cells sequentially to reproduce the complete analysis.

---

# Course Information

**Course:** Machine Learning Fundamentals

**Organization:** Neurofive Solutions

---

# Assignment Status

Completed

---

# Author

**Abdul Raheem**

Electrical Engineering Student

Government College University Faisalabad (GCUF)

Machine Learning Fundamentals Track – Neurofive Solutions

---

# Repository

This project is part of my Machine Learning Fundamentals learning journey. It demonstrates the application of ensemble learning techniques by comparing Logistic Regression, Random Forest, and XGBoost on the Titanic dataset.

The project includes data preprocessing, model training, performance evaluation, feature importance analysis, and model comparison, providing practical experience with industry-standard ensemble learning methods.