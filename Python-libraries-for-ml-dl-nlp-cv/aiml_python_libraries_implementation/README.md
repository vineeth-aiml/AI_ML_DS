# AI/ML Python Libraries — Complete Implementation Pack

This pack is designed for teaching and hands-on implementation before Machine Learning.

## Files

1. `01_NumPy_Complete_Implementation.ipynb`
   - Arrays, indexing, slicing, reshape, broadcasting, statistics, random, boolean filtering,
     stacking/splitting, NaN handling, matrix operations, linear algebra, saving/loading.

2. `02_Pandas_Complete_Implementation.ipynb`
   - Series, DataFrames, file I/O, inspection, filtering, missing values, duplicates, strings,
     grouping, aggregations, transforms, merges, joins, dates, pivots, SQL and export.

3. `03_Matplotlib_Complete_Implementation.ipynb`
   - Line, bar, scatter, histogram, box, pie, legends, grids, figure/axes, subplots,
     annotations, error bars and saving figures.

4. `04_Seaborn_Complete_Implementation.ipynb`
   - Scatter, line, count, bar, hist/KDE, box, violin, strip, regression,
     heatmap, pairplot, jointplot and catplot.

5. `05_Integrated_Data_Analysis_Project.ipynb`
   - Full project using NumPy + Pandas + Matplotlib + Seaborn together.
   - Covers data cleaning, duplicates, missing values, outliers, feature creation,
     groupby analysis, EDA, correlations and exports.

6. `06_All_In_One_Revision.ipynb`
   - Fast revision notebook combining all four libraries.

## Dataset

`data/employee_analytics_project.csv`

The project dataset intentionally contains:
- missing values
- duplicates
- salary outliers
- numerical and categorical variables

This makes it suitable for realistic preprocessing and EDA.

## Recommended Order

NumPy → Pandas → Matplotlib → Seaborn → Integrated Project → Machine Learning

## Install Requirements

```bash
pip install numpy pandas matplotlib seaborn jupyter openpyxl
```

## Start Jupyter

From this folder:

```bash
jupyter notebook
```

or:

```bash
jupyter lab
```

Open notebooks in numerical order and run cells from top to bottom.
