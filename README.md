# 📊 Customer Churn Prediction Using Machine Learning

This project aims to predict whether a customer will churn (leave the company) based on various features such as electricity usage, contract history, pricing variations, and more.

---

## 🚀 Project Workflow

1. **Data Cleaning & Preprocessing**  
   - Removed irrelevant columns (`id`, `Unnamed: 0`)
   - Converted date columns to datetime and extracted useful features
   - Engineered new features like price trends, average prices, estimated profit
   - Removed or encoded categorical variables

2. **Exploratory Data Analysis (EDA)**  
   - Visualized churn distribution, consumption trends, pricing correlations
   - Detected imbalance in churn classes

3. **Feature Engineering**  
   - Added columns like:
     - `est_profit` = `cons_12m` × `net_margin`
     - Price variance trends (6-month vs yearly)
     - Date parts from `date_modif_prod`

4. **Model Building**  
   - Used `RandomForestClassifier` for binary classification
   - Accuracy, confusion matrix, and classification report were evaluated

---

## 📁 Dataset Overview

- `clean_data_after_eda.csv`: Cleaned and processed data after EDA
- `data_for_predictions.csv`: Final dataset used for model training/testing

---

## 📈 Results

- **Model Used:** Random Forest
- **Evaluation Metrics:**
  - Accuracy: ~XX%
  - Precision / Recall / F1-Score: Reported using `classification_report`
  - Confusion Matrix: Heatmap plotted

---

## 🔬 Task 1: Hypothesis Testing

We performed statistical hypothesis testing to validate our assumptions (see `Task_1_Hypothesis.ipynb`).

---

## 📦 Libraries Used

- Python 3.x
- pandas, numpy, seaborn, matplotlib
- scikit-learn

---

## 🧠 Future Scope

- Try advanced models (XGBoost, LightGBM)
- Perform hyperparameter tuning
- Handle class imbalance using SMOTE
- Feature selection using importance metrics

---

## 👨‍💻 Author

- **Your Name** - [GitHub](https://github.com/yourusername)

