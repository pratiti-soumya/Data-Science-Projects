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

## 🔗 Related Blog Post

📖 _ Medium_: _“Predicting Developer Salaries with Machine Learning”_ (https://medium.com/@pratitisoumya/predicting-developer-salaries-with-machine-learning-f2d81579af86)

