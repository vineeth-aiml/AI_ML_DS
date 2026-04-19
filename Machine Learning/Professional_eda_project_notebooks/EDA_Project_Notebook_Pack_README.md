# EDA Project Notebook Pack

This repository pack contains **4 GitHub-ready Jupyter notebooks** built from our chat and organized as separate end-to-end EDA projects.

## Projects Included

1. `adult_income_eda.ipynb` — **Classification EDA**
2. `ames_regression_eda.ipynb` — **Regression EDA**
3. `online_retail_unsupervised_eda.ipynb` — **Unsupervised / Customer Segmentation EDA**
4. `open_bandit_eda.ipynb` — **RL-style / Logged Bandit EDA**

Each notebook covers:
- problem framing
- why each step is used
- NumPy + Pandas + Matplotlib + Seaborn + Plotly usage
- preprocessing and cleaning
- EDA and visualization
- analysis and insights
- saving cleaned CSVs before modeling

---

# How to Use This Pack

## 1) Download the notebooks
Use the `.ipynb` files directly from this pack and place each one inside the correct project folder.

## 2) Create a separate GitHub repo or folder for each project
Recommended structure:

```text
project-name/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── your_notebook.ipynb
│
├── reports/
│   ├── figures/
│   └── insights.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## 3) Download the raw dataset for that project
Place the raw file in the expected `data/raw/` path.

## 4) Open the notebook in Jupyter
Run cells from top to bottom.

## 5) Check generated outputs
After the notebook runs, processed CSVs and plots will be saved in `data/processed/` and `reports/figures/`.

## 6) Push to GitHub
Upload:
- notebook
- processed outputs you want to show
- plots
- README
- requirements file

---

# Project 1 — Adult Income EDA (Classification)

## Notebook
`adult_income_eda.ipynb`

## Problem Type
Classification

## Goal
Analyze the Adult / Census Income dataset before building classification models.

## Raw dataset to download
**Official source:** UCI Adult dataset

Dataset page:
- https://archive.ics.uci.edu/dataset/2/adult

Files available there:
- `adult.data`
- `adult.test`
- `adult.names`

## What you should do
1. Download `adult.data`
2. Rename it to `adult.csv`
3. Place it here:

```text
eda-adult-income/data/raw/adult.csv
```

## Recommended project structure

```text
eda-adult-income/
│
├── data/
│   ├── raw/
│   │   └── adult.csv
│   └── processed/
│
├── notebooks/
│   └── adult_income_eda.ipynb
│
├── reports/
│   ├── figures/
│   └── insights.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Main outputs generated
- `adult_missing_report.csv`
- `adult_numeric_summary.csv`
- `adult_categorical_summary.csv`
- `adult_outlier_report.csv`
- `adult_skew_report.csv`
- `adult_cleaned.csv`

## Next modeling step
Use `adult_cleaned.csv` for:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost / LightGBM / CatBoost later

---

# Project 2 — Ames Housing EDA (Regression)

## Notebook
`ames_regression_eda.ipynb`

## Problem Type
Regression

## Goal
Analyze housing price data before building regression models.

## Raw dataset to download
**Recommended source:** Kaggle House Prices competition dataset

Dataset page:
- https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## What you should do
1. Download `train.csv`
2. Place it here:

```text
eda-ames-housing/data/raw/train.csv
```

## Recommended project structure

```text
eda-ames-housing/
│
├── data/
│   ├── raw/
│   │   └── train.csv
│   └── processed/
│
├── notebooks/
│   └── ames_regression_eda.ipynb
│
├── reports/
│   ├── figures/
│   └── insights.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Main outputs generated
- `ames_missing_report.csv`
- `ames_numeric_summary.csv`
- `ames_categorical_summary.csv`
- `ames_outlier_report.csv`
- `ames_skew_report.csv`
- `target_summary.csv`
- `neighborhood_price_summary.csv`
- `quality_price_summary.csv`
- `ames_cleaned.csv`

## Next modeling step
Use `ames_cleaned.csv` for:
- Linear Regression
- Ridge
- Lasso
- ElasticNet
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost / LightGBM / CatBoost later

---

# Project 3 — Online Retail EDA (Unsupervised)

## Notebook
`online_retail_unsupervised_eda.ipynb`

## Problem Type
Unsupervised learning / Customer Segmentation

## Goal
Clean raw retail transactions, build customer features, and prepare data for clustering.

## Raw dataset to download
**Official source:** UCI Online Retail dataset

Dataset page:
- https://archive.ics.uci.edu/dataset/352/online%2Bretail

File available there:
- `Online Retail.xlsx`

## What you should do
1. Download `Online Retail.xlsx`
2. Rename it to `online_retail.xlsx`
3. Place it here:

```text
eda-online-retail-unsupervised/data/raw/online_retail.xlsx
```

## Recommended project structure

```text
eda-online-retail-unsupervised/
│
├── data/
│   ├── raw/
│   │   └── online_retail.xlsx
│   └── processed/
│
├── notebooks/
│   └── online_retail_unsupervised_eda.ipynb
│
├── reports/
│   ├── figures/
│   └── insights.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Main outputs generated
- `retail_missing_report.csv`
- `retail_numeric_summary.csv`
- `retail_categorical_summary.csv`
- `retail_outlier_report.csv`
- `retail_transaction_cleaned.csv`
- `retail_customer_features.csv`
- `retail_rfm_summary.csv`
- `retail_country_summary.csv`

## Next modeling step
Use `retail_customer_features.csv` for:
- KMeans
- Hierarchical Clustering
- DBSCAN
- Gaussian Mixture Model
- PCA / t-SNE visualization

---

# Project 4 — Open Bandit Dataset EDA (RL-style)

## Notebook
`open_bandit_eda.ipynb`

## Problem Type
RL-style logged bandit / offline bandit analysis

## Goal
Analyze logged bandit feedback, flatten it into a modeling-ready table, and prepare for bandit algorithms and off-policy evaluation.

## Raw dataset to download
**Official docs / loader:** Open Bandit Pipeline (OBP)

Quickstart:
- https://zr-obp.readthedocs.io/en/latest/quickstart.html

About OBP:
- https://zr-obp.readthedocs.io/en/latest/about.html

## What you should do
1. Install `obp`
2. Use the notebook to load the dataset through the official loader
3. Keep a folder like this for OBP raw data cache / files:

```text
eda-open-bandit-rl/data/raw/obd/
```

## Recommended project structure

```text
eda-open-bandit-rl/
│
├── data/
│   ├── raw/
│   │   └── obd/
│   └── processed/
│
├── notebooks/
│   └── open_bandit_eda.ipynb
│
├── reports/
│   ├── figures/
│   └── insights.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Main outputs generated
- `bandit_raw_export.csv`
- `bandit_missing_report.csv`
- `bandit_numeric_summary.csv`
- `bandit_categorical_summary.csv`
- `bandit_reward_summary.csv`
- `bandit_action_summary.csv`
- `bandit_policy_summary.csv`
- `bandit_cleaned.csv`
- `bandit_model_table.csv`

## Next modeling step
Use `bandit_model_table.csv` for:
- Random baseline
- Epsilon-Greedy
- UCB
- Thompson Sampling
- Contextual bandits
- IPS / SNIPS / Doubly Robust evaluation

---

# What to Upload to GitHub

For each project, upload:
- the `.ipynb` notebook
- `README.md`
- `requirements.txt`
- `.gitignore`
- selected processed CSVs
- selected figures from `reports/figures/`
- `reports/insights.md`

## Recommended
Do **not** upload extremely large raw files unless needed.
Instead, keep the README dataset link and explain where to download the data.

---

# Important Notes

## 1) Raw data path matters
If the notebook is inside `notebooks/`, paths like `../data/raw/...` will work.

## 2) Run from top to bottom
These notebooks are designed to be run in sequence from the first cell to the last.

## 3) Cleaned CSV is the main modeling file
Summary CSVs are for analysis.
The cleaned / model table CSV is what you use for modeling.

Examples:
- `adult_cleaned.csv` → classification models
- `ames_cleaned.csv` → regression models
- `retail_customer_features.csv` → clustering models
- `bandit_model_table.csv` → bandit / RL-style models

---

# Suggested GitHub Repo Names

- `adult-income-eda-classification`
- `ames-housing-eda-regression`
- `online-retail-eda-unsupervised`
- `open-bandit-eda-rl`

---

# Suggested Commit Flow

1. Create repo
2. Add folder structure
3. Add notebook
4. Add README
5. Run notebook locally
6. Add processed outputs and figures
7. Push final version

---

# Final Note

This pack is meant to help you post serious, organized EDA projects to GitHub.
Each notebook is designed to look more professional than normal small demo notebooks because it includes:
- structure
- reasoning
- preprocessing
- visualization
- saved outputs
- modeling readiness

