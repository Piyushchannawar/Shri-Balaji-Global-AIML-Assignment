# Customer Churn Prediction using Machine Learning

## Project Overview
This project focuses on predicting **customer churn** for a telecom company using machine learning. The goal is to determine whether a customer is likely to leave the service based on their account details, service usage, and billing information. The project demonstrates a complete end-to-end machine learning workflow including data preprocessing, visualization, model training, and evaluation.

---

## Dataset
- **Name:** Telco Customer Churn Dataset  
- **Source:** Public dataset (Kaggle / UCI Repository)  
- **Records:** ~7,000 customers  
- **Target Variable:** `Churn`  
  - `1` → Customer churned  
  - `0` → Customer did not churn  

The dataset contains both numerical and categorical features such as:
- Tenure
- MonthlyCharges
- TotalCharges
- Contract type
- Internet services
- Payment method

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

---

## Project Workflow

### 1. Data Loading & Exploration
- Loaded the dataset using pandas
- Inspected data structure using `head()` and `info()`

### 2. Data Preprocessing
- Converted `TotalCharges` from text to numeric format
- Handled missing values using median imputation
- Converted target variable `Churn` from categorical (`Yes/No`) to numerical (`1/0`)
- Dropped irrelevant column (`customerID`)
- Applied **one-hot encoding** to categorical features

### 3. Data Visualization
- Plotted churn distribution to understand class imbalance
- Used box plots to analyze:
  - Tenure vs Churn
  - Monthly Charges vs Churn

### 4. Model Building
- Split data into training and testing sets
- Applied feature scaling using `StandardScaler`
- Trained a **Logistic Regression** model

### 5. Model Evaluation
- Evaluated model using:
  - Accuracy score
  - Confusion matrix (visualized using heatmap)

---

## Model Used
### Logistic Regression
Logistic Regression was chosen because:
- Churn prediction is a **binary classification problem**
- The model is simple and easy to interpret
- It works well with structured tabular data
- It provides probabilistic outputs useful for business decisions

---

## Results
- **Accuracy:** ~80%
- The confusion matrix shows that the model correctly predicts a large portion of both churned and non-churned customers.
- Visual evaluation helps understand correct and incorrect predictions.

---
