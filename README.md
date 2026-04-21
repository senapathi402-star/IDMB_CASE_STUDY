# 🚢 Titanic Data Cleaning & Visualization
> **Tools Used:** Python | Pandas | NumPy | Matplotlib | Seaborn
> **Dataset:** 891 Passengers | 2 Sections (Cleaning + Visualization)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/senapathi402-star/data_cleaning_and_visualizing_titanic_dataset/blob/main/Titanic_data_cleaning_And_visualization.ipynb)

---

## 📌 Objective

Analyze the Titanic passenger dataset to clean missing values, handle data quality issues, and uncover survival trends based on gender, passenger class, deck, age, and fare using Pandas, NumPy, Matplotlib, and Seaborn.

---

## 🗃️ Dataset Structure

### titanic — 891 rows × 15 columns

| Column | Type | Description |
|--------|------|-------------|
| `survived` | int | Survival status (0 = No, 1 = Yes) |
| `pclass` | int | Passenger class (1 = First, 2 = Second, 3 = Third) |
| `sex` | object | Gender of passenger |
| `age` | float | Age of passenger |
| `sibsp` | int | Number of siblings/spouses aboard |
| `parch` | int | Number of parents/children aboard |
| `fare` | float | Ticket fare ($) |
| `embarked` | object | Port of embarkation (S / C / Q) |
| `class` | category | Passenger class (text) |
| `who` | object | Man / Woman / Child |
| `adult_male` | bool | Whether passenger is an adult male |
| `deck` | category | Deck on the ship (A–G) |
| `embark_town` | object | Embarkation town name |
| `alive` | object | Survival status (yes / no) |
| `alone` | bool | Whether passenger was travelling alone |

---

## 🔍 Key Dataset Highlights

| Metric | Value |
|--------|-------|
| 🚢 Total Passengers | 891 |
| ✅ Survivors | 342 (38.4%) |
| ❌ Deaths | 549 (61.6%) |
| 👩 Female Survival Rate | 74.2% |
| 👨 Male Survival Rate | 18.9% |
| 📅 Missing Age Values | 177 |
| 🃏 Missing Deck Values | 688 |
| 🔁 Duplicate Rows Found | 116 |

---

## 🎯 Notable Statistics

| Category | Detail |
|----------|--------|
| Most Passengers | Class 3 — 491 passengers |
| Most Common Deck | Deck F (after imputation) |
| Boarding Port | Southampton — most common |
| Average Female Age | 28 years |
| Average Male Age | 31 years |
| Fare Range | $0 – $512 |
| Age Range | 0 – 80 years |

---

## 🧹 Data Cleaning Steps

| Column | Issue | Solution |
|--------|-------|----------|
| `age` | 177 missing values | Filled with gender-wise mean |
| `embarked` | 2 missing values | Filled with mode (`S`) |
| `embark_town` | 2 missing values | Filled with mode (`Southampton`) |
| `deck` | 688 missing values | Filled with pclass-wise mode |
| `age` | Float dtype | Converted to integer |

> **Note:** 116 duplicate rows were identified but **not removed**, as without passenger names, identical rows may represent genuinely different individuals.

---

## 📊 Visualizations Covered

| Type | Analysis |
|------|----------|
| Univariate — Numerical | Passenger class distribution (bar chart) |
| Univariate — Categorical | Deck distribution (count plot) |
| Bivariate — Cat vs Num | Survival count by deck (grouped bar chart) |
| Bivariate — Cat vs Cat | Survival rate by gender (pie chart) |
| Bivariate — Num vs Num | Fare vs Age (scatter plot) |
| Distribution | Fare distribution (box plot) |
| Distribution | Age distribution (box plot) |

---

## 🛠️ Python Concepts Used

- `sns.load_dataset()` — loading built-in Titanic dataset
- `df.isna().sum()` — detecting missing values per column
- `df.fillna()` — imputing missing values with mode and mean
- `df.groupby()` — computing gender-wise age averages
- `df.astype()` — converting float to integer
- `df.duplicated()` — identifying duplicate rows
- `df.value_counts()` — frequency counts per category
- `sns.countplot()` — bar charts for categorical data
- `sns.scatterplot()` — numerical vs numerical analysis
- `sns.boxplot()` — outlier detection and distribution
- `plt.pie()` — survival percentage by gender

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `Titanic_data_cleaning_And_visualization.ipynb` | Jupyter Notebook with full analysis |
| `README.md` | Project documentation |

---

## ▶️ How to Run

1. Clone this repository:
```bash
   git clone https://github.com/senapathi402-star/data_cleaning_and_visualizing_titanic_dataset.git
```

2. Install dependencies:
```bash
   pip install pandas numpy matplotlib seaborn
```

3. Open `Titanic_data_cleaning_And_visualization.ipynb` in Jupyter Notebook or Google Colab

4. Run all cells from top to bottom

---

## 👤 Author

**Senapathi Krishna Sai**
Data Analyst | SQL | Python | Tableau | Excel

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/senapathi-krishna-sai-a54721388)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/senapathi402-star)
