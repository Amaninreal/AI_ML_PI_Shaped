# Titanic Dataset Analysis - Jupyter Notebook Project

This project explores the famous [Titanic dataset](https://www.kaggle.com/c/titanic) using Python and key data analysis libraries. It walks through data loading, cleaning, analysis, and visualization to understand survival trends and uncover insights.

---

## Dataset Used

- File: `Titanic-Dataset.csv`
- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)

---

## Objectives

- Practice data manipulation and exploratory data analysis (EDA)
- Handle missing values and clean raw data
- Discover survival patterns using statistics and visualization
- Summarize insights with compelling charts

---

## Libraries Used

- `pandas` – Data manipulation
- `numpy` – Numeric operations
- `matplotlib` & `seaborn` – Visualization

---

## Steps Performed

### 1. Data Loading & Familiarization
- Loaded the CSV using `pandas.read_csv()`
- Inspected the structure with `.head()`, `.info()`, `.describe()`

### 2. Initial Exploration
- Checked dataset shape, missing values
- Explored basic statistical trends

### 3. Data Cleaning
- Filled missing values (`Age`, `Embarked`)
- Dropped irrelevant/redundant columns (`Cabin`, `Ticket`, `Name`, etc.)
- Converted categorical variables (`Sex`, `Embarked`) to numeric format

### 4. Feature Engineering
- Extracted titles from passenger names
- Grouped rare titles under a single label: `Rare`
- Created age buckets (Child, Teen, Adult, etc.)

### 5. Data Analysis
- Analyzed survival rates by:
  - Gender
  - Passenger class
  - Age group
  - Titles

### 6. Visualization
- Used bar plots, count plots, histograms, and pie charts to visualize:
  - Survival rates by gender, class, and age group
  - Distribution of rare titles and their survival chances

---

## Key Insights

- **Females had a significantly higher survival rate than males.**
- **First-class passengers had the highest chance of survival.**
- **Children and young adults had better survival chances than older passengers.**
- **Certain social titles (like "Mrs", "Miss", "Master") had much higher survival rates.**
- **Passengers with rare titles also showed varied survival patterns.**

---

## Files Included

- `Titanic-Dataset.csv` – Main dataset
- `Titanic_Analysis.ipynb` – Jupyter notebook with complete step-by-step code, commentary, and visualizations
- `README.md` – Project documentation

---