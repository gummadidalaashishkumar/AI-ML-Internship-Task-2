# AI-ML-Internship-Task-2
finding missing values and analysing 
# No-Show Medical Appointment Prediction 🏥📊

This project focuses on analyzing, training, and testing a machine learning model to predict whether a patient will **miss a medical appointment** using historical healthcare data.

---

## 📌 Project Overview

Hospitals face losses and inefficiencies when patients do not show up for appointments.  
This project uses **Exploratory Data Analysis (EDA)** and **Machine Learning** to predict **No-Show appointments** in advance.

---

## 📂 Dataset Information

- **Dataset Name:** No-Show Appointments
- **File:** `noshowappointments.csv`
- **Rows:** 110,000+
- **Target Variable:** `No-show`
  - `0` → Patient attended
  - `1` → Patient did not attend

### Key Features
- Gender
- Age
- Scholarship
- Hypertension
- Diabetes
- Alcoholism
- Handicap
- SMS_received
- WaitingDays (engineered feature)

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to understand:
- Class imbalance in `No-show`
- Age distribution of patients
- Gender distribution
- Impact of SMS reminders on attendance

### Insights:
- Dataset is **imbalanced**
- SMS reminders reduce no-show rate
- Longer waiting days increase no-shows
- Age is a significant factor

---

## 🛠️ Data Preprocessing Steps

1. Checked and confirmed no missing values
2. Encoded categorical variables:
   - Gender (M/F → 0/1)
   - No-show (No/Yes → 0/1)
3. Converted date columns to datetime
4. Created `WaitingDays` feature
5. Removed irrelevant columns

---

## 🤖 Machine Learning Model

- **Algorithm:** Logistic Regression
- **Problem Type:** Binary Classification
- **Train-Test Split:** 80% training, 20% testing

---

## 📊 Model Evaluation

Evaluation metrics used:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### Results:
- ~80% accuracy
- Better at predicting attendance
- No-show prediction affected by class imbalance

---

## 🚀 How to Run the Project

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/no-show-prediction.git
