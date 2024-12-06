# Heart Disease Prediction: A Machine Learning Approach

## Project Overview
Cardiovascular diseases are among the leading causes of death worldwide. Early detection of heart disease is crucial to improving patient outcomes and quality of life. This project builds a machine learning pipeline to predict the likelihood of heart disease based on patient health indicators, such as age, blood pressure, cholesterol levels, and lifestyle habits.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Development](#model-development)
- [Model Evaluation](#model-evaluation)
- [Feature Importance](#feature-importance)
- [Conclusion](#conclusion)
- [Setup](#setup)

## Introduction
This project leverages supervised learning techniques to develop a classification model for heart disease prediction. The objective is to identify individuals at risk based on health and demographic data, facilitating early medical intervention.

## Dataset
The dataset contains various health-related features:
- **Demographics**: Age, gender
- **Health Indicators**: Blood pressure, cholesterol, glucose levels, height, weight
- **Lifestyle Factors**: Smoking, alcohol consumption, physical activity
- **Target Variable**: Presence of heart disease (`0` or `1`)

## Data Preprocessing
To prepare the data for modeling, the following steps were performed:
1. **Handling Missing Values**: Replaced missing and infinite values with the median.
2. **Encoding Categorical Features**: Converted binary categorical features (e.g., gender) into numerical format.
3. **Scaling Numerical Features**: Standardized features using `StandardScaler` to normalize the range of values.

## Model Development
The following machine learning models were trained and evaluated:
1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **Support Vector Machine (SVM)**

## Model Evaluation
Each model was evaluated using the following metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

Performance summary:

| Model                | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | 0.712    | 0.730     | 0.672  | 0.699    |
| Decision Tree        | 0.630    | 0.630     | 0.629  | 0.629    |
| Random Forest        | 0.714    | 0.719     | 0.702  | 0.711    |
| SVM                  | 0.719    | 0.764     | 0.632  | 0.692    |

## Feature Importance
Using the Random Forest model, the following features were identified as the most important predictors of heart disease:
1. Age
2. Systolic blood pressure (`ap_hi`)
3. Weight
4. Height
5. Diastolic blood pressure (`ap_lo`)

## Conclusion
The **Random Forest** model was selected as the final model due to its superior performance across evaluation metrics. The model provides a balance between accuracy and interpretability, making it a valuable tool for heart disease prediction.

## Setup
To replicate this project:
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-repo/heart-disease-prediction.git
