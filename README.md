# 🎬 IMDB Case Study — Movies & Directors Analysis

> **Tools Used:** Python | Pandas | NumPy
> **Dataset:** 1,465 Movies | 2 Tables (movies.csv + directors.csv)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/senapathi402-star/IDMB_CASE_STUDY/blob/main/IDMB_Case_Study.ipynb)

---

## 📌 Objective

Analyze IMDB movie data to uncover trends in movie budgets, revenues, popularity, ratings, and release patterns across years and months using Pandas and NumPy.

---

## 🗃️ Dataset Structure

### movies.csv — 1,465 rows × 11 columns

| Column | Type | Description |
|--------|------|-------------|
| `id` | int | Movie ID |
| `budget` | int | Production budget ($) |
| `popularity` | int | Popularity score |
| `revenue` | int | Total revenue ($) |
| `title` | object | Movie title |
| `vote_average` | float | IMDB rating (out of 10) |
| `vote_count` | int | Number of votes |
| `director_id` | int | Foreign key to directors |
| `year` | int | Release year |
| `month` | object | Release month |
| `day` | object | Release day of week |

### directors.csv
Contains director details linked to movies via `director_id`

---

## 🔍 Key Dataset Highlights

| Metric | Value |
|--------|-------|
| 🎬 Total Movies | 1,465 |
| 💰 Highest Revenue Movie | Avatar — $2,787,965,087 |
| ⭐ Avatar Rating | 7.2 / 10 |
| 🏆 Highest Budget | Pirates of the Caribbean: At World's End — $300M |
| 📅 Year Range | 1978 – 2015 |
| 🎭 Most Popular Movie | Avatar (popularity score: 150) |

---

## 🎯 Notable Movies in Dataset

| Title | Year | Budget | Revenue | Rating |
|---|---|---|---|---|
| Avatar | 2009 | $237M | $2.79B | 7.2 |
| The Dark Knight Rises | 2012 | $250M | $1.08B | 7.6 |
| Pirates of the Caribbean: At World's End | 2007 | $300M | $961M | 6.9 |
| Spectre | 2015 | $245M | $880M | 6.3 |
| Spider-Man 3 | 2007 | $258M | $890M | 5.9 |

---

## 🛠️ Python Concepts Used

- `pd.read_csv()` — loading multiple CSV files with `index_col=0`
- **Multi-table analysis** — working with movies and directors datasets
- `df.merge()` — joining movies and directors on `director_id`
- `df.info()` — checking data types and null counts
- `df.describe()` — statistical summary of numerical columns
- `df.sort_values()` — ranking movies by revenue, rating, budget
- `df.groupby()` — aggregating by year, month, day of week
- **NumPy** — numerical calculations and array operations

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `IDMB_Case_Study.ipynb` | Jupyter Notebook with full analysis |
| `movies.csv` | IMDB movies dataset |
| `directors.csv` | Directors dataset |
| `README.md` | Project documentation |

---

## ▶️ How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install pandas numpy
   ```
3. Open `IDMB_Case_Study.ipynb` in Jupyter Notebook or Google Colab
4. Run all cells from top to bottom

---

## 👤 Author

**Senapathi Krishna Sai**
Data Analyst | SQL | Python | Tableau | Excel

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/senapathi-krishna-sai-a54721388)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/senapathi402-star)
