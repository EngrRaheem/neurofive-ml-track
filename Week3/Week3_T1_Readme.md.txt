# Week 3 – Model Evaluation & Hyperparameter Tuning: Beyond Accuracy

## 📖 Introduction

This project is the first task of **Week 3** in the **Neurofive Machine Learning Fundamentals Track**. The objective is to evaluate and improve the Logistic Regression model developed in Week 2 using advanced model evaluation metrics and hyperparameter tuning techniques.

While accuracy is one of the most common evaluation metrics, it does not always provide a complete picture of a model's performance, especially when dealing with imbalanced datasets. Therefore, additional metrics such as Precision, Recall, and F1-Score are used to better assess classification performance.

Furthermore, **GridSearchCV** is applied to optimize the model's hyperparameters, resulting in a more reliable and better-performing classification model.

---

# 🎯 Objectives

The objectives of this task are to:

- Reuse the Titanic classification dataset from Week 2.
- Train a baseline Logistic Regression model.
- Evaluate the model using multiple performance metrics.
- Calculate Precision, Recall, and F1-Score.
- Explain why accuracy alone may be misleading.
- Improve the model using GridSearchCV.
- Tune multiple hyperparameters.
- Compare the original and optimized models.
- Understand the importance of systematic model optimization.

---

# 📂 Folder Contents

| File | Description |
|------|-------------|
| Week3_Model_Evaluation_Tuning.ipynb | Complete Jupyter Notebook |
| Week3_Model_Evaluation_Tuning.pdf | PDF version of the notebook |
| README.md | Documentation for Week 3 |
| train.csv | Titanic dataset used for training and evaluation |

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

# 🔄 Data Preprocessing

The preprocessing steps performed include:

- Loaded the Titanic dataset.
- Filled missing values in:
  - Age using the median.
  - Embarked using the mode.
  - Cabin using "Unknown".
- Converted categorical variables into numerical values using One-Hot Encoding.
- Removed unnecessary columns:
  - PassengerId
  - Name
  - Ticket
  - Cabin
- Split the dataset into training and testing subsets.

---

# 🤖 Baseline Machine Learning Model

## Algorithm Used

**Logistic Regression**

Logistic Regression is a supervised Machine Learning algorithm used for binary classification problems.

It estimates the probability that an observation belongs to one of two classes and predicts the class with the highest probability.

The baseline model was trained using Scikit-learn's default Logistic Regression settings.

---

# 📈 Model Evaluation Metrics

Instead of relying only on accuracy, the following evaluation metrics were used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics provide a more comprehensive understanding of the model's performance.

---

# 📌 Accuracy

Accuracy measures the percentage of correctly classified samples.

Although it is simple to understand, accuracy alone may produce misleading conclusions when one class is much larger than another.

---

# 📌 Precision

Precision measures how many passengers predicted as "Survived" actually survived.

Higher precision indicates fewer false positive predictions.

---

# 📌 Recall

Recall measures how many actual survivors were correctly identified by the model.

Higher recall indicates fewer false negatives.

---

# 📌 F1-Score

The F1-Score combines Precision and Recall into a single metric.

It is particularly useful when dealing with imbalanced datasets because it balances both types of classification errors.

---

# 📊 Confusion Matrix

The Confusion Matrix summarizes prediction performance by comparing actual labels with predicted labels.

It consists of:

- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

This visualization helps identify where the model performs well and where prediction errors occur.

---

# ⚠ Why Accuracy Alone Can Be Misleading

Accuracy only tells us the percentage of correct predictions made by the model.

In an imbalanced dataset, where one class contains significantly more samples than the other, a model can achieve high accuracy simply by predicting the majority class every time.

For example, if 90% of passengers did not survive, a model that always predicts "Did Not Survive" would still achieve approximately 90% accuracy while completely failing to identify passengers who actually survived.

Precision, Recall, and F1-Score provide a much more reliable evaluation because they measure different aspects of classification performance rather than only the overall number of correct predictions.

---

# 🔧 Hyperparameter Tuning

To improve model performance, **GridSearchCV** was used.

GridSearchCV automatically tests multiple combinations of hyperparameters and selects the combination that produces the best cross-validation score.

---

# ⚙ Tuned Hyperparameters

The following Logistic Regression hyperparameters were optimized:

- C (Regularization Strength)
- Solver

Multiple combinations were evaluated using 5-fold cross-validation.

---

# 📊 Model Comparison

The notebook compares the original Logistic Regression model with the optimized model.

Comparison includes:

- Original Accuracy
- Tuned Accuracy

This comparison demonstrates whether hyperparameter tuning improved predictive performance.

---

# 📈 Results

The notebook includes:

- Logistic Regression training
- Accuracy calculation
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix
- Hyperparameter tuning using GridSearchCV
- Best hyperparameter selection
- Original vs Tuned model comparison

---

# 📖 Learning Outcomes

After completing this project, I learned how to:

- Evaluate classification models beyond accuracy.
- Interpret Precision, Recall, and F1-Score.
- Understand why accuracy alone is insufficient for imbalanced datasets.
- Apply GridSearchCV for systematic hyperparameter tuning.
- Improve model performance using optimized parameters.
- Compare baseline and tuned models using quantitative metrics.
- Build more reliable and robust Machine Learning models.

---

# 📁 Project Structure

```
Week3/
│
├── README.md
├── Week3_Model_Evaluation_Tuning.ipynb
├── Week3_Model_Evaluation_Tuning.pdf
└── train.csv
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
Week3_Model_Evaluation_Tuning.ipynb
```

Run all cells sequentially to reproduce the results.

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

This project is part of my Machine Learning Fundamentals learning journey. It demonstrates practical experience in evaluating classification models using multiple performance metrics and improving model performance through hyperparameter tuning.

The techniques implemented in this project reflect standard practices used in real-world Machine Learning workflows to build accurate, reliable, and well-optimized predictive models.