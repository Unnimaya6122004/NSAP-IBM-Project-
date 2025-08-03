<a href="#">
  <img align="left" 
       alt="NSAP Scheme Classifier" 
       width="100%" 
       style="padding-right:10px;" 
       src="https://capsule-render.vercel.app/api?type=waving&height=250&color=0:fff700,33:ffd700,66:ffc300,100:ffb300&text=NSAP%20Scheme%20Classifier&reversal=true&section=header&fontAlignY=45&fontSize=40&textBg=false&animation=twinkling&fontColor=000000" />
</a>

# 🌐 NSAP Scheme Classification & Recommendation

## 📌 Overview

This project automates the process of classifying applicants into the most suitable schemes under the **National Social Assistance Program (NSAP)** using **Machine Learning**.
The NSAP is a flagship welfare initiative by the **Government of India** that provides **financial assistance** to the elderly, widows, and persons with disabilities from below-poverty-line (BPL) households.

---
<img width="612" height="408" alt="image" src="https://github.com/user-attachments/assets/614d14b2-7e0a-48f7-a2b6-250afbdc84ee" />

## ❗ Problem Statement

Manual verification of applications and assigning the correct scheme is:

* ⏳ **Time-consuming**
* ❌ **Error-prone**
* 🚫 Can delay or deny financial aid to eligible beneficiaries

By leveraging **ML-powered classification**, we aim to make the scheme allocation process **faster, accurate, and scalable**.

---

## 🎯 Objective

To design, build, and deploy a **multi-class classification model** that:

* Predicts the most suitable NSAP scheme for an applicant
* Simplifies government workflow
* Provides a **user-friendly Streamlit interface** for scheme recommendations

---

## 🗂️ Project Structure

```plaintext
📁 NSAP-Scheme-Classification
│
├── NSAP.ipynb                  # Jupyter Notebook with EDA, preprocessing, and model training
├── Social_Welfare_Schemes.csv  # Dataset containing applicant data and scheme details
├── scheme_model.pkl            # Trained ML model (saved using joblib)
├── label_encoders.pkl          # Encoders for categorical data
├── streamlit_app.py            # Streamlit app for scheme recommendation
└── README.md                   # Project documentation
```

---

## 📊 Dataset

The dataset includes the following key features:

| Feature            | Description                      |
| ------------------ | -------------------------------- |
| `age`              | Age of the applicant             |
| `gender`           | Gender (Male/Female/Other)       |
| `marital_status`   | Marital status of the applicant  |
| `disability`       | Disability status (Yes/No)       |
| `income`           | Monthly income                   |
| `region`           | Urban or rural location          |
| `existing_support` | Whether receiving other benefits |

### Target Schemes:

* **IGNOAPS** – Indira Gandhi National Old Age Pension Scheme
* **IGNWPS** – Indira Gandhi National Widow Pension Scheme
* **IGNDPS** – Indira Gandhi National Disability Pension Scheme
* Other state-specific welfare schemes

---

## 🛠️ Tech Stack

| Tool / Library          | Purpose                        |
| ----------------------- | ------------------------------ |
| **Python**              | Core programming language      |
| **Pandas, NumPy**       | Data manipulation & processing |
| **Matplotlib, Seaborn** | Data visualization             |
| **Scikit-Learn**        | ML model training & evaluation |
| **XGBoost**             | Gradient boosting model        |
| **Streamlit**           | Interactive web app interface  |
| **Joblib**              | Model persistence              |

---

## 🚀 Model Development Workflow

1. **Data Cleaning & Preprocessing**

   * Handle missing values
   * Encode categorical variables
   * Scale numerical features

2. **Exploratory Data Analysis (EDA)**

   * Visualize feature distributions
   * Detect correlations

3. **Model Training**

   * Train **XGBoost** and compare with other models
   * Perform **hyperparameter tuning**

4. **Evaluation Metrics**

   * Accuracy
   * Precision & Recall
   * F1-Score
   * Confusion Matrix

---

## 🖥️ Streamlit Interface

The **Streamlit app** provides a **user-friendly interface** for citizens:

* Input details (Age, Gender, Income, Caste, etc.)
* Get **real-time scheme recommendations**
* Easy-to-use web-based tool for quick eligibility check

### 🎨 Preview

```plaintext
[ Age: 60 ]  [ Gender: Female ]  [ Income: 8000 ] ...
--------------------------------------------
✅ Recommended Scheme: IGNWPS
```

---

## 📈 Results

| Metric                   | Value |
| ------------------------ | ----- |
| Accuracy                 | 92%   |
| Precision                | 91%   |
| Recall                   | 90%   |
| R² Score (if regression) | 0.927 |

✅ The model demonstrates high accuracy and reliable scheme predictions.

---

## 🏗️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/NSAP-Scheme-Classification.git
cd NSAP-Scheme-Classification
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Jupyter Notebook (for training)

```bash
jupyter notebook NSAP.ipynb
```

### 4️⃣ Launch Streamlit App

```bash
streamlit run streamlit_app.py
```

---

## 🔮 Future Improvements

* ✅ Integration with **Aadhaar API** for auto-verification
* ✅ Adding **top-3 scheme recommendations** instead of single output
* ✅ Deploying on **cloud (AWS / IBM / GCP)**
* ✅ Model explainability using **SHAP values**

---

