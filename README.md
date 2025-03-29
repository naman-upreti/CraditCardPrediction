# 💳 Credit Card Approval Prediction






An intelligent machine learning system that predicts whether a credit card application will be approved or rejected based on applicant information.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Usage](#-usage)
- [Model Performance](#-model-performance)
- [Project Structure](#-project-structure)
- [Interactive Dashboard](#-interactive-dashboard)
- [Future Improvements](#-future-improvements)
- [License](#-license)

---

## 🔍 Overview

Credit card approval is a crucial process for financial institutions. This project automates decision-making using machine learning techniques to predict whether an application will be approved or rejected based on various applicant attributes.

### ✅ Key Highlights

- High accuracy achieved with **Random Forest** and **Logistic Regression** models.
- Feature engineering, hyperparameter tuning, and performance evaluation included.
- Interactive **Gradio-powered web dashboard** for real-time predictions.

---

## ✨ Features

✔ **Data Preprocessing**: Handles missing values, categorical encoding, and feature scaling.\
✔ **Exploratory Data Analysis**: Visualizes patterns and relationships in the data.\
✔ **Machine Learning Models**: Implements and compares multiple classification algorithms.\
✔ **Hyperparameter Tuning**: Optimizes model performance using Grid Search.\
✔ **Performance Evaluation**: Measures accuracy, precision, recall, and F1-score.\
✔ **Interactive Dashboard**: A user-friendly web-based interface using **Gradio**.

---

## 📊 Dataset

The dataset includes information about credit card applicants with key features:

| **Category**       | **Features**                               |
| ------------------ | ------------------------------------------ |
| **Demographics**   | Age, Gender                                |
| **Financial**      | Debt, Income, Credit Score                 |
| **Employment**     | Years Employed, Employment Status          |
| **Credit History** | Prior Default                              |
| **Personal**       | Marital Status, Education Level, Ethnicity |

- The **target variable** `Approval_Status` indicates whether an application was **approved (+)** or **denied (-)**.

---

## 🛠️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/credit-card-approval-prediction.git
cd credit-card-approval-prediction
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Jupyter Notebook

```bash
jupyter notebook CraditCardPrediction.ipynb
```

---

## 🚀 Usage

Import the trained model and make predictions:

```python
import joblib

# Load the model
model = joblib.load('credit_card_approval_model.pkl')

# Make predictions
model.predict(new_data)
```

---

## 📈 Model Performance

After hyperparameter tuning, the **Random Forest model** achieved:

| **Metric**    | **Score** |
| ------------- | --------- |
| **Accuracy**  | 87.5%     |
| **Precision** | 89.2%     |
| **Recall**    | 85.7%     |
| **F1-Score**  | 87.4%     |
| **AUC-ROC**   | 0.92      |

### 🔍 Confusion Matrix



### 📊 ROC Curve



### 🔥 Feature Importance



---

## 📁 Project Structure

```plaintext
credit-card-approval-prediction/
│
├── CraditCardPrediction.ipynb     # Main Jupyter notebook
├── requirements.txt               # Required Python packages
├── credit_card_approval_model.pkl # Saved model
├── README.md                      # Project documentation
│
└── datasets/                      # Data directory
    └── cc_approvals_cleaned.csv   # Cleaned dataset
```

---

## 🌐 Interactive Dashboard

The project includes an **interactive Gradio dashboard** allowing users to:
✅ Input applicant details & get real-time predictions.\
✅ Explore model performance metrics & feature importance.\
✅ Understand how different factors influence approval decisions.

---

## 🔮 Future Improvements

🔹 Implement additional machine learning models for comparison.\
🔹 Improve explainability with **SHAP values** & model interpretability.\
🔹 Deploy the model as a full-fledged web application.\
🔹 Integrate **real-time data updates** from financial APIs.

---
#   C r a d i t C a r d P r e d i c t i o n  
 