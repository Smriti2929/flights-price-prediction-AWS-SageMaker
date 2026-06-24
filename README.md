# ✈️ Flight Price Prediction using AWS SageMaker

## Live Demo
🔗 Streamlit App:
https://flights-price-prediction-aws-sagemaker-dau2cubgs9s4rue2mz45mg.streamlit.app/

## 📌 Project Overview

This project predicts airline ticket prices using Machine Learning and demonstrates an end-to-end MLOps workflow using AWS SageMaker, Amazon S3, XGBoost, and Streamlit.

The project covers the complete machine learning lifecycle, including:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Model Training
* Model Evaluation
* Model Serialization
* Interactive Streamlit Web Application
* Cloud Storage with Amazon S3

---

## 🚀 Project Architecture

```text
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Engineering Pipeline
      │
      ▼
XGBoost Regression Model
      │
      ▼
Model Evaluation
      │
      ▼
Saved Model (.pkl)
      │
      ▼
Streamlit Web Application
```

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Feature Engine
* XGBoost
* AWS SageMaker
* Amazon S3
* Streamlit
* Joblib
* Pickle

---

## 📂 Project Structure

```text
flight-price-prediction-AWS-SageMaker
│
├── app.py
├── requirements.txt
│
├── data/
│   ├── flight_price.csv
│   ├── train.csv
│   ├── val.csv
│   └── test.csv
│
├── model/
│   ├── preprocessor.pkl
│   └── xgb_model.pkl
│
└── notebooks/
    ├── data-cleaning.ipynb
    ├── EDA.ipynb
    ├── feature-engineering.ipynb
    ├── model-training.ipynb
    └── eda_helper_functions.py
```

---

## 🔍 Feature Engineering

The preprocessing pipeline includes:

* Rare Label Encoding
* Mean Encoding
* Count Frequency Encoding
* Datetime Feature Extraction
* Outlier Treatment using Winsorization
* Power Transformation
* Standardization & Scaling
* Feature Selection using Random Forest

---

## 🤖 Model

### Algorithm

XGBoost Regressor

### Evaluation Results

| Dataset    | RMSE    | R² Score |
| ---------- | ------- | -------- |
| Validation | 2158.20 | 0.7908   |
| Test       | 2217.28 | 0.7565   |

The model explains approximately **75–79% of the variance** in flight prices while maintaining good generalization on unseen data.

---

## ☁️ AWS Services Used

### Amazon S3

Used for:

* Dataset Storage
* Processed Data Storage
* Model Artifact Storage

### AWS SageMaker

Used for:

* Data Preparation
* Feature Engineering
* Model Development Environment
* Experimentation and Training Workflow

---

## 🌐 Streamlit Application

The project includes a Streamlit web application where users can enter:

* Airline
* Date of Journey
* Source
* Destination
* Departure Time
* Arrival Time
* Duration
* Total Stops
* Additional Information

and receive an instant flight price prediction.

---

## ▶️ Running the Project Locally

### Clone Repository

```bash
git clone https://github.com/Smriti2929/flights-price-prediction-AWS-SageMaker.git
cd flights-price-prediction-AWS-SageMaker
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Streamlit App

```bash
python -m streamlit run app.py
```

---

## 📈 Future Improvements

* Hyperparameter Optimization
* Model Deployment on AWS SageMaker Endpoints
* CI/CD Pipeline
* Docker Containerization
* Real-time Flight Data Integration

---
