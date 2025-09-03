## Identifying Risk Factors and Stroke Prediction Using Machine Learning

This project utlizes machine learning to predict stroke risk based on patient clinical and lifestyle data and determine the major risk factors. It involves various trained models and an interactive web interface built with Flask.

---

## Project Structure

- `cerebralstroke.ipynb` – Jupyter Notebook with full ML pipeline
- `diagrams.ipynb` – Jupyter Notebook with some visualizations
- `cleaned.csv` – Preprocessed dataset (one-hot encoded)
- `dataset.csv` – Raw dataset

---

## Problem Statement

Stroke is the third leading cause of death in the world. Early detection and intervention can drastically reduce mortality and long-term disability. This project aims to predict stroke likelihood from patient data using machine learning techniques.

---

## Models Evaluated

| Model               | Accuracy | F1 Score | AUC    |
|---------------------|----------|----------|--------|
| Logistic Regression | 0.79     | 0.68     | 0.8548 |
| Random Forest       | 0.99     | 0.99     | 0.9998 |
| XGBoost             | 0.94     | 0.92     | 0.9833 |
| K-Nearest Neighbors | 0.97     | 0.96     | 0.9906 |
| Gradient Boosting   | 0.91     | 0.88     | 0.9697 |
| Decision Tree       | 0.98     | 0.97     | 0.9872 |
| Neural Network      | 0.92     | 0.92     | 0.9673 |

**Random Forest** was selected for deployment due to superior balance across metrics.

---

## Exploratory Data Analysis

- Age distribution and stroke correlation
- BMI vs. Glucose colored by stroke outcome
- Hypertension and smoking trends
- Correlation heatmap between features

Visuals were generated using `matplotlib` and `seaborn` in the notebook.

---

## Features Used

- Age, BMI, Hypertension, Glucose
- Gender, Marriage status
- Residence type, Smoking status (one-hot)

---

## Web App Demo

Built with Flask. Users enter patient information and receive a stroke risk probability along with a color-coded risk bar:

- 🟢 Low Risk
- 🟡 Mild Risk
- 🟠 Moderate Risk
- 🔴 High Risk

Inputs are validated and scaled before prediction using the same scaler and model from the notebook.
- [Stroke Application repository](https://github.com/BrandyRumRum/Stroke-Application)
---

## 🧠 Stroke Prediction Model  

A machine learning project to predict stroke risk using healthcare data.  
Built and deployed as part of a team project with multiple ML models evaluated.  

🚀 **Live Demo:** [Stroke Prediction App](https://stroke-prediction-applicaiton.onrender.com/)  
