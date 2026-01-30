# Heart Disease Prediction using Machine Learning

##  Project Overview
This project focuses on predicting the presence of heart disease using machine learning techniques.
A Random Forest classifier was trained and tuned to improve prediction performance.

The project is developed and executed entirely in **Jupyter Notebook**, with an interactive user interface implemented using **ipywidgets** to allow dynamic user input and real-time predictions.

---

##  Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Jupyter Notebook
- ipywidgets

---

##  Dataset
The dataset contains medical attributes such as:
- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise-induced Angina
- Oldpeak
- ST Slope

Target variable:
- **HeartDisease** (0 = No, 1 = Yes)

---

##  Model Details
- Algorithm: **Random Forest Classifier**
- Preprocessing:
  - Categorical features encoded using **OneHotEncoder**
  - Numerical features passed directly
  - Implemented using **ColumnTransformer**
- Model Pipeline used to prevent data leakage
- Stratified train-test split

---

## 🔧 Hyperparameter Tuning
- **GridSearchCV** was used to tune Random Forest hyperparameters
- Optimization metric: **ROC-AUC**
- Cross-validation applied to improve generalization

This tuning significantly improved model performance compared to the baseline model.

---

##  Model Performance
The tuned Random Forest model achieved:
- Accuracy ≈ **89%**
- Improved Precision, Recall, and F1-score
- Better ROC-AUC compared to baseline

---

##  User Interface
An interactive UI is implemented **inside the Jupyter Notebook** using **ipywidgets**.
Users can input medical values dynamically and obtain real-time predictions.

---

##  How to Run the Project
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
