# Post-Operative-Delirium
Machine learning project predicting post-operative delirium in elderly surgical patients using clinical features like age, frailty, and lab values. Includes data cleaning, EDA, multiple ML models, risk-factor analysis, and a simple interface for Low/High delirium risk prediction.
Predicting Post-Operative Delirium Using Machine Learning

This repository presents a machine learning workflow designed to estimate the likelihood of post-operative delirium in elderly surgical patients. Delirium is a serious but preventable complication, and early identification of high-risk individuals can support better monitoring and intervention.

Project Summary

The goal of this project is to build an interpretable classification model that uses routinely collected clinical data to predict whether a patient may develop delirium after surgery. The repository includes data cleaning steps, exploratory analysis, model development, evaluation, and a simple risk-prediction interface.

Dataset

The dataset contains anonymized patient records with features typically available in peri-operative settings, such as:

Age

Frailty Index

Hematocrit

Albumin

Creatinine

ICU admission indicator

Post-operative length of stay

Additional peri-operative variables

The target variable indicates whether the patient experienced post-operative delirium (0 = No, 1 = Yes). Delirium cases are fewer, so models are trained with attention to class imbalance.

Data Processing

Key processing steps include converting text-encoded numeric fields, imputing missing values using medians, removing patient identifiers, scaling features where needed, and applying a stratified train–test split to preserve the delirium ratio.

Exploratory Analysis

Initial analysis examines delirium frequency and the relationship between delirium and features like age and frailty. These trends help guide model expectations and align with known clinical risk factors.

Machine Learning Models

The project evaluates several classical machine learning algorithms:

Logistic Regression

Support Vector Machine

Random Forest

Multi-Layer Perceptron

Models are assessed using confusion matrices, accuracy, recall, and ROC-AUC. Class weighting is used to improve detection of delirium cases.

Key Findings

Across models, predictors such as age, frailty, and selected lab values consistently appear as important contributors to delirium risk. A simple interface is included to demonstrate how a clinician could enter patient values and receive a Low or High risk flag.

Limitations

This project is meant for research and educational purposes only. It is based on a single dataset, does not include all clinically relevant variables, and has not undergone external validation. It is not intended for real medical decision-making.

Future Enhancements

Future improvements could include incorporating additional datasets, expanding the feature set, testing more advanced models, performing calibration, and conducting bias and fairness analysis.

Reference

Zhao, Hong (2022). Machine learning delirium. Mendeley Data, V1.
