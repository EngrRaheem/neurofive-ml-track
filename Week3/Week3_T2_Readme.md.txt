# Week 3 – Task 2: Customer Churn Prediction Using Decision Tree and Logistic Regression

## 📖 Introduction

This project is the second task of **Week 3** in the **Neurofive Machine Learning Fundamentals Track**. The objective is to solve a real-world business problem by predicting customer churn using Machine Learning.

Customer churn prediction is widely used in industries such as telecommunications, banking, insurance, and SaaS, where retaining existing customers is often more cost-effective than acquiring new ones. In this project, two classification models—**Decision Tree Classifier** and **Logistic Regression**—were developed and compared to identify customers who are likely to leave a company's service.

The project also includes Exploratory Data Analysis (EDA), data preprocessing, feature importance analysis, and a business-oriented interpretation of the results.

---

# 🎯 Objectives

The objectives of this project are to:

- Load and explore the Telco Customer Churn dataset.
- Perform quick Exploratory Data Analysis (EDA).
- Handle missing values and categorical variables.
- Identify any class imbalance in the dataset.
- Train a Decision Tree Classifier.
- Train a Logistic Regression model.
- Compare both models using evaluation metrics.
- Identify the top features influencing customer churn.
- Provide business insights based on the analysis.

---

# 📂 Folder Contents

| File | Description |
|------|-------------|
| Week3_Task2_Customer_Churn_Prediction.ipynb | Complete Jupyter Notebook |
| Week3_Task2_Customer_Churn_Prediction.pdf | PDF version of the notebook |
| README.md | Documentation for Week 3 Task 2 |
| Telco-Customer-Churn.csv | Customer Churn dataset |

---

# 🛠 Software Used

- Python 3
- Jupyter Notebook

---

# 📚 Python Libraries Used

The following libraries were used throughout this project:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📊 Dataset Information

### Dataset Name

Telco Customer Churn Dataset

### Dataset Source

Kaggle

### Problem Type

Binary Classification

### Target Variable

**Churn**

- Yes → Customer Left the Service
- No → Customer Stayed with the Service

---

# 📋 Dataset Features

The dataset contains customer information including:

- Customer demographics
- Account information
- Contract type
- Internet service
- Payment method
- Monthly charges
- Total charges
- Customer tenure
- Churn status

Each row represents one customer.

---

# 🔄 Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Checked dataset structure and summary statistics.
- Identified missing values.
- Converted non-numeric columns into numerical format using Label Encoding.
- Converted numerical columns where necessary.
- Prepared the dataset for Machine Learning models.

---

# 📈 Exploratory Data Analysis (EDA)

Several visualizations were created to understand customer behavior and identify factors related to churn.

Visualizations include:

- Customer Tenure Histogram
- Monthly Charges Boxplot
- Contract Type Bar Chart
- Correlation Heatmap

These visualizations helped identify important relationships between customer characteristics and churn.

---

# ⚠ Class Imbalance

The target variable (Churn) was examined to determine whether the dataset is balanced.

Although the dataset may contain more customers who stayed than those who left, this imbalance was identified and discussed as part of the analysis. Future improvements could include techniques such as:

- SMOTE (Synthetic Minority Over-sampling Technique)
- Random Oversampling
- Class Weight Adjustment

---

# 🤖 Machine Learning Models

Two supervised classification algorithms were implemented.

## Decision Tree Classifier

Decision Trees classify customers by learning a series of decision rules from historical customer data.

Advantages include:

- Easy to interpret
- Visual decision-making process
- Provides feature importance scores

---

## Logistic Regression

Logistic Regression predicts the probability that a customer will churn.

Advantages include:

- Simple and efficient
- Fast training
- Strong baseline classifier
- Easy to interpret probabilities

---

# 📊 Model Evaluation

Both models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

These evaluation metrics provide a comprehensive understanding of model performance beyond accuracy alone.

---

# 📈 Model Comparison

The notebook compares the performance of:

- Decision Tree Classifier
- Logistic Regression

The comparison helps determine which model provides better predictive performance for customer churn.

---

# ⭐ Feature Importance

One major advantage of Decision Trees is the ability to measure feature importance.

Using the `.feature_importances_` attribute, the most influential features contributing to customer churn were identified.

The notebook displays the **Top 3 Most Important Features** as well as a feature importance visualization.

---

# 💼 Business Summary

The analysis indicates that customer churn is primarily influenced by factors such as customer tenure, contract type, and monthly charges.

Customers with shorter service durations and less favorable contract plans are generally more likely to discontinue their services. These insights allow organizations to proactively identify high-risk customers and implement targeted retention strategies, such as personalized offers, loyalty programs, or contract upgrades.

By applying Machine Learning to customer behavior data, businesses can improve customer satisfaction, reduce churn, and increase long-term revenue.

---

# 📖 Learning Outcomes

After completing this project, I learned how to:

- Solve a real-world business classification problem.
- Perform Exploratory Data Analysis on customer data.
- Handle categorical variables.
- Detect and discuss class imbalance.
- Train multiple Machine Learning models.
- Compare classification algorithms.
- Interpret feature importance.
- Translate Machine Learning results into business insights.

---

# 📁 Project Structure

```
Week3/
│
├── README.md
├── Week3_Task1_Model_Evaluation_Tuning.ipynb
├── Week3_Task1_Model_Evaluation_Tuning.pdf
├── Week3_Task2_Customer_Churn_Prediction.ipynb
├── Week3_Task2_Customer_Churn_Prediction.pdf
└── Telco-Customer-Churn.csv
```

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/neurofive-ml-track.git
```

---

## 2. Navigate to the Week 3 Folder

```bash
cd neurofive-ml-track/Week3
```

---

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 4. Launch Jupyter Notebook

```bash
python -m notebook
```

Open:

```
Week3_Task2_Customer_Churn_Prediction.ipynb
```

Run all notebook cells sequentially to reproduce the complete analysis.

---

# 🎓 Course Information

**Course:** Machine Learning Fundamentals

**Organization:** Neurofive Solutions

---

# 📌 Assignment Status

✅ Completed

---

# 👨‍💻 Author

**Abdul Raheem**

Electrical Engineering Student

Government College University Faisalabad (GCUF)

Machine Learning Fundamentals Track – Neurofive Solutions

---

# ⭐ Repository

This project is part of my **Machine Learning Fundamentals** learning journey. It demonstrates how Machine Learning can be applied to solve real-world business problems by predicting customer churn using multiple classification algorithms.

The project emphasizes data preprocessing, exploratory data analysis, model comparison, feature importance analysis, and business-oriented interpretation, providing practical experience in developing predictive analytics solutions for customer retention.