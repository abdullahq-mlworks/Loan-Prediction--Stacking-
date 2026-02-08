## 📌 Project Overview
This project focuses on predicting loan approval status using machine learning techniques.  
A **stacking ensemble model** is implemented by combining multiple base learners to improve prediction performance.

---

## 📁 Project Folder Structure
Loan-Prediction-(Stacking)/
- Loan Prediction.ipynb
- loan_data.csv
- requirements.txt
- README.md

---


## The project uses:
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier  
as base models, and a Logistic Regression model as the **meta-learner**.

Evaluation is done using **ROC-AUC Score**, which is suitable for binary classification problems.

---

## 📊 Dataset
**File:** `loan_data.csv`
The dataset contains applicant information such as:
- Gender
- Marital Status
- Dependents
- Education
- Employment Status
- Applicant Income
- Loan Amount Term
- Credit History  
and the target variable **Loan_Status** (Approved / Not Approved).

---

## ⚙️ Data Preprocessing
- Missing values handled using:
  - **Mode** for categorical features
  - **Median** for numerical features
- Categorical variables encoded using **One-Hot Encoding**
- Target variable (`Loan_Status`) mapped to binary values:
  - Y → 1
  - N → 0
- Feature scaling applied **only for Logistic Regression**

---

## 🤖 Models Used
### Base Models
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### Meta Model
- Logistic Regression

The predictions from base models are stacked and passed to the meta-model.

---

## 📈 Model Evaluation
Evaluation Metric:
- **ROC-AUC Score**

Results include:
- Individual ROC-AUC scores for each base model
- Final ROC-AUC score for the stacking ensemble model

---

## 🛠 Technologies & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost

---

## ▶️ How to Run
1. Clone the repository
git clone https://github.com/abdullahq-mlworks/Loan-Prediction--Stacking-.git

---

2. Navigate to project directory
cd Loan-Prediction-(Stacking)
3. Install dependencies
pip install -r requirements.txt
4. Run the notebook
jupyter notebook "Loan Prediction.ipynb"

---

## 🎯 Key Highlights

- Proper handling of missing values
- Feature scaling applied selectively
- Advanced ensemble technique (Stacking)
- ROC-AUC based evaluation
- Clean and modular ML pipeline

---