# 🚢 Titanic Survival Prediction - Machine Learning Project

## 📌 Project Overview
This project uses the famous **Titanic dataset** from Kaggle to predict passenger survival using different Machine Learning models.  
The goal is to apply **data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and evaluation**.

---

## 📊 Dataset
- **Source**: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)  
- **Files used**:  
  - `tested.csv` → Testing dataset  

**Target variable**: `Survived`  
- `0` → Passenger did not survive  
- `1` → Passenger survived  

---

## ⚙️ Methods & Workflow
1. **Data Cleaning & Preprocessing**  
   - Handled missing values (`Age`, `Fare`, `Embarked`)  
   - Converted categorical features using **one-hot encoding**  
   - Removed duplicates  

2. **Exploratory Data Analysis (EDA)**  
   - Used **Pandas & NumPy** for statistics  
   - Visualized distributions with **Matplotlib & Seaborn**  
   - Created interactive plots using **Plotly**  

3. **Feature Engineering**  
   - Split data into features (X) and target (y)  
   - Scaled numerical features  
   - Train-test split  

4. **Model Training**  
   - K-Nearest Neighbors (KNN)  
   - Decision Tree Classifier  
   - Random Forest Classifier  

5. **Hyperparameter Tuning**  
   - Used **RandomizedSearchCV** to optimize parameters  

6. **Model Evaluation**  
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix  
   - ROC Curve  

---

## 🏆 Results
- **Best Model**: Random Forest Classifier  
- **Reason**: Achieved highest accuracy and balanced performance across precision, recall, and F1-score.  
- **Most Important Features**:
  - Passenger Class (`Pclass`)  
  - Sex (`female`)  
  - Age  
  - Fare
    

---
Titanic-Survival-Prediction/
│
├── README.md
├── Titanic_ML_Assignment.ipynb
├── requirements.txt
│
├── data/
│ ├── tested.csv
│
├── plots/
│ ├── survival_count.png
│ ├── gender_survival.png
│ ├── age_distribution.png
│ └── feature_importance.png
│
└── html_plots/
└── titanic_age_fare_scatter.html


---

## 📦 Requirements
Install dependencies with:
```bash
pip install -r requirements.txt
**Dependencies**:

pandas

numpy

matplotlib

seaborn

scikit-learn

plotly

Random Forest performed best due to handling of non-linear relationships and feature importance.

Passenger Class, Sex, and Age were the strongest predictors of survival.

Hyperparameter tuning improved performance compared to default models.


