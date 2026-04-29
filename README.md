# IoT Regression Analysis using Machine Learning and Deep Learning (RT-IoT2022)

## 📌 Project Overview
This project applies machine learning and deep learning regression models to the RT-IoT2022 dataset to predict network flow behaviour in IoT-based cyber-physical systems.

The main goal is to compare different models under varying feature selection settings and evaluate their performance using standard regression metrics.

---

## 🎯 Objectives
- Apply multiple regression algorithms to IoT network data  
- Evaluate the impact of feature selection (45, 40, 35, 30 features)  
- Compare ML and DL model performance  
- Identify the best-performing model based on MAE, RMSE, and R²  

---

## 📊 Dataset
The RT-IoT2022 dataset contains realistic IoT network traffic data including normal and attack behaviours.

Source:  
https://archive.ics.uci.edu/dataset/942/rt-iot2022

---

## ⚙️ Methodology

The project follows a structured pipeline:

1. Data preprocessing (encoding, cleaning, scaling)  
2. Feature selection using SelectKBest (F-test)  
3. Training multiple models  
4. Evaluation using regression metrics  
5. Model saving for future use  

---

## 🤖 Models Used

### Machine Learning Models
- Linear Regression  
- Ridge Regression  
- Gradient Boosting Regressor  
- Extra Trees Regressor  

### Deep Learning Models
- MLP Regressor  
- Autoencoder-based Regression Model  

---

## 📏 Evaluation Metrics

- **MAE (Mean Absolute Error)**  
- **RMSE (Root Mean Squared Error)**  
- **R² Score (Coefficient of Determination)**  

These metrics measure prediction accuracy and model reliability.

---

## 📉 Experimental Setup

- Feature sets tested: 45, 40, 35, 30  
- Deep learning epochs: 15, 10, 5  
- Train-test split: 80/20  
- Standard scaling applied to all features  

---

## 🏆 Key Findings

- Extra Trees Regressor achieved the best overall performance  
- Feature selection significantly improved model accuracy  
- Ensemble methods outperformed linear and deep learning models  
- Deep learning models were sensitive to epoch and feature variation  

---

## 📦 Model Saving

All trained models are saved using:
- `joblib` for machine learning models  
- `.h5` format for deep learning models  

---

## 📊 Outputs

The project generates:
- Performance tables (MAE, RMSE, R²)  
- Comparison charts across feature sets  
- Best model analysis plots  
- Saved trained models  

---

## 🚀 How to Run

Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn tensorflow joblib
