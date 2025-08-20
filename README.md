# Soil Irrigation System: Moisture Prediction with Machine Learning

This repository demonstrates a complete machine learning pipeline applied to data collected from a **soil irrigation system**.  
The system uses sensor readings (temperature, humidity, and motor state) to predict soil moisture.  

---

## 📂 Contents
- `environmental_model.ipynb` — Jupyter Notebook containing the full ML pipeline.
- `feeds.csv` — Dataset with raw sensor values (temperature, humidity, motor, moisture).

---

## ⚙️ Pipeline Overview
1. **Data Preprocessing**
   - Raw sensor readings (temperature & humidity as continuous features, motor state as categorical feature).
   - Scaling of numerical inputs with `StandardScaler`.
   - Train-test split with stratification on the motor state.

2. **Exploratory Data Analysis (EDA)**
   - Scatter plots and pairwise relationships.
   - Visual inspection of how motor state affects soil moisture.
   - 3D visualization of temperature, humidity, and moisture.

3. **Model Training**
   - Linear Regression
   - Polynomial Regression
   - Decision Tree Regressor
   - Neural Network (MLP Regressor)
   - XGBoost Regressor
   - AdaBoost Regressor

4. **Evaluation**
   - Models compared using **Mean Squared Error (MSE)** and **R² score** as well as Predicted moisture VS Actual moisture plot for each model
   - Final recommendation of the most suitable model for predicting soil moisture

5. **Prediction**
   - The most suitable model is used for predicting soil moisture for new, unseen values of temperature, humidity and motor state
