# Week 2 – Predict Titanic Survival Using Logistic Regression

## 📖 Introduction

In Week 2 of the **Neurofive Machine Learning Fundamentals Track**, the focus shifts from understanding and preparing data to building the first Machine Learning model.

Using the cleaned Titanic dataset from Week 1, a **Logistic Regression** classifier was developed to predict whether a passenger survived the Titanic disaster. Since the target variable (**Survived**) contains only two possible outcomes (0 = Did Not Survive, 1 = Survived), this problem is a **Binary Classification** task.

The workflow includes data preprocessing, categorical feature encoding, dataset splitting, model training, prediction, and performance evaluation using standard classification metrics.

---

# 🎯 Objectives

The objectives of this task are to:

- Load the cleaned Titanic dataset
- Handle any remaining missing values
- Encode categorical variables into numerical format
- Select appropriate input features and target variable
- Split the dataset into training and testing sets
- Train a Logistic Regression classifier
- Predict passenger survival
- Evaluate model performance using accuracy
- Generate and interpret a confusion matrix
- Document the complete Machine Learning workflow

---

# 📂 Folder Contents

| File | Description |
|------|-------------|
| Week2_Logistic_Regression.ipynb | Complete Jupyter Notebook containing the classification model |
| Week2_Logistic_Regression.pdf | PDF version of the notebook |
| README.md | Documentation for Week 2 |
| train.csv | Titanic dataset used for training and testing |

---

# 🛠 Software Used

- Python 3
- Jupyter Notebook

---

# 📚 Python Libraries

The following libraries were used throughout this project:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📊 Dataset Information

**Dataset Name**

Titanic – Machine Learning from Disaster

**Source**

Kaggle Competition Dataset

**Dataset Characteristics**

- Total Records: 891
- Total Features: 12
- Target Variable: Survived

---

# 🔄 Data Preprocessing

Before training the Machine Learning model, several preprocessing steps were performed:

- Loaded the dataset using Pandas
- Checked dataset information
- Filled missing values in:
  - Age using the median
  - Embarked using the mode
  - Cabin using "Unknown"
- Converted categorical variables into numerical values using One-Hot Encoding
- Removed unnecessary columns that do not contribute significantly to prediction

---

# 🤖 Machine Learning Model

## Algorithm Used

**Logistic Regression**

Logistic Regression is a supervised Machine Learning algorithm designed for binary classification problems. It estimates the probability that an observation belongs to one of two possible classes.

For this project, the model predicts whether a passenger:

- Survived (1)
- Did Not Survive (0)

---

# 📌 Feature Selection

### Target Variable

```
Survived
```

### Predictor Features

The model uses passenger-related information such as:

- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

Columns including PassengerId, Name, Ticket, and Cabin were excluded from training.

---

# ✨ Feature Encoding

Machine Learning algorithms require numerical input.

Categorical variables were converted into numerical features using:

- Pandas `get_dummies()`
- One-Hot Encoding
- `drop_first=True` to avoid multicollinearity

Encoded features include:

- Sex
- Embarked

---

# ✂ Train-Test Split

The dataset was divided into two subsets:

- Training Set: 80%
- Testing Set: 20%

The split was performed using:

```
train_test_split()
```

A fixed random state was used to ensure reproducibility.

---

# 📈 Model Evaluation

The trained model was evaluated using:

- Accuracy Score
- Confusion Matrix

These metrics help determine how well the model predicts passenger survival on previously unseen data.

---

# 📊 Confusion Matrix

The confusion matrix compares predicted outcomes with actual outcomes.

It provides four important values:

- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

These values help identify where the model makes correct and incorrect predictions.

---

# 📌 Results

The notebook includes:

- Data preprocessing
- Feature encoding
- Logistic Regression training
- Prediction
- Accuracy calculation
- Confusion Matrix visualization
- Interpretation of model performance

---

# 📖 Learning Outcomes

After completing this task, I learned how to:

- Build a Binary Classification model
- Use Logistic Regression
- Split datasets into training and testing subsets
- Encode categorical variables
- Train Machine Learning models using Scikit-learn
- Evaluate model performance
- Interpret a Confusion Matrix
- Develop a complete Machine Learning workflow

---

# 📁 Project Structure

```
Week2/
│
├── README.md
├── Week2_Logistic_Regression.ipynb
├── Week2_Logistic_Regression.pdf
└── train.csv
```

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/neurofive-ml-track.git
```

---

## 2. Navigate to Week 2

```bash
cd neurofive-ml-track/Week2
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
Week2_Logistic_Regression.ipynb
```

Run all cells sequentially.

---

# 🎓 Course

Machine Learning Fundamentals

**Organized by:** Neurofive Solutions

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

This project is part of my **Machine Learning Fundamentals** learning journey, where I document each week's concepts, practical implementations, and outcomes while building a professional Machine Learning portfolio on GitHub.