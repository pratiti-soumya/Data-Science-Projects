# 🧠 Data Science Projects Portfolio

Welcome to my personal portfolio of data science projects!

More projects will be added regularly as I explore new datasets, apply advanced techniques, and build toward more complex models.

---

## 📂 Projects

### 1. Investigate a Dataset – TMDb Movie Data
Analyze data from The Movie Database (TMDb) to explore patterns in movie popularity, revenue, and runtime.

📄 [View Notebook](./Investigate_a_Dataset.ipynb)

#### Key Highlights:
- Cleaned and filtered movie metadata for missing and irrelevant values
- Explored trends over time using aggregation and grouping
- Visualized relationships between popularity, runtime, and revenue
- Used correlation and summary statistics to answer 4 data-driven questions

---

### 2. Keyword Search vs Sales Analysis 📈  
Explored the relationship between online search trends and product sales using Kaggle sales data and **Google Trends API** (via `pytrends`).

📄 [View Notebook](./Keyword_Search_vs_Sales_Analysis.ipynb)

#### Key Highlights:
- Pulled real-time trend data from **Google Trends API** for the keyword **"laptops"**
- Combined it with weekly product sales data from **Kaggle**
- Investigated whether spikes in search interest align with sales patterns across categories
- Explored **seasonal trends** by aggregating monthly averages
- Created visualizations to support two research questions

---

### 3. Loan Data Visualization with Matplotlib & Seaborn 💵📊  
An in-depth exploratory and explanatory analysis of Prosper loan data, focused on understanding how credit score, employment status, and income level influence borrower interest rates.

📁 [Project Folder](./Loan_Data_Insights/)

#### Files:
- `Loan_Data_EDA.ipynb`: Univariate, bivariate, and multivariate exploratory analysis using histograms, scatter plots, facet grids, and correlation heatmaps
- `Loan_Data_Insights_Presentation.ipynb`: A refined explanatory notebook presenting 3 key visualizations supported by clean, narrative insights
- `prosperLoanData.csv`, `prosperdata_final.csv`: Raw and cleaned versions of the Prosper dataset

#### Key Highlights:
- Cleaned 81-column dataset, handled missing values strategically and selected meaningful features
- Converted date fields to datetime format for accurate parsing
- Visualized the distribution of loan status, interest rates, and loan amounts
- Investigated key relationships:
  - **Interest Rate vs Credit Score by Employment Status** (line plot)
  - **Interest Rate vs Employment Status by Loan Status** (clustered bar chart)
  - **Correlation Heatmap** showing weak correlation between income and borrower rate
- **Findings Summary**:
  - Credit scores have a strong impact on interest rates
  - Employment status plays a secondary but visible role
  - Income range shows very little direct influence on interest rates

---

## 💻 Tech Stack
- Python (Jupyter Notebook)
- pandas, numpy
- matplotlib, seaborn
