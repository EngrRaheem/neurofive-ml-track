# Week 4 – Task 1: Building a Machine Learning Pipeline with Feature Engineering

##  Introduction

This project is the first task of **Week 4** in the **Neurofive Machine Learning Fundamentals Track**. The objective is to build a professional Machine Learning pipeline using Scikit-learn that combines data preprocessing, feature engineering, and model training into a single reusable workflow.

Instead of manually performing preprocessing before model training, Scikit-learn Pipelines automate the entire workflow. This ensures consistent preprocessing, prevents data leakage between training and testing datasets, and makes the model easier to deploy in real-world applications.

The Titanic dataset from previous tasks was reused to demonstrate how a production-style Machine Learning pipeline can simplify the entire modeling process.

---

#  Objectives

The objectives of this project are to:

- Reuse the Titanic dataset from previous tasks.
- Create new engineered features.
- Separate numerical and categorical variables.
- Build preprocessing pipelines for different feature types.
- Apply StandardScaler to numerical features.
- Apply OneHotEncoder to categorical features.
- Combine preprocessing and model training using a Pipeline.
- Evaluate the pipeline's performance.
- Save the trained pipeline using Joblib for future use.

---

#  Folder Contents

| File | Description |
|------|-------------|
| Week4_Task1_ML_Pipeline.ipynb | Complete Jupyter Notebook |
| Week4_Task1_ML_Pipeline.pdf | PDF version of the notebook |
| README.md | Documentation for Week 4 Task 1 |
| train.csv | Titanic dataset |
| titanic_pipeline.pkl | Saved Machine Learning pipeline |

---

#  Software Used

- Python 3
- Jupyter Notebook

---

#  Python Libraries Used

The following libraries were used throughout this project:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

#  Dataset Information

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

#  Feature Engineering

To improve the predictive capability of the model, two additional features were created.

### 1. FamilySize

This feature represents the total number of family members traveling with each passenger.

```
FamilySize = SibSp + Parch + 1
```

It combines siblings/spouses, parents/children, and the passenger.

---

### 2. IsAlone

This feature indicates whether a passenger was traveling alone.

- 1 → Passenger traveled alone
- 0 → Passenger traveled with family

These engineered features provide additional information that may improve model performance.

---

#  Data Preprocessing

Instead of manually preprocessing the dataset, a professional preprocessing pipeline was developed.

The preprocessing workflow includes:

- Missing value imputation
- Feature scaling
- Categorical encoding
- Automatic preprocessing during training and prediction

This approach ensures consistent data preparation throughout the Machine Learning workflow.

---

#  ColumnTransformer

A **ColumnTransformer** was used to apply different preprocessing techniques to different types of features.

### Numerical Features

The following transformations were applied:

- Median value imputation
- StandardScaler

Features:

- Age
- Fare
- FamilySize
- IsAlone

---

### Categorical Features

The following transformations were applied:

- Most frequent value imputation
- OneHotEncoder

Features:

- Pclass
- Sex
- Embarked

---

#  Machine Learning Pipeline

The preprocessing steps and Logistic Regression model were combined into a single Scikit-learn Pipeline.

The pipeline automatically performs:

1. Missing value handling
2. Feature scaling
3. Categorical encoding
4. Model training
5. Prediction

This eliminates repetitive preprocessing code and significantly reduces the possibility of data leakage.

---

#  Machine Learning Model

## Algorithm Used

**Logistic Regression**

Logistic Regression was selected because it is:

- Fast
- Interpretable
- Efficient for binary classification
- Suitable for the Titanic survival prediction problem

---

#  Model Evaluation

The trained pipeline was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

The pipeline produced performance comparable to or better than the manual preprocessing approach used in previous tasks while providing a much cleaner implementation.

---

#  Saving the Pipeline

The final trained pipeline was saved using **Joblib**.

Saved file:

```
titanic_pipeline.pkl
```

Saving the pipeline allows the trained model and preprocessing steps to be reused later without retraining.

This is a common practice in production Machine Learning systems.

---

#  Why Machine Learning Pipelines Matter

Machine Learning pipelines provide several important advantages:

- Prevent data leakage.
- Ensure identical preprocessing during training and prediction.
- Simplify model deployment.
- Reduce repetitive code.
- Improve reproducibility.
- Make projects easier to maintain.

For these reasons, pipelines are widely used in professional Machine Learning projects.

---

#  Learning Outcomes

After completing this project, I learned how to:

- Build reusable Machine Learning pipelines.
- Apply different preprocessing techniques using ColumnTransformer.
- Engineer new features to improve prediction.
- Combine preprocessing and modeling into a single workflow.
- Save trained pipelines using Joblib.
- Develop cleaner, more maintainable Machine Learning code.

---

#  Project Structure

```
Week4/
│
├── README.md
├── Week4_Task1_ML_Pipeline.ipynb
├── Week4_Task1_ML_Pipeline.pdf
├── train.csv
└── titanic_pipeline.pkl
```

---

#  How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/neurofive-ml-track.git
```

---

## 2. Navigate to the Week 4 Folder

```bash
cd neurofive-ml-track/Week4
```

---

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

---

## 4. Launch Jupyter Notebook

```bash
python -m notebook
```

Open:

```
Week4_Task1_ML_Pipeline.ipynb
```

Run all notebook cells sequentially to reproduce the complete workflow.

---

#  Course Information

**Course:** Machine Learning Fundamentals

**Organization:** Neurofive Solutions

---

#  Assignment Status

 Completed

---

#  Author

**Abdul Raheem**

Electrical Engineering Student

Government College University Faisalabad (GCUF)

Machine Learning Fundamentals Track – Neurofive Solutions

---

#  Repository

This project is part of my **Machine Learning Fundamentals** learning journey. It demonstrates how to build production-ready Machine Learning workflows using Scikit-learn Pipelines and ColumnTransformers.

The project combines feature engineering, preprocessing, model training, evaluation, and model persistence into a single reusable pipeline, reflecting industry best practices for developing reliable and maintainable Machine Learning solutions.