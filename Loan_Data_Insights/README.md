# 📊 Loan Data Insights – Exploratory & Explanatory Analysis

This project explores loan data from [Prosper Marketplace](https://www.prosper.com/) to identify patterns influencing borrower interest rates. It is structured into two key phases: an exploratory data analysis (EDA) and a refined explanatory presentation.

---

## 🗂️ Project Structure

### 🔍 1. Exploratory Analysis: `Loan_Data_EDA.ipynb`
A deep dive into the Prosper loan dataset with a focus on:
- **Data Cleaning**: 
  - Dropped irrelevant columns
  - Handled missing values (dropped or imputed where appropriate)
  - Converted date fields to datetime format
- **Univariate Analysis**:
  - Explored the distributions of borrower interest rate, loan status, and loan amounts
- **Bivariate Analysis**:
  - Scatter plot: BorrowerRate vs. LoanAmount
  - Box plot: BorrowerRate vs. EmploymentStatus
  - Clustered bar chart: LoanStatus vs. IncomeRange
- **Multivariate Analysis**:
  - Regression plot using FacetGrid (ProsperScore × EmploymentStatus × BorrowerRate)
  - Correlation heatmap of numeric variables
  - PairGrid of key numeric variables

👉 Cleaned data saved to `prosperdata_clean.csv` for use in the explanatory notebook.

---

### 📈 2. Explanatory Presentation: `Loan_Data_Insights_Presentation.ipynb`
Refined narrative visualizations answering 3 central questions:

#### Visualization 1: Line Plot  
**Q**: How do ProsperScores and Employment Status influence interest rates?  
**A**: Higher ProsperScores are associated with lower rates across all employment categories.

#### Visualization 2: Box Plot  
**Q**: Does employment status affect the range of interest rates borrowers receive?  
**A**: Yes, but it's a secondary factor. Self-employed and unemployed individuals tend to have more rate variability.

#### Visualization 3: Heatmap  
**Q**: Does income range correlate with interest rates?  
**A**: Very little. The correlation heatmap shows a near-zero relationship.

---

## 🧾 Summary of Findings

- **Credit scores** (via ProsperScore) have a strong and consistent impact on borrower rates.
- **Employment status** has a visible but secondary influence.
- **Income range** shows little to no direct correlation with interest rates.

---

## 🛠️ Tools Used
- Python (pandas, numpy)
- Seaborn, Matplotlib
- Jupyter Notebook

---

## 📁 Dataset
- `prosperLoanData.csv`: Original dataset with 113,000+ loan records
- `prosperdata_clean.csv`: Cleaned and subsetted dataset used for visualization

---

## 🔗 Credits
Project developed as part of Udacity Data Science Nanodegree Program to demonstrate EDA and explanatory storytelling skills.

