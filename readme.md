##🏠 House Price Prediction | End-to-End ML Project
Production-ready machine learning pipeline to predict median house prices using structured housing data.
Designed with industry best practices: preprocessing pipelines, reproducibility, and clean train–inference flow.

#🔍 Problem Statement
Predict median house value based on demographic, geographic, and housing features.

#🧠 Solution Overview
Built a scikit-learn Pipeline for numerical & categorical data
Applied stratified sampling to preserve income distribution
Trained an ensemble regression model
Persisted artifacts using joblib
Implemented single-script training & inference workflow

#⚙️ Tech Stack
Python · Pandas · NumPy · Scikit-learn · Joblib
📊 Machine learning model Details 
Model: Random Forest Regressor
Preprocessing:
    1. Median imputation
    2. Standard scaling
    3. One-Hot Encoding
    4. Pipeline: ColumnTransformer + Pipeline
    5. Evaluation Metric: RMSE

📂 Project Structure
├── main.py # Training & inference logic
├── housing.csv # Dataset
├── input.csv # Test data (auto-generated)
├── output.csv # Predictions
├── model.pkl # Not included (large file)
├── pipeline.pkl # Not included (large file)
└── README.md

🚫 Large Files Notice
To comply with GitHub size limits, the following files are not committed:
    1. model.pkl 
    2. pipeline.pkl

📌 Run main.py to train the model and persist artifacts using joblib.

#▶️ How to Run ?
Run the following command to:
    •	Train the model
    •	Build the preprocessing pipeline
    •	Persist both using joblib
>>python main.py

This will generate:
    1. model.pkl
    2. pipeline.pkl
    3. input.csv

#Run Inference
>>python main.py
    ✔ Loads saved artifacts
    ✔ Generates predictions in output.csv

