# Data Science Projects Portfolio

Welcome to my personal portfolio of data science projects!

I regularly add new projects as I explore different datasets, apply advanced techniques, and continue growing my skills as a data scientist.

## 📂 Projects

### 1. Investigate a Dataset – TMDb Movie Data  
I analyzed data from The Movie Database (TMDb) to explore patterns in movie popularity, revenue, and runtime.

📄 [View Notebook](./Investigate_a_Dataset.ipynb)

#### Key Highlights:
I cleaned and filtered the movie metadata to handle missing and irrelevant values  
I explored trends over time using aggregation and grouping  
I visualized relationships between popularity, runtime, and revenue  
I used correlation and summary statistics to answer four data-driven questions

#### Findings:
Movies released in the 2000s and beyond tend to have higher popularity scores  
There was no strong relationship between runtime and revenue, but very long or very short movies tend to earn less  
Popular movies generally have high vote counts and strong marketing visibility

---

### 2. Keyword Search vs Sales Analysis  
I explored the relationship between online search trends and product sales using Kaggle sales data and real-time search data from the Google Trends API.

📄 [View Notebook](./Keyword_Search_vs_Sales_Analysis.ipynb)

#### Key Highlights:
I pulled Google Trends data for the keyword "laptops"  
I combined that with weekly sales data to understand how search interest aligns with sales activity  
I examined seasonal trends and aggregated monthly averages  
I used visualizations to explore two key research questions

#### Findings:
Does online search interest in "laptops" affect sales?
- Yes, especially in the technology category, where spikes in search interest were followed by higher sales.

Do certain months have higher search interest and sales?
- Yes, Q4 (Oct–Dec) consistently showed higher interest and increased sales volume.

Which categories show alignment with search interest?
- Technology had the strongest correlation, followed by occasional spikes in Office Supplies.

---

### 3. Loan Data Visualization with Matplotlib and Seaborn 💵📊  
I conducted an exploratory and explanatory analysis of Prosper loan data to understand how borrower interest rates vary with credit score, employment status, and income.

📁 [Project Folder](./Loan_Data_Insights/)

#### Files:
`Loan_Data_EDA.ipynb` – My exploratory notebook with univariate, bivariate, and multivariate analysis  
`Loan_Data_Insights_Presentation.ipynb` – My explanatory notebook with refined visualizations and key takeaways  
`prosperLoanData.csv`, `prosperdata_final.csv` – Raw and cleaned versions of the dataset

#### Key Highlights:
I cleaned and filtered the 81-column dataset, managed missing values, and selected relevant features  
I converted date columns to proper datetime format  
I visualized loan status distribution, interest rates, and loan amounts  
I investigated relationships such as:
- Interest rate versus credit score by employment status
- Interest rate versus employment status by loan status
- A correlation heatmap showing weak correlation between income and borrower rates

#### Findings:
Credit scores have a strong influence on interest rates, with higher scores leading to lower borrowing costs  
Unemployed and self-employed individuals generally receive loans with higher interest rates  
Income does not significantly affect the borrower rate, despite assumptions to the contrary

---

### 4. Stack Overflow Salary Prediction 💼📈  
I built a regression model using the Stack Overflow 2024 Developer Survey to predict annual salaries based on developer experience, education, and job profile.

📄 [View Notebook](./stackoverflow_salary_prediction.ipynb)

#### Key Highlights:
I selected and cleaned relevant features like education, country, years of experience, and employment  
I handled missing values and applied one-hot encoding to categorical features  
I explored relationships between salary and key variables using histograms, bar plots, and regression plots  
I built and evaluated multiple regression models including Linear Regression, Decision Tree, and Random Forest  
I improved model performance by selecting the top 10 most important features  
I used SHAP values to explain my final model’s predictions and ensure transparency

#### Findings:
Salaries are heavily skewed, and Random Forest models handle this better than linear models  
Key predictors include years of experience, country, education level, and job type  
Using only the top 10 features led to a better-performing model with lower RMSE and improved R² scores  
SHAP analysis confirmed that experience and job type consistently influence salary the most

---

## 💻 Tech Stack
Python (Jupyter Notebook)  
pandas, numpy  
matplotlib, seaborn  
scikit-learn, SHAP, pytrends
