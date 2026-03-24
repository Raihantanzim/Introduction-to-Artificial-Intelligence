# Harnessing NLP for Diabetic Text Classification using Neural Network
![image alt](https://github.com/Raihantanzim/Machine-Learning/blob/9bea35245988ff7fef6f43f2cebe7c19c45cdc96/Machine%20Learning%20in%20Food%20Delivery%20Operations.jpg)
## Overview
This project explores the use of machine learning and deep learning techniques for **diabetes prediction** using structured medical attributes. The main goal is to build an intelligent classification system that can help identify whether a patient is likely to have diabetes based on diagnostic features.

The project focuses on:
- preprocessing medical data
- training a Neural Network classifier
- comparing performance with traditional machine learning models
- evaluating prediction quality using classification metrics

Although the title references NLP, the implementation described in the report is based on **tabular clinical data classification** rather than free-text processing.

---

## Problem Statement
Diabetes is a serious chronic disease that can lead to major complications such as heart disease, kidney failure, nerve damage, and vision loss. Early prediction is important because it can support faster diagnosis, earlier intervention, and better patient outcomes.

This project investigates whether machine learning and neural networks can improve the accuracy of diabetes prediction using patient diagnostic features.

---

## Project Objectives
The main objectives of this project are to:

- predict diabetes using clinical and diagnostic attributes
- build and evaluate a Neural Network classification model
- compare Neural Network performance with traditional ML models
- understand how different algorithms perform on the same dataset
- support healthcare decision-making through AI-based prediction

---

## Dataset
The dataset was sourced from **GitHub** and contains medical predictor variables with one binary target variable:

- **Outcome = 1** → person has diabetes
- **Outcome = 0** → person does not have diabetes

### Features described in the report
The independent variables include:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

These features are used to predict the target variable **Outcome**.

---

## Methodology

### Data Preprocessing
The data preprocessing pipeline includes:
- train/test split using an **80:20 ratio**
- feature standardisation using **StandardScaler**
- preparation of numerical features for model training

### Feature Selection
All provided features were used because they represent important diagnostic information for diabetes prediction.

### Neural Network Model
The main proposed model is a **Neural Network** implemented using the **Keras Sequential API**.

#### Neural Network Architecture
- input layer with **10 units** and **ReLU activation**
- hidden layer with **3 units**
- output layer with **Sigmoid activation**
- optimizer: **Adam**
- training: **40 epochs**
- early stopping used to reduce overfitting

### Other Models Discussed / Compared
The report also compares or discusses:
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

---

## Evaluation Metrics
The models are evaluated using standard classification metrics:

- Accuracy
- Precision
- Recall
- F1-score

These metrics help assess how well the model predicts diabetes cases and non-diabetes cases.

---

## Results

### Best Model Performance
According to the discussion section, the **Neural Network** achieved the best overall performance:

- **Accuracy:** 0.76
- **Precision:** 0.81
- **Recall:** 0.82
- **F1-score:** 0.81

### Comparison Table
| Model | Accuracy | Precision | Recall | F1 Score |
|------|---------:|----------:|-------:|---------:|
| Neural Networks | 0.76 | 0.81 | 0.82 | 0.81 |
| Logistic Regression | 0.75 | 0.81 | 0.80 | 0.81 |
| Support Vector Machine | 0.72 | 0.74 | 0.89 | 0.81 |
| Random Forest | 0.75 | 0.81 | 0.80 | 0.80 |

The results show that the Neural Network slightly outperformed the other models overall, while SVM achieved the highest recall.

---

## Key Insights
- Neural Networks performed best overall in this study
- Logistic Regression showed competitive performance with simpler modelling
- SVM achieved strong recall but lower accuracy
- Random Forest provided good interpretability but slightly lower performance
- Hyperparameter tuning and preprocessing improved model effectiveness

---

## Tech Stack
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

