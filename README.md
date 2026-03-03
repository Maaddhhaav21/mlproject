# 🎓 Student Exam Performance Predictor (End-to-End ML Project)

A production-ready **End-to-End Machine Learning Web Application** that predicts a student's **Math Score** based on demographic and academic features.

🌐 **Live Demo:**  
https://studentperfomancepredictor.onrender.com  

> ⚠️ Note: Hosted on Render Free Tier. First load may take 30–60 seconds due to cold start.

---

## 🚀 Project Highlights

✔ End-to-End ML Pipeline (Training → Prediction → Deployment)  
✔ Modular Project Architecture  
✔ Custom Exception Handling & Logging  
✔ Preprocessing using ColumnTransformer  
✔ Model Persistence using Pickle  
✔ Web Deployment using Flask + Gunicorn  
✔ Live Cloud Deployment (Render)

---

## 🧠 Problem Statement

The objective of this project is to build a regression model that predicts a student's **Math Score** using:

- Gender  
- Race / Ethnicity  
- Parental Level of Education  
- Lunch Type  
- Test Preparation Course  
- Reading Score  
- Writing Score  

---

## 🏗️ System Architecture

User Input → Flask App → DataFrame Creation →  
Preprocessor (Encoding + Scaling) →  
Trained Regression Model →  
Predicted Math Score → Web UI

---

## 📁 Project Structure

```
mlproject/
│
├── app.py                      # Flask application entry point
├── requirements.txt            # Project dependencies
├── README.md                   # Project documentation
│
├── templates/                  # HTML templates
│   └── index.html
|   └── style.css
│
|
│   
│
├── src/                        # Source code
│   │
│   ├── components/             # Training components
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/               # Training & Prediction pipeline
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   │
│   ├── exception.py            # Custom exception handling
│   ├── logger.py               # Logging configuration
│   └── utils.py                # Utility functions
│
├── artifacts/                  # Saved models & preprocessing objects
│   ├── model.pkl
│   └── preprocessor.pkl
│
└── notebook/                   # Jupyter notebooks for experimentation
    └── EDA.ipynb
```

---


---

## ⚙️ Tech Stack

- Python  
- Flask  
- Scikit-learn  
- Pandas  
- NumPy  
- HTML & CSS  
- Gunicorn  
- Render (Cloud Deployment)

---

## 📊 Machine Learning Details

- Problem Type: Regression  
- Target Variable: Math Score  
- Preprocessing:
  - OneHotEncoder (Categorical features)
  - StandardScaler (Numerical features)
  - ColumnTransformer
- Model: RandomForestRegressor (Best selected model)

---

## 🔍 Workflow

### 1️⃣ Data Ingestion
- Load dataset
- Split into train/test

### 2️⃣ Data Transformation
- Handle categorical encoding
- Scale numerical features
- Save preprocessor object

### 3️⃣ Model Training
- Train regression models
- Evaluate performance
- Save best model

### 4️⃣ Prediction Pipeline
- Load saved model
- Apply preprocessing
- Predict math score

### 5️⃣ Deployment
- Flask application
- Gunicorn production server
- Deployed on Render cloud platform

---

## 👨‍💻 Author

**Madhav Manoj**
