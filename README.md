# Student Academic Success Prediction

Machine Learning pipeline to predict student academic outcomes (**Graduate / Dropout / Enrolled**) using advanced boosting algorithms and a Flask web interface.

---

## Key Results

| Metric              | Value                  |
|---------------------|------------------------|
| Best Model          | **LightGBM**           |
| F1-Score            | **~83%**               |
| Feature Selection   | Top 15 features (RF + RFE) |
| Class Imbalance     | Handled with SMOTE     |
| Deployment          | Flask Web Application  |

**Main findings:**
- LightGBM provided the best overall performance
- Feature selection significantly improved model efficiency
- SMOTE effectively handled the class imbalance problem

---

## Project Overview

This project aims to predict the final academic status of students based on demographic, academic, and socio-economic features.

The complete pipeline includes:

1. Exploratory Data Analysis (EDA)
2. Data cleaning and preprocessing
3. Handling class imbalance with **SMOTE**
4. Feature selection using **Random Forest + RFE** (Top 15 features)
5. Benchmark of multiple boosting models
6. Deployment of a simple **Flask web application** for real-time predictions

---

## Models Compared

- LightGBM (selected as best model)
- XGBoost
- CatBoost
- Other classical Machine Learning models

---

## Dataset

- **Name**: Predict Student Dropout and Academic Success
- **Target**: Student final status (Graduate / Dropout / Enrolled)
- **Type**: Multi-class classification

---

## How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt

###2. Training & Evaluation
Open the notebook:notebooks/1_training_and_evaluation.ipynb

This  notebook contains:
Data loading and EDA
Preprocessing
Feature selection
Model training and evaluation
Performance visualizations

###3. Web ApplicationOpen the notebook:

Open the notebook: notebooks/2_flask_web_app.ipynbThis notebook launches a Flask application with:
Prediction interface
User account management
Prediction history

## Repository Structure
student-success-prediction-ml/
├── notebooks/
│   ├── 1_training_and_evaluation.ipynb
│   └── 2_flask_web_app.ipynb
├── data/
│   └── student_dropout.csv
├── outputs/
│   └── figures/
├── docs/
├── requirements.txt
└── README.md

###Technologies

Python
Scikit-learn
LightGBM / XGBoost / CatBoost
Imbalanced-learn (SMOTE)
Flask
Pandas / NumPy
Matplotlib / Seaborn

###Features of the Web App

Real-time student success prediction
Simple and clean user interface
Prediction history tracking
Account management