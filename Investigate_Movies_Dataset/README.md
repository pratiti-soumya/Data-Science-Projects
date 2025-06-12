# TMDb Movie Dataset Analysis

This project explores the [TMDb movie dataset](https://www.themoviedb.org/), focusing on uncovering trends in movie budgets, revenue, popularity by genre, and runtime over time. I developed it as part of Udacity data science project using Python and key data science libraries.

## 📁 Project Files
- `Investigate_a_Dataset.ipynb` (not included here): Jupyter Notebook containing the full analysis
- `tmdb-movies.csv`: The dataset used (pre-cleaned version)

## 🔍 Overview
The dataset includes over 10,000 movies with details like title, release year, genres, budget, revenue, popularity, runtime, user ratings, and vote count. This project aims to answer three main analytical questions using data wrangling and visualization techniques.

## 🧹 Data Wrangling Steps
- Dropped irrelevant columns: `id`, `imdb_id`, `homepage`, `overview`, `tagline`, `keywords`, `production_companies`, and `cast`.
- Removed duplicate rows.
- Handled missing values (dropped rows with missing `director` or `genres`).
- Split multi-valued `genres` column using `.str.split('|')` and `.explode()`.

## 📊 Exploratory Questions and Analysis

### 1. Do movies with higher budgets tend to earn higher revenue?
- Created a scatter plot of budget vs revenue.
- Applied log transformation to reduce skewness.
- Found a moderate positive correlation (≈ 0.65) between log-transformed budget and revenue.

### 2. Which genres have the highest average popularity?
- Transformed and grouped genre data.
- Used a bar chart to visualize average popularity.
- Found that **Adventure**, **Science Fiction**, and **Fantasy** genres scored the highest.

### 3. How has the average movie runtime changed over the years?
- Grouped data by release year and calculated average runtime.
- Created a line chart.
- Found that movies were longest in the 1960s and have shortened in more recent years.

## 📝 Conclusion
- **Higher budgets are generally associated with higher revenue**, but correlation is not causation.
- **Adventure and Sci-Fi genres are the most popular**, likely due to production value and franchise appeal.
- **Movie runtimes have decreased** from the 1960s to the present, possibly due to changing audience preferences.


## 💻 Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib

## 👩‍💻 Author
**Pratiti Soumya**  
[LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/)

