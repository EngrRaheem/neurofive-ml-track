# Week 1 — Environment Setup & Exploratory Data Analysis (EDA)

##  Introduction

The first week of the Neurofive Machine Learning Fundamentals Track focuses on preparing the development environment and
learning how to explore a dataset before applying any Machine Learning algorithms.A significant portion of every Machine
Learning project involves understanding the dataset, identifying data quality issues, and recognizing the characteristics
of each feature. This process is known as **Exploratory Data Analysis (EDA)**.The Titanic dataset is used as the introductory
dataset for this week's assignment.


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


#  Folder Contents

|             File               |                     Description                    |
|--------------------------------|----------------------------------------------------|
| Week1_Titanic_EDA.ipynb        | Jupyter Notebook containing the complete EDA       |
| Week1_Titanic_EDA.pdf          | PDF export of the notebook                         |
| Week1_README.md                | Week 1 documentation                               |
| Python_Jupyter_Setup_Guide.png | Visual installation cheat sheet                    |
| Titanic_Dataset.zip            | Titanic dataset used in this assignment            |


#  Software Used

- Python 3
- Jupyter Notebook (pandas, numpy, seaborn, matplotlib, scikit-Learn)


#  Dataset Information

**Dataset Name**

Titanic — Machine Learning from Disaster

Source: Kaggle Competition Dataset
Dataset Size
- Rows: 891
- Columns: 12


# Exploratory Data Analysis Performed

The following analyses were completed:

- Dataset loading
- Dataset preview
- Dataset information
- Statistical summary
- Missing value identification
- Numerical feature identification
- Categorical feature identification


# Key Findings

- The dataset contains 891 passenger records.
- Several columns contain missing values, particularly **Age**, **Cabin**, and **Embarked**.
- Both numerical and categorical features are present.
- The dataset is suitable for classification tasks after preprocessing.


# Files Required

To run the notebook successfully, ensure the following files remain in the same directory/or you can give direct path of
dataset file as i use in this code (df = pd.read_csv(r"Complete File Path"):

```
Week1/
│
├── Week1_Titanic_EDA.ipynb
├── train.csv
```


# Required Python Libraries

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```


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


# Learning Outcomes

After completing this week, I learned how to:

- Configure a Machine Learning development environment
- Work with Jupyter Notebook
- Load datasets using Pandas
- Understand dataset structure
- Explore numerical and categorical features
- Detect missing values
- Perform basic Exploratory Data Analysis


# Assignment Status

 Completed


# Author

**Abdul Raheem**

Machine Learning Fundamentals Track

Neurofive Solutions
