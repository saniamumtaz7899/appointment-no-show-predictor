# 📅 Appointment No-Show Predictor

This project predicts which patients are likely to **miss their medical appointments** using historical, demographic, and scheduling data. It also suggests appropriate **intervention strategies** like SMS reminders or phone calls to reduce no-shows.

## 🧠 Problem Statement

Healthcare systems face revenue and resource losses due to patients not attending scheduled appointments. The goal is to:
- Predict the likelihood of a patient **not showing up**
- Suggest appropriate **retention strategies**

## ✅ Features & Deliverables

| Component               | Description                                               |
|------------------------|-----------------------------------------------------------|
| 🔍 Data Source          | Kaggle Appointment Data (Brazil, 2016)                    |
| 🔬 ML Model             | XGBoost with SMOTE oversampling for class imbalance       |
| 🧾 Features Used        | Age, Gender, Neighbourhood, Chronic conditions, etc.      |
| 🎯 Target               | No-show (1 = did not attend, 0 = attended)                |
| 📊 Risk Score           | Predicted probability of missing the appointment          |
| 📣 Intervention Logic   | Risk-based action: SMS / Call / Reschedule                |
| 🖥️ Gradio UI            | Simple web interface to test predictions interactively     |
| 📁 Output File          | `Appointment_NoShow_Risk_Predictions.csv`                |

---

## 🛠️ Tech Stack

- Python 🐍
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- SMOTE (imbalanced-learn)
- Gradio (for live UI)
- Google Colab

## 🚀 How to Use

### 🔗 Option 1: Run in Google Colab
1. Upload the dataset ZIP file (Kaggle 2016 appointment dataset)
2. Run all cells from top to bottom
3. Download the final predictions CSV
4. Use the Gradio UI for live patient predictions

### 🔗 Option 2: Run Locally
```bash
git clone https://github.com/your-username/appointment-no-show-predictor.git
cd appointment-no-show-predictor
pip install -r requirements.txt
python app.py
