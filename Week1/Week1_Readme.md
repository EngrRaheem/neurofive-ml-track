# Week 1 
# Task 1 — Environment Setup & Exploratory Data Analysis (EDA)

##  Introduction

The first week of the Neurofive Machine Learning Fundamentals Track focuses on preparing the development environment and learning how to explore a dataset before applying any Machine Learning algorithms.

A significant portion of every Machine Learning project involves understanding the dataset, identifying data quality issues, and recognizing the characteristics of each feature. This process is known as **Exploratory Data Analysis (EDA)**.

The Titanic dataset is used as the introductory dataset for this week's assignment.

---

#  Objectives

- Install Python
- Install Jupyter Notebook
- Configure the Machine Learning environment
- Install required Python libraries
- Download the Titanic dataset
- Load the dataset using Pandas
- Explore dataset structure
- Generate descriptive statistics
- Identify missing values
- Identify numerical and categorical features
- Summarize findings

---

#  Folder Contents

| File | Description |
|------|-------------|
| Week1_Titanic_EDA.ipynb | Jupyter Notebook containing the complete EDA |
| Week1_Titanic_EDA.pdf | PDF export of the notebook |
| README.md | Week 1 documentation |
| Quick_Start_Guide.pdf | Quick reference guide for beginners |
| Python_Jupyter_Setup_Guide.png | Visual installation cheat sheet |
| Titanic_Dataset.zip | Titanic dataset used in this assignment |

---

# 🛠 Software Used

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
---

#  Dataset Information

**Dataset Name**

Titanic — Machine Learning from Disaster

Source

Kaggle Competition Dataset

Dataset Size

- Rows: 891
- Columns: 12

---

# Exploratory Data Analysis Performed

The following analyses were completed:

- Dataset loading
- Dataset preview
- Dataset information
- Statistical summary
- Missing value identification
- Numerical feature identification
- Categorical feature identification

---

# Key Findings

- The dataset contains 891 passenger records.
- Several columns contain missing values, particularly **Age**, **Cabin**, and **Embarked**.
- Both numerical and categorical features are present.
- The dataset is suitable for classification tasks after preprocessing.

---

# Files Required

To run the notebook successfully, ensure the following files remain in the same directory:

```
Week1/
│
├── Week1_Titanic_EDA.ipynb
├── train.csv
```

---

# Required Python Libraries

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

# Running the Notebook

Navigate to the Week1 directory:

```bash
cd "Week1"
```

Launch Jupyter Notebook:

```bash
python -m notebook
```

Open:

```
Week1_Titanic_EDA.ipynb
```

Run each notebook cell sequentially.

---

# Learning Outcomes

After completing this week, I learned how to:

- Configure a Machine Learning development environment
- Work with Jupyter Notebook
- Load datasets using Pandas
- Understand dataset structure
- Explore numerical and categorical features
- Detect missing values
- Perform basic Exploratory Data Analysis

---

---

#  Task 2 – Data Cleaning & Visualization

##  Introduction

After performing Exploratory Data Analysis (EDA) in Task 1, the second task focuses on preparing the dataset for Machine Learning. Real-world datasets often contain missing values, inconsistent information, and unusual observations (outliers) that can negatively impact model performance. Before training any predictive model, the dataset must be cleaned and explored visually to gain deeper insights into its characteristics.

This task demonstrates essential data preprocessing techniques and uses visual analytics to better understand passenger survival patterns in the Titanic dataset.

---

#  Objectives

The primary objectives of this task were:

- Handle missing values using appropriate preprocessing techniques.
- Justify the selected data cleaning strategy.
- Detect potential outliers in numerical features.
- Explore the dataset through multiple visualizations.
- Understand relationships between variables.
- Identify features that are likely to influence passenger survival.
- Prepare the dataset for future Machine Learning models.

---

#  Data Cleaning Performed

The following preprocessing steps were completed:

- Examined missing values in every feature.
- Filled missing values in the **Age** column using the median.
- Filled missing values in the **Embarked** column using the mode.
- Replaced missing values in the **Cabin** column with "Unknown".
- Verified that missing values were handled successfully.

### Why `fillna()` instead of `dropna()`?

Using `dropna()` would remove many passenger records and reduce the amount of training data available. Since the Titanic dataset is relatively small, preserving as much information as possible is beneficial. Therefore, missing values were imputed using statistically appropriate replacement methods.

---

#  Data Visualizations

Four different visualizations were created to better understand the dataset.

## 1. Histogram

Purpose:

- Examine the distribution of passenger ages.
- Identify whether the data is normally distributed.
- Observe age concentration among passengers.

---

## 2. Boxplot

Purpose:

- Detect outliers within the Fare feature.
- Understand the spread of ticket prices.
- Identify unusually expensive ticket purchases.

---

## 3. Bar Chart

Purpose:

- Compare the number of passengers who survived versus those who did not survive.
- Provide a quick overview of class distribution within the target variable.

---

## 4. Correlation Heatmap

Purpose:

- Measure relationships among numerical features.
- Identify positively and negatively correlated variables.
- Discover features that may contribute most to survival prediction.

---

#  Observations

Some important observations from this analysis include:

- The Age column contained several missing values requiring preprocessing.
- The Cabin feature had the highest percentage of missing data.
- Passenger Fare contains several extreme values (outliers).
- Female passengers generally exhibited higher survival rates.
- Passenger Class (Pclass) showed a noticeable relationship with survival.
- Most passengers embarked from Southampton (S).

---

#  Key Insights

The visualizations indicate that:

- **Sex** is one of the strongest predictors of survival.
- Passengers travelling in **First Class** had a greater chance of survival.
- Fare is positively associated with passenger class and survival.
- Age alone appears to have a weaker influence compared to gender and passenger class.

---

#  Skills Learned

During this task, the following practical skills were developed:

- Data Cleaning
- Missing Value Treatment
- Feature Inspection
- Outlier Detection
- Exploratory Data Visualization
- Statistical Data Interpretation
- Correlation Analysis
- Markdown Documentation
- Professional Notebook Organization

---

#  Python Libraries Used

| Library | Purpose |
|----------|---------|
| Pandas | Data loading and preprocessing |
| NumPy | Numerical operations |
| Matplotlib | Basic plotting |
| Seaborn | Statistical data visualization |

---

#  Deliverables

This folder contains:

- Week1_Titanic_EDA.ipynb
- Week1_Titanic_EDA.pdf
- README.md
- Getting Started with Python and Jupyter Notebook.png
- Quick_Start_Guide.pdf
- Titanic Dataset (.zip)

---

#  Learning Outcome

After completing Task 2, I am able to:

- Clean real-world datasets.
- Handle missing values using appropriate techniques.
- Detect outliers through visualization.
- Create informative statistical plots.
- Interpret graphical insights from data.
- Prepare datasets for subsequent Machine Learning workflows.

---

#  Next Step

The cleaned and visualized dataset produced in this task will be used in the upcoming weeks to perform feature engineering, train Machine Learning models, and evaluate predictive performance.


---

# Author

**Abdul Raheem**

Machine Learning Fundamentals Track

Neurofive Solutions
