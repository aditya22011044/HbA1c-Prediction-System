# HbA1c Prediction Model (Quarterly Forecast)

## Overview
This project builds a machine learning pipeline to predict **future HbA1c values** using historical patient clinical data.  
The model processes vitals and lab measurements, handles missing values, trains regression models, and forecasts HbA1c for **future quarters**.

---

## Key Objectives
- Predict HbA1c using historical medical data
- Handle missing clinical values with medical logic
- Train regression-based ML models
- Forecast HbA1c for upcoming quarters (2025–2026)

---

## Data Source
- Data is fetched from a **MySQL database**
- Limited to **10,000 patients** for scalable execution
- Key features include:
  - HbA1c
  - Blood Pressure
  - Blood Glucose
  - BMI
  - Age
  - Quarterly timestamps

---

## Data Processing
- Missing HbA1c values are handled using:
  - Last available patient value
  - Mean-based fallback when required
- Data is converted into a **quarter-wise format**
- Cleaned datasets are saved as CSV files

---

## Model Training
- Regression models are trained on processed datasets
- Models are serialized and stored as `.pkl` files
- Supports **quantile-based predictions** for robustness

---

## Prediction Pipeline
- Uses trained models to generate HbA1c predictions for:
  - Future quarters (2025–2026)
- Automatically manages:
  - Date and quarter calculations
  - Patient-level predictions
- Outputs structured prediction results

---

## Technologies Used
- Python
- Pandas
- NumPy
- MySQL Connector
- Scikit-learn
- Pickle
- Jupyter Notebook

---

## How to Run
1. Update MySQL database credentials
2. Open `HbA1c_Model.ipynb`
3. Run all cells sequentially
4. Models and prediction outputs will be generated automatically

---

## Use Cases
- Predictive healthcare analytics
- Chronic disease monitoring
- Clinical decision support
- Patient risk forecasting

---

## Author
Aditya Atole  
AI / ML Engineer
