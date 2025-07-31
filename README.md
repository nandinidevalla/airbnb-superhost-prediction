# 🏠 Predicting Airbnb Superhost Status with Machine Learning

A machine learning solution to predict Superhost status on Airbnb using historical behavioral and performance metrics.

---

## 💡 Project Summary

As part of Purdue’s *AI for Business Decisions* course, our team built a classification model to predict whether a host would achieve or lose Superhost status. We used datasets from multiple cities and applied robust feature engineering, statistical testing, and model training with scikit-learn.

This project blends **machine learning, feature selection, and model evaluation** with a strong business lens: enabling Airbnb to proactively support top-performing and at-risk hosts.

---

## 🎯 Business Problem

> Can we predict who will become a Superhost — and who is at risk of losing their badge?

**Target Variable:**
- `host_is_superhost_in_period` (binary: 1 = Superhost, 0 = Not Superhost)

**Impact:**
- Retain high-performing hosts through early interventions
- Encourage likely Superhosts with proactive support

---

## 🛠️ Tech Stack

| Tool        | Purpose                          |
|-------------|----------------------------------|
| Python      | Modeling and data processing     |
| pandas      | Data wrangling                   |
| scikit-learn| ML models and evaluation         |
| XGBoost     | Gradient boosting classifier     |
| matplotlib  | Visual analysis                  |
| PowerPoint  | Business presentation            |

---

## 🔍 Approach

- **Data Cleaning & Preprocessing:**
  - Imputed missing values
  - Handled outliers
  - Removed highly correlated features (via correlation + VIF)

- **Feature Selection:**
  - Chi-square for categorical vars
  - Recursive feature elimination

- **Models Tested:**
  - Random Forest ✅ (Best, 97.26% accuracy)
  - XGBoost
  - LightGBM

- **Evaluation:**
  - Precision, Recall, F1-Score
  - ROC-AUC
  - Stratified 10-fold cross-validation

---

## 📊 Key Results

| Metric         | Random Forest |
|----------------|---------------|
| Accuracy       | 97.26%        |
| ROC-AUC        | 99.52%        |
| Precision      | 96.36%        |
| Recall         | 95.42%        |

---

## 📁 Project Structure

data/ # Excel datasets per city
notebooks/ # Jupyter notebook with all modeling code
presentation/ # Final deck used in business presentation
README.md # Project documentation


---

## 📎 Files

- 📊 [Jupyter Notebook](./notebooks/airbnb_superhost_prediction.ipynb)
- 🧠 [Final Deck](./presentation/Predicting-Superhost-Status-A-Data-Driven-Approach.pptx)

---

## 👥 Team Members

- Nandini Priya Devalla
- Krithiga Rajan Sangeetha Rajan
- Shashank Sridhar

---

## 💬 Takeaway

This project showcases how to turn raw behavioral and performance metrics into meaningful predictions. It blends technical skills with product thinking — a key asset for SDEs and ML engineers alike.
