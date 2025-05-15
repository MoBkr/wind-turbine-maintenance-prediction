# ⚙️ Wind Turbine Maintenance Prediction using Machine Learning

## 🚀 Overview

This project tackles a real-world **Predictive Maintenance** challenge for wind turbines, inspired by industrial applications from **GE Renewable Energy** and **Siemens Gamesa**. By analyzing sensor data, we aim to predict the maintenance status of each turbine and classify its condition into three categories:

- **0 — Healthy 🟢**: No maintenance required.  
- **1 — Maintenance Suggested 🟡**: May need servicing soon.  
- **2 — Immediate Maintenance Required 🔴**: Critical failure is imminent.

The goal is to **reduce downtime**, **optimize maintenance schedules**, and **increase operational efficiency** in wind farms through data-driven decisions.

---

## 🎯 Project Objectives

- Build a robust machine learning model for multi-class classification of turbine health.
- Explore and clean real-world sensor data.
- Apply effective feature engineering to extract meaningful insights.
- Evaluate and tune models for high performance.
- Simulate a practical solution that aligns with industry needs.

---

## 🧠 Skills Demonstrated

> This project reflects core skills relevant to Data Science and Machine Learning roles:

- **Python for Data Analysis**
- **Data Cleaning & Preprocessing**
- **Exploratory Data Analysis (EDA)** using `pandas`, `matplotlib`, and `seaborn`
- **Feature Engineering** and handling **class imbalance**
- **Model Building & Evaluation** with `scikit-learn` and `XGBoost`
- **Hyperparameter Tuning**
- **Performance Metric**:F1-score
- **Clear Reporting** and **real-world simulation**

---

## 📁 Files in this Repository

- `project.ipynb`: Complete Jupyter Notebook including data exploration, model building, and results.
- `wind_turbine_maintenance_data.csv`: The dataset with sensor readings and labels.

---

## 📊 Dataset Description

The dataset contains anonymized **sensor data from wind turbines** and a target label:

- Numerical features representing sensor readings
- Target variable `Condition` with values {0, 1, 2} for maintenance status

---

## 🔄 Workflow Summary

1. **Load & inspect the data**
2. **Handle missing values & outliers**
3. **EDA to understand feature relationships**
4. **Encode and scale features**
5. **Split the data and handle class imbalance**
6. **Train multiple ML models (Random Forest, XGBoost)**
7. **Evaluate models using classification metrics**
8. **Interpret results and highlight business impact**

---

## 📈 Key Results

- **Best Model**: [XGBClassifier]
- **Macro F1-score**: 77%
- Important features identified:
  - Sensor X, Sensor Y strongly indicate potential failures.
- Applied [SMOTE / class weights] to address class imbalance and improve generalization.

---

## 🧪 How to Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/your-username/wind-turbine-maintenance-prediction.git
cd wind-turbine-maintenance-prediction

# 2. Install required packages
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook project.ipynb
