# Week 2 – Task 2: House Price Prediction Using Linear Regression

## 📖 Introduction

This project is the second task of **Week 2** in the **Neurofive Machine Learning Fundamentals Track**. Unlike classification problems, which predict discrete categories, regression models are designed to predict continuous numerical values.

In this task, a **Linear Regression** model was developed to estimate house prices using the **California Housing Dataset** provided by Scikit-learn. The project follows a complete machine learning workflow, including dataset exploration, feature selection, model training, prediction, performance evaluation, and result interpretation.

The goal is to understand how numerical features influence house prices and evaluate the model using standard regression metrics.

---

# 🎯 Objectives

The objectives of this task are to:

- Load a real-world housing dataset.
- Explore and understand the dataset.
- Select the most influential features affecting house prices.
- Split the dataset into training and testing subsets.
- Train a Linear Regression model using Scikit-learn.
- Predict house prices on unseen data.
- Evaluate model performance using RMSE and R² Score.
- Visualize Actual vs Predicted house prices.
- Explain the R² Score in simple, non-technical language.

---

# 📂 Folder Contents

| File | Description |
|------|-------------|
| Week2_Task2_House_Price_Regression.ipynb | Complete Jupyter Notebook containing the regression model |
| Week2_Task2_House_Price_Regression.pdf | PDF version of the notebook |
| README.md | Documentation for Week 2 Task 2 |

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

California Housing Dataset

### Dataset Source

Scikit-learn (`sklearn.datasets.fetch_california_housing`)

### Problem Type

Regression

### Target Variable

**MedHouseVal**

The target variable represents the median house value for each California district.

---

# 📋 Dataset Features

The California Housing Dataset contains several numerical features describing different aspects of housing districts.

Examples include:

- Median Income
- House Age
- Average Number of Rooms
- Average Number of Bedrooms
- Population
- Average Occupancy
- Latitude
- Longitude

---

# 🔍 Feature Selection

For this project, the following features were selected based on their expected impact on house prices:

- MedInc (Median Income)
- HouseAge (Average House Age)
- AveRooms (Average Number of Rooms)
- AveOccup (Average Occupancy)
- Latitude (Location)

These features provide meaningful information related to property value while keeping the model simple and easy to interpret.

---

# ✂ Dataset Splitting

The dataset was divided into:

- **Training Set:** 80%
- **Testing Set:** 20%

The training dataset was used to train the model, while the testing dataset was used to evaluate its predictive performance on unseen data.

---

# 🤖 Machine Learning Model

## Algorithm Used

**Linear Regression**

Linear Regression is one of the most fundamental supervised Machine Learning algorithms used for regression problems.

It predicts continuous numerical values by learning the relationship between input features and the target variable.

The model attempts to fit the best possible straight line through the training data while minimizing prediction error.

---

# 📈 Model Evaluation

The trained model was evaluated using two widely used regression metrics:

## Root Mean Squared Error (RMSE)

RMSE measures the average difference between predicted and actual house prices.

- Lower RMSE indicates better prediction accuracy.
- RMSE is expressed in the same units as the target variable.

---

## R² Score (Coefficient of Determination)

The R² Score measures how well the selected features explain the variation in house prices.

- R² = 1.0 → Perfect prediction
- R² = 0.0 → Model explains none of the variation
- Higher values indicate better predictive performance.

---

# 📊 Data Visualization

A scatter plot was generated to compare:

- Actual House Prices
- Predicted House Prices

A well-performing model produces points that lie close to an imaginary diagonal line, indicating that predicted values closely match actual values.

---

# 📌 Results

The notebook includes:

- Dataset exploration
- Feature selection
- Linear Regression model training
- House price prediction
- RMSE calculation
- R² Score calculation
- Actual vs Predicted scatter plot
- Model interpretation

---

# 💡 Plain English Explanation of R² Score

The R² Score tells us how much of the difference in house prices can be explained by the information provided to the model.

For example, if the model achieves an R² Score of **0.80**, it means that about **80% of the variation in house prices** can be explained using the selected features. The remaining variation is caused by factors that were not included in the model.

In simple terms, a higher R² Score means the model's predictions are generally closer to the actual house prices.

---

# 📖 Learning Outcomes

After completing this project, I learned how to:

- Solve a regression problem using Machine Learning.
- Select meaningful features for prediction.
- Train a Linear Regression model.
- Split data into training and testing subsets.
- Predict continuous numerical values.
- Evaluate regression models using RMSE and R² Score.
- Interpret regression results.
- Visualize prediction performance using scatter plots.

---

# 📁 Project Structure

```
Week2/
│
├── README.md
├── Week2_Task2_House_Price_Regression.ipynb
└── Week2_Task2_House_Price_Regression.pdf
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
Week2_Task2_House_Price_Regression.ipynb
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

This project is part of my **Machine Learning Fundamentals** learning journey. Each notebook in this repository demonstrates practical implementation of machine learning concepts while maintaining professional documentation and reproducible workflows.

Future weeks will expand upon these foundations by introducing more advanced machine learning algorithms, feature engineering techniques, and model evaluation strategies.