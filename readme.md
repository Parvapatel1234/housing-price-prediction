## 🏠 House Price Prediction | End-to-End ML Project
Production-ready machine learning pipeline to predict median house prices using structured housing data.
Designed with industry best practices: preprocessing pipelines, reproducibility, and clean train–inference flow.

## 🔍 Problem Statement
Predict median house value based on demographic, geographic, and housing features.

## 🧠 Solution Overview
* Built a scikit-learn Pipeline for numerical & categorical data
* Applied stratified sampling to preserve income distribution
* Trained an ensemble regression model
* Persisted artifacts using joblib
* Implemented single-script training & inference workflow

## ⚙️ Tech Stack
Python · Pandas · NumPy · Scikit-learn · Joblib

## 📊 Machine Learning Model Details
* **Model:** Random Forest Regressor
* **Preprocessing:**
    1. Median imputation
    2. Standard scaling
    3. One-Hot Encoding
* **Pipeline:** ColumnTransformer + Pipeline
* **Evaluation Metric:** RMSE

## 📂 Project Structure
```text
├── main.py          # Training & inference logic
├── housing.csv      # Dataset
├── input.csv        # Test data (auto-generated)
├── output.csv       # Predictions
├── model.pkl        # Not included (large file)
├── pipeline.pkl     # Not included (large file)
└── README.md
```

## 🚫 Large Files Notice
To comply with GitHub size limits, the following files are not committed:
1. `model.pkl`
2. `pipeline.pkl`

> 📌 **Note:** Run `main.py` to train the model and persist artifacts using joblib.

## ▶️ How to Run

### 1. Train the Model
Run the following command to train the model, build the preprocessing pipeline, and persist artifacts:
```bash
python main.py
```
This will generate: `model.pkl`, `pipeline.pkl`, and `input.csv`.

### 2. Run Inference
```bash
python main.py
```
* ✔ Loads saved artifacts
* ✔ Generates predictions in `output.csv`
