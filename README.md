# 🎬 Movie Data Analysis Project

## Overview
This project involves analyzing a movie dataset with over 60,000 entries spanning from 1975 to 2025. The goal is to explore industry trends, understand what factors contribute to a movie’s success, and derive actionable insights from the data using Python (Pandas, Matplotlib, Seaborn).

---

## 📁 Dataset Description

### 🧾 Column Descriptions

| **Column Name**             | **Description**                                                                 |
|----------------------------|---------------------------------------------------------------------------------|
| `IMDb ID of the Movie`     | A unique identifier assigned to each movie by IMDb.                            |
| `title`                    | The official title of the movie.                                               |
| `year`                     | The release year of the movie. Useful for trend analysis.                      |
| `duration`                 | Runtime of the movie (e.g., "2h 15m"). Converted to minutes for consistency.   |
| `MPA`                      | Motion Picture Association rating (e.g., G, PG-13, R).                         |
| `rating`                   | Average IMDb user rating (scale of 0 to 10).                                   |
| `votes`                    | Number of users who rated the movie. Reflects popularity.                      |
| `meta_score`               | Critic rating from Metacritic (0–100 scale).                                   |
| `description`              | Short plot summary or synopsis of the movie.                                   |
| `Movie_Link`               | URL to the IMDb page for the movie.                                            |
| `writers`                  | List of writers involved in the movie.                                         |
| `directors`                | List of directors. Useful for analyzing directorial influence.                 |
| `stars`                    | Leading actors or actresses in the movie.                                      |
| `budget`                   | Estimated production budget (standardized to USD).                             |
| `opening_weekend_gross`    | Opening weekend earnings.                                                      |
| `gross_usa`                | Total earnings in the USA.                                                     |
| `worldwide_gross`          | Global revenue.                                                                |
| `genre`                    | Genre(s) associated with the movie.                                            |
| `country`                  | Country or countries where the movie was produced.                             |

---

## 🧹 Data Cleaning

Key steps performed:
- Removed null and irrelevant entries.
- Cleaned currency columns and converted all values to USD.
- Standardized runtime (`duration`) into minutes.
- Removed special characters from genre, country, and list-based fields (e.g., `[]`, `''`).

---

## 📈 Exploratory Data Analysis (EDA)

### 🎥 General Insights
- Average number of movies produced per year: **~594**
- Data spans **50+ years** of global movie production.
  
### 💰 Financial Performance
- Higher budgets generally correlate with higher worldwide gross.
- Action, Adventure, Fantasy, and Science Fiction genres tend to perform best globally.

### 🌍 Genre & Country Insights
- USA dominates the movie industry in both volume and revenue.
- Countries like India, UK, and Canada also show strong contributions in specific genres.

### 🎯 ROI (Return on Investment)
- Movies with low budgets but high returns are often in Horror, Thriller, and Drama genres.
- High-budget movies that underperform were identified and analyzed.

### ⭐ Ratings & Popularity
- Most rated movies: Top 10 list based on number of IMDb votes.
- Highest-rated movies (with minimum vote thresholds) are typically in Drama and Biography genres.
- Meta score and IMDb rating show moderate correlation.

### ⏱️ Duration Analysis
- Most popular duration range: **90–120 minutes**.
- Extremely long or short movies tend to have polarized ratings.

---

## 📊 Visualizations

Key plots created using Python:
- Budget vs. Worldwide Gross scatter plot
- Rating vs. Duration box plot
- Top 10 genres by average ROI
- Yearly movie production trend line
- Top 10 most rated movies bar chart

---

## 📌 Business Problem

The business goal was to identify the key factors that lead to a movie’s financial and critical success. This insight can help:

- Production houses optimize budgeting.
- Marketing teams target high-ROI genres and durations.
- Studios invest in countries and genres with rising success rates.

---

## Tools & Technologies Used

- **Languages**: Python
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib
- **Visualization**: Jupyter Notebook
- **Data Cleaning**: Regex, Currency normalization
- **Data Source**: IMDb, Kaggle (dataset already aggregated)

---

## 📌 Conclusion

This analysis provided a data-driven look into the film industry, helping uncover trends that can guide production decisions. Future work may include predictive modeling (e.g., predicting box office success) or deeper NLP analysis on movie descriptions.




