# Week 4 – Task 3: Handling Imbalanced and Messy Real-World Data

## Introduction

This project is the third task of Week 4 in the Machine Learning Fundamentals track offered by Neurofive Solutions. The objective is to understand the challenges of working with highly imbalanced datasets and apply appropriate techniques to improve machine learning model performance.

The Credit Card Fraud Detection dataset was used to identify fraudulent financial transactions. Since fraudulent transactions represent only a very small percentage of the data, this project demonstrates why relying solely on accuracy can be misleading and highlights the importance of Precision, Recall, and F1-score when evaluating classification models.

A Logistic Regression model was trained before and after applying SMOTE (Synthetic Minority Over-sampling Technique), and the results were compared.

---

# Objectives

The objectives of this project are to:

- Analyze the Credit Card Fraud Detection dataset.
- Examine the distribution of fraud and non-fraud transactions.
- Visualize class imbalance using a bar chart.
- Train a Logistic Regression model on the original dataset.
- Apply SMOTE to balance the training data.
- Retrain the model using the balanced dataset.
- Compare model performance before and after balancing.
- Explain why accuracy is not an appropriate metric for highly imbalanced datasets.

---

# Folder Contents

| File | Description |
|------|-------------|
| Week4_Task3_Handling_Imbalanced_Data.ipynb | Complete Jupyter Notebook |
| Week4_Task3_Handling_Imbalanced_Data.pdf | PDF version of the notebook |
| README.md | Project documentation |
| creditcard.csv | Credit Card Fraud Detection dataset |

---

# Software Used

- Python 3
- Jupyter Notebook

---

# Python Libraries Used

The following libraries were used:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

# Dataset Information

Dataset Name

Credit Card Fraud Detection

Dataset Source

Kaggle

Problem Type

Binary Classification

Target Variable

Class

- 0 → Legitimate Transaction
- 1 → Fraudulent Transaction

The dataset contains anonymized features generated using Principal Component Analysis (PCA), along with transaction time, transaction amount, and the target class.

---

# Data Exploration

The dataset was inspected to understand:

- Dataset dimensions
- Data types
- Missing values
- Class distribution

The class distribution revealed a significant imbalance, with fraudulent transactions representing only a very small percentage of the total observations.

---

# Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Verified that no missing values were present.
- Selected the target variable.
- Split the dataset into training and testing sets using stratified sampling.

Since the dataset contains only numerical features, no categorical encoding was required.

---

# Class Imbalance Analysis

The class distribution was visualized using a bar chart.

The visualization clearly shows that legitimate transactions heavily outnumber fraudulent transactions. Such imbalance can bias machine learning models toward predicting the majority class.

---

# Machine Learning Model

Algorithm Used

Logistic Regression

A Logistic Regression classifier was trained using the original imbalanced dataset to establish a baseline for comparison.

---

# Handling Class Imbalance

SMOTE (Synthetic Minority Over-sampling Technique) was applied to the training dataset.

SMOTE generates synthetic samples for the minority class rather than duplicating existing records, allowing the model to learn a more balanced decision boundary.

After applying SMOTE, the Logistic Regression model was retrained using the balanced dataset.

---

# Model Evaluation

Both models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

The evaluation demonstrates that balancing the dataset improves the model's ability to correctly identify fraudulent transactions.

---

# Performance Comparison

The notebook includes a comparison table showing the performance of:

| Model | Evaluation |
|-------|------------|
| Logistic Regression (Original Dataset) | Before SMOTE |
| Logistic Regression (Balanced Dataset) | After SMOTE |

The comparison focuses on Precision, Recall, and F1-score rather than accuracy alone.

---

# Why Accuracy is Misleading

Accuracy is not a reliable evaluation metric for highly imbalanced datasets.

Since fraudulent transactions account for only a tiny fraction of all observations, a model that predicts every transaction as legitimate could still achieve an accuracy greater than 99%, while failing to detect any fraudulent activity.

Precision, Recall, and F1-score provide a much better assessment because they evaluate how effectively the model identifies the minority class.

---

# Learning Outcomes

After completing this project, I learned how to:

- Identify class imbalance in real-world datasets.
- Visualize class distribution.
- Apply SMOTE for oversampling.
- Train classification models on balanced data.
- Compare model performance before and after balancing.
- Understand why multiple evaluation metrics are necessary for imbalanced classification problems.

---

# Project Structure

```
Week4/
│
├── README.md
├── Week4_Task3_Handling_Imbalanced_Data.ipynb
├── Week4_Task3_Handling_Imbalanced_Data.pdf
└── creditcard.csv
```

---

# How to Run the Project

## Clone the Repository

```bash
git clone https://github.com/your-username/neurofive-ml-track.git
```

## Navigate to the Project Folder

```bash
cd neurofive-ml-track/Week4
```

## Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

## Launch Jupyter Notebook

```bash
python -m notebook
```

Open:

```
Week4_Task3_Handling_Imbalanced_Data.ipynb
```

Run all notebook cells sequentially.

---

# Course Information

Course: Machine Learning Fundamentals

Organization: Neurofive Solutions

---

# Assignment Status

Completed

---

# Author

Abdul Raheem

Electrical Engineering Student

Government College University Faisalabad (GCUF)

Machine Learning Fundamentals Track – Neurofive Solutions

---

# Repository

This project is part of my Machine Learning Fundamentals learning journey. It demonstrates practical techniques for handling imbalanced datasets using SMOTE and evaluating classification models with appropriate performance metrics. The project highlights the importance of balancing data to improve fraud detection and illustrates why evaluation metrics such as Precision, Recall, and F1-score are more informative than accuracy when working with highly skewed datasets.