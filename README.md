# Loan Approval Prediction System
![Uploading image.png…]()

## 📋 Project Overview

This project analyzes a loan dataset and builds classification models to predict loan approval status. The best performing model achieved **87.1% accuracy** using Support Vector Classifier (SVC) with hyperparameter tuning.

**Key Highlights:**
- Comprehensive **EDA** and data cleaning
- Handled missing values and categorical encoding
- Implemented **KNN** and **SVC** with GridSearchCV
- Model saved for deployment (`model.pkl`)
- 
## 📊 Dataset

- **Source**: `loan_data.csv`
- **Rows**: 381
- **Features**: 13 columns
- **Target Variable**: `Loan_Status` (Y / N)

### Features:
- `Loan_ID`, `Gender`, `Married`, `Dependents`
- `Education`, `Self_Employed`
- `ApplicantIncome`, `CoapplicantIncome`
- `LoanAmount`, `Loan_Amount_Term`
- `Credit_History`, `Property_Area`

## 🛠 Data Preprocessing

- Removed null values (dropped rows with missing data)
- Verified no duplicate entries
- Encoded categorical variables
- Feature scaling using StandardScaler

## 📈 Exploratory Data Analysis

- Analyzed applicant income distribution
- Visualized relationships between features and loan status
- Explored credit history impact on approval

---

## 🤖 Models Implemented

### 1. K-Nearest Neighbors (KNN)
- Hyperparameter tuning using GridSearchCV
- Best Parameters: `n_neighbors=8`, `weights=distance`
- **Accuracy**: 84.95%

### 2. Support Vector Classifier (SVC)
- Hyperparameter tuning using GridSearchCV
- Best Parameters: `C=0.01`, `kernel=linear`
- **Accuracy**: **87.10%** (Best Model)

## 🚀 Results

| Model | Accuracy    | Best Parameters                  |
|-------|-------------|----------------------------------|
| KNN   | 84.95%      | n_neighbors=8, weights=distance |
| **SVC**   | **87.10%**  | C=0.01, kernel=linear           |

---

## 🧪 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Animesh789486/loan-approval-prediction.git
   cd loan-approval-prediction
