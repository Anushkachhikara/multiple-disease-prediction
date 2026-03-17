# 🩺 Disease Prediction System

A machine learning-based web application that predicts the likelihood of **Heart Disease**, **Diabetes**, and **Kidney Disease** using trained ML models — deployed with an interactive Streamlit interface.

---

## 🔍 Overview

This project provides an end-to-end disease prediction system that takes user-input clinical parameters and returns a prediction on whether the patient is likely to have a specific disease. The system is designed to assist in early detection and awareness — it is **not** a substitute for professional medical diagnosis.

The web application is built using **Streamlit**, making it lightweight, interactive, and easy to use without any frontend development.

---

## 🏥 Diseases Covered

| Disease | Description |
|---|---|
| ❤️ Heart Disease | Predicts the likelihood of coronary artery disease or cardiac conditions |
| 🩸 Diabetes | Predicts whether a patient has diabetes based on diagnostic measurements |
| 🫘 Kidney Disease | Predicts the presence of chronic kidney disease (CKD) |

---

## 🛠 Tech Stack

- **Language:** Python 3.x
- **ML Libraries:** Scikit-learn, NumPy, Pandas
- **Web Framework:** Streamlit
- **Model Persistence:** Pickle / Joblib
- **Data Visualization:** Matplotlib / Seaborn *(if applicable)*

---

## 📁 Project Structure

```
disease-prediction/
│
├── app.py                        # Main Streamlit application
│
├── models/
│   ├── heart.pkl   # Trained heart disease model
│   ├── diabetes.pkl        # Trained diabetes model
│   └── kidney.pkl  # Trained kidney disease model
│
├── notebooks/
│   ├── heart_disease.ipynb       # EDA & model training — Heart Disease
│   ├── diabetes.ipynb            # EDA & model training — Diabetes
│   └── kidney_disease.ipynb      # EDA & model training — Kidney Disease
│
├── datasets/
│   ├── heart.csv
│   ├── diabetes.csv
│   └── kidney_disease.csv
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Anushkachhikara/multiplt-disease-prediction.git
cd multiple-disease-prediction
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

Run the Streamlit application:

```bash
streamlit run app.py
```

Then open your browser at `http://localhost:8501` to use the app.

1. Select the disease you want to predict from the sidebar.
2. Enter the required clinical parameters.
3. Click **Predict** to see the result.

---

## 🤖 Model Details

Each disease has its own independently trained ML model. Below is a summary:

| Disease | Algorithm | Dataset Source |
|---|---|---|
| Heart Disease | Logistic Regression / Random Forest | UCI Heart Disease Dataset |
| Diabetes | Support Vector Machine (SVM) | PIMA Indians Diabetes Dataset |
| Kidney Disease | Random Forest / Decision Tree | UCI Chronic Kidney Disease Dataset |

> 

### Model Training Steps

1. Data loading and exploratory data analysis (EDA)
2. Data preprocessing (handling missing values, encoding, scaling)
3. Train-test split (typically 80/20)
4. Model training and hyperparameter tuning
5. Evaluation using accuracy, precision, recall, and F1-score
6. Model serialization using `pickle` or `joblib`

---

## 📋 Input Parameters

### ❤️ Heart Disease
| Parameter | Description |
|---|---|
| Age | Age of the patient |
| Sex | Gender (0 = Female, 1 = Male) |
| Chest Pain Type | Type of chest pain (0–3) |
| Resting Blood Pressure | In mm Hg |
| Serum Cholesterol | In mg/dl |
| Fasting Blood Sugar | > 120 mg/dl (1 = True, 0 = False) |
| Max Heart Rate | Maximum heart rate achieved |
| ... | *(add remaining features)* |

### 🩸 Diabetes
| Parameter | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| Blood Pressure | Diastolic blood pressure (mm Hg) |
| Skin Thickness | Triceps skinfold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body mass index |
| Diabetes Pedigree Function | Likelihood based on family history |
| Age | Age of the patient |

### 🫘 Kidney Disease
| Parameter | Description |
|---|---|
| Age | Age of the patient |
| Blood Pressure | In mm Hg |
| Specific Gravity | Urine specific gravity |
| Albumin | Albumin levels (0–5) |
| Sugar | Sugar levels (0–5) |
| Red Blood Cells | Normal / Abnormal |
| Hemoglobin | In gms |
| ... | *(add remaining features)* |

---

## 🖼 Screenshots

> *<img width="1908" height="925" alt="Screenshot 2025-04-26 111324" src="https://github.com/user-attachments/assets/948bb983-d469-412f-b88e-bcb22b9ed1b5" />
*



⭐ If you found this project helpful, please give it a star!
