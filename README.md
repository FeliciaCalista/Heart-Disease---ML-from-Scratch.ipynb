# Heart Disease Analysis and Prediction

## Project Description

This project aims to predict the risk of heart disease using the Heart Disease dataset (heart.csv) with the following approach:

- Exploratory Data Analysis (EDA)
- Machine Learning
- Implementing models from scratch (without pre-built ML libraries)

The main focus of this project is to understand the architecture and mathematics behind ML models, not just to generate predictions.

---

## Project Goals

1. Understand health data characteristics through EDA
2. Implement ML algorithms from scratch
3. Gain understanding of:
   - How models learn
   - How predictions are made

---

## Dataset

- **Nama**: Heart Disease Dataset
- **Kaggle**: `https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset`
- **Target**:
  - `0` → No heart disease
  - `1` → Has heart disease

After removing duplicate data, the dataset contains 302 samples.

---

## Exploratory Data Analysis (EDA)

The EDA steps include:

### Data Cleaning
- Remove duplicate data
- Check for missing values
- Validate data types

### Data Distribution Analysis
- Histogram:
  - Examine data distribution
  - Identify skewness
- Boxplot:
  - Detect outliers
  - Compare distributions across classes

### Feature Relationship Analysis
- Using Crosstab (`pd.crosstab`)
  - Used to observe relationships between categorical features and the target

---

## Data Preprocessing

- **Train-Test Split**
  - Using stratify=y to maintain class distribution
- **Feature Scaling**
  - Required for Logistic Regression
  - Optional for Decision Tree & Random Forest

---

## Model Machine Learning

### Logistic Regression (From Scratch)

**Purpose:**
- Baseline model
- Easy to interpret
- Produces probabilities mathematically

**Implemented Concepts:**
- Linear combination of features
- Sigmoid function
- Binary Cross-Entropy Loss
- Gradient Descent

---

### Decision Tree (From Scratch)

**Core Concepts:**
- Node and leaf structure
- Split selection using Gini Impurity
- Recursion
- Early stopping

---

### Random Forest (From Scratch)

**How it works:**
- Ensemble of multiple Decision Trees
- Data bootstrapping
- Random feature selection
- Voting dan probability averaging

---

## Model Evaluation

### Evaluation Metrics:
- ROC-AUC
- Confusion Matrix
- Accuracy, Precision, Recall

