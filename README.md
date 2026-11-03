# Data-Cleaning-Project-
Developing data science skills through data cleaning of a messy dataset obtained from kaggle
# Hospital lab results: cleaning and exploration

**Question:** Do three hospitals differ in glucose, cholesterol and HbA1c
results, and how many results are above the normal limit?

**Data:** 1,500 results, 3 hospitals, 3 tests (likely synthetic).
Link: https://www.kaggle.com/datasets/nudratabbas/multi-hospital-lab-results-messy-data

**What I did:**  I explored and cleaned the dataset, I found out that the dataset had 101 missing values which came in disguised form(empty cells, -999 placeholders and not collected text), 7 glucose values above 30 were treated as outliers 6 of which were of value 500 and set to missing.

**Key findings:** 
-Hospital A has the highest share above the limit in all three tests, differences are modest and haven’t been tested statistically. If our dataset is synthetic, this explains such abnormal values.Else, a high percentage of the population is unhealthy(a guess from if the dataset is real).
-From plot 6, Collection was steady at about 55 to 70 results per month, with no empty months.The lowest months were March 2024 (15, a partial first month), February 2025 (44) and September 2024 (46)

**Plots:** 
figures\01_missing_types.png
figures\03_distribution_vs_limit.png


**Limitations:** This dataset has a high probability of being synthetic hence the presence of so many placeholders and unrealistic values, hospital differences not tested statistically.

**How to run:** pip install -r requirements.txt, then open the notebook.
