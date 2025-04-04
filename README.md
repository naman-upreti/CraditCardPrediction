---

# 💳 **Credit Card Approval Prediction**  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange)  
![Gradio](https://img.shields.io/badge/Gradio-3.40.1-green)  
![License](https://img.shields.io/badge/License-MIT-yellow)  

An intelligent **machine learning** system that predicts whether a **credit card application** will be **approved** or **rejected** based on applicant information.  

<p align="center">
  <img src="CraditCardPrediction_confusion_matrix.png" width="30%" />
  <img src="CraditCardPrediction_roc_curve.png" width="30%" /> 
  <img src="CraditCardPrediction_feature_importance.png" width="30%" />
</p>

---

## 📋 **Table of Contents**  

- [🔍 Overview](#-overview)  
- [✨ Features](#-features)  
- [📊 Dataset](#-dataset)  
- [🛠️ Installation](#-installation)  
- [🚀 Usage](#-usage)  
- [📈 Model Performance](#-model-performance)  
- [📁 Project Structure](#-project-structure)  
- [🌐 Interactive Dashboard](#-interactive-dashboard)  
- [🔮 Future Improvements](#-future-improvements)  
- [📜 License](#-license)  

---

## 🔍 **Overview**  

Credit card approval is a critical process for **financial institutions**. This project **automates** the decision-making process using **machine learning techniques** to predict whether an application will be **approved** or **rejected**.  

The system achieves **high accuracy** through:  
✅ Data Preprocessing  
✅ Feature Engineering  
✅ Model Optimization with **Random Forest & Logistic Regression**  

---

## ✨ **Features**  

✔️ **Data Preprocessing**: Handles missing values, categorical encoding, and feature scaling  
✔️ **Exploratory Data Analysis (EDA)**: Visualizes patterns and relationships in the data  
✔️ **Machine Learning Models**: Implements and compares multiple classification algorithms  
✔️ **Hyperparameter Tuning**: Optimizes model performance using Grid Search  
✔️ **Performance Evaluation**: Measures accuracy, precision, recall, and F1-score  
✔️ **Interactive Web Dashboard**: A user-friendly interface for making predictions  

---

## 📊 **Dataset**  

The dataset includes **credit card applicants'** information such as:  

| **Category**    | **Features**                  |  
|---------------|------------------------------|  
| **Demographics**  | Age, Gender |  
| **Financial**  | Debt, Income, Credit Score |  
| **Employment**  | Years Employed, Employment Status |  
| **Credit History**  | Prior Default |  
| **Personal Details**  | Marital Status, Education Level, Ethnicity |  

🔹 **Target Variable**: `"Approval_Status"` ( `+` = Approved, `-` = Denied )  

📂 **Dataset File**: [`cc_approvals_cleaned.csv`](datasets/cc_approvals_cleaned.csv)  

---

## 🛠️ **Installation**  

### 1️⃣ Clone this Repository  
```bash
git clone https://github.com/yourusername/credit-card-approval-prediction.git
cd credit-card-approval-prediction
```

### 2️⃣ Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Run Jupyter Notebook  
```bash
jupyter notebook CraditCardPrediction.ipynb
```

---

## 🚀 **Usage**  

```python
import joblib

# Load the trained model
model = joblib.load('credit_card_approval_model.pkl')

# Make predictions
prediction = model.predict(new_data)
print(prediction)
```

---

## 📈 **Model Performance**  

The **Random Forest model** achieved **excellent performance** after hyperparameter tuning:  

📊 **Performance Metrics**  

| **Metric**  | **Score**  |  
|------------|-----------|  
| **Accuracy**  | 87.5% |  
| **Precision**  | 89.2% |  
| **Recall**  | 85.7% |  
| **F1-Score**  | 87.4% |  
| **AUC (ROC Curve)**  | 0.92 |  

### 🏆 **Key Performance Visualizations**  
📌 **Confusion Matrix**  
📌 **ROC Curve**  
📌 **Feature Importance**  

---

## 📁 **Project Structure**  

```plaintext
credit-card-approval-prediction/
│
├── CraditCardPrediction.ipynb     # Jupyter Notebook (Main Script)
├── requirements.txt               # Required Python Packages
├── credit_card_approval_model.pkl # Trained ML Model
├── README.md                      # Project Documentation
│
└── datasets/                      # Data Directory
    └── cc_approvals_cleaned.csv   # Cleaned Dataset
```

---

## 🌐 **Interactive Dashboard**  

🚀 This project includes a **web-based dashboard** using **Gradio** that allows users to:  

🔹 **View model performance metrics and visualizations**  
🔹 **Input applicant details and get instant predictions**  
🔹 **Explore feature importance and model insights**  

---

## 🔮 **Future Improvements**  

🔸 Implement additional **machine learning algorithms** for comparison  
🔸 Add **more advanced feature engineering techniques**  
🔸 Develop a **comprehensive explainability module**  
🔸 Deploy the model as a **full-stack web application**  
🔸 Incorporate **real-time data updates**  
---
