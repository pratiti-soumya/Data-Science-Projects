# 🧠 Predicting Developer Salaries  
Using the 2024 Stack Overflow Developer Survey

---

## 📌 Overview

This project explores the challenge of predicting a developer's salary (`ConvertedCompYearly`) using data from the 2024 Stack Overflow Developer Survey. The analysis follows an end-to-end data science pipeline:

- Data cleaning & preprocessing  
- Exploratory data analysis (EDA)  
- Regression modeling (Linear, Decision Tree, Random Forest)  
- Feature selection & hyperparameter tuning  
- Model interpretation using SHAP values  

---

## ❓ Business Questions & Insights

### 1. **Does education level significantly affect a developer’s salary?**
**Insight:** Yes — developers with higher degrees (Master’s, PhD, Professional) generally earn more. However, there are notable exceptions where developers with lower formal education (e.g. self-taught) still report high salaries.

---

### 2. **Is there a strong correlation between years of experience and salary?**
**Insight:** A weak positive trend exists, but it's not linear. Some developers with very little experience report high salaries, and vice versa. This suggests that experience alone is not a strong predictor.

---

### 3. **Which countries are associated with higher average salaries?**
**Insight:** The United States consistently ranks at the top, followed by certain countries in Europe. Country was the most influential feature in the SHAP analysis.

---

### 4. **What developer roles (DevType) are linked to higher compensation?**
**Insight:** Executive-level roles (e.g. C-Suite, VP, Director) and specialized roles (e.g. Project Manager) had higher predicted salaries compared to general developer titles.

---

### 5. **Which features have the highest predictive power for salary?**
**Insight:** Based on SHAP values and feature importance from Random Forest, the top predictors were:
- `Country`
- `YearsCode`
- `DevType`
- `EdLevel`

---

## 📊 Dataset

- Source: [Stack Overflow Developer Survey 2024](https://insights.stackoverflow.com/survey)
- Target: `ConvertedCompYearly` (Annual salary in USD)

> ⚠️ Dataset is excluded from this repo due to GitHub’s file size limits. Please download it from the official source above.

---

## 🔍 Final Model Performance (Random Forest Regressor on top 10 features)

- Train R²: 0.188  
- Test R²: 0.045  
- Test RMSE: ~$113,000

---

## 📈 SHAP Feature Insights

The most important features driving salary predictions:

1. Country: United States  
2. Years of Experience  
3. DevType: Executive roles  
4. Education Level  
5. Country: Ukraine, South Africa

## 🧾 Author

Made by [Pratiti Soumya](https://github.com/pratiti-soumya)  
📫 Reach me via GitHub or LinkedIn.

---


📖 _ Medium_: _“Predicting Developer Salaries with Machine Learning”_ (https://medium.com/@pratitisoumya/predicting-developer-salaries-with-machine-learning-f2d81579af86)

