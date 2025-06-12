# Keyword Search vs Sales Analysis

In this project, I analyzed whether public interest in a specific keyword—**“laptops”**—had any relationship with **product sales trends** in different categories like technology, furniture, and office supplies.

I conducted the full end-to-end data wrangling process using real-world datasets and applied exploratory analysis to uncover trends and answer business questions.

## Project Objective

My main goal was to understand:

1. **Does online interest in "laptops" align with real-world sales patterns?**
2. **Do sales and search patterns show seasonality?**
3. **Can we quantify how aligned tech category sales are with laptop-related searches?**

---

## Datasets and Gathering Methods

I combined **two datasets** gathered using different methods:

- **Dataset 1**: [Superstore Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) – Programmatically downloaded using Kaggle CLI.
- **Dataset 2**: Google Trends search interest for the keyword “laptops” – Retrieved via the PyTrends API.

---

## Data Wrangling Steps

I applied the following data cleaning and tidying steps:

- Converted date columns to proper `datetime` format.
- Dropped the `isPartial` column from the Google Trends data as it contained only `False` values.
- Created a `Week` column from the sales data to match the weekly granularity of Google Trends.
- Reset the index in Google Trends to make date a column, and aligned the dates for merging.
- Merged the cleaned datasets on the common weekly date, resulting in a consolidated dataset with:
  - **Week**
  - **Region**
  - **Category**
  - **Sales**
  - **Quantity**
  - **Laptop search interest**

---

## 📈 Analysis Summary

### 1️⃣ Weekly Trends

- I grouped the data weekly by category.
- After **normalizing** the data to a 0–1 scale, I visualized weekly sales vs search interest.
- **Key Insight**: The **Technology** category showed the strongest alignment with spikes in "laptops" search interest. The alignment was less pronounced in Furniture and Office Supplies.

### 2️⃣ Seasonality Check

- I grouped the data by **month** and again normalized the values.
- **Key Insight**: There was a **clear seasonal trend** with both search interest and sales spiking in **November and December**, likely driven by events like Black Friday and Christmas.

---

## ✅ Business Questions Answered

1. **Does online search interest in "laptops" affect sales?**  
   → Yes, especially in the **technology category**, where spikes in search interest were followed by higher sales.

2. **Do certain months have higher search interest and sales?**  
   → Yes, **Q4 (Oct–Dec)** consistently showed higher interest and increased sales volume.

3. **Which categories show alignment with search interest?**  
   → Technology had the **strongest correlation**, followed by occasional spikes in Office Supplies.

---

## Files Included

- `Keyword_Search_vs_Sales_Analysis.ipynb` – Full Jupyter Notebook with code and charts
- `cleaned_merged_sales_trends.csv` – Final cleaned dataset
- `trends_laptops.csv` – Raw Google Trends data
- `Sample - Superstore.csv` – Raw sales dataset from Kaggle

---

## Insights and Conclusions

This project demonstrates that **search interest data can serve as a useful leading indicator for tech sales**. It also shows how seasonal patterns align with consumer interest.

From a business standpoint, **search trend monitoring can guide inventory planning, marketing, and promotions**, especially for tech-related products.

---

## 🔗 Additional Notes

I handled all steps from data gathering to final analysis independently. This notebook demonstrates a full real-world data wrangling pipeline, and I’m proud of completing this from scratch.

📂 View the full notebook and files here:  
👉 [GitHub Repository Link](https://github.com/pratiti-soumya/Data-Science-Projects/tree/main/Keyword_Search_vs_Sales_Analysis)
"""
