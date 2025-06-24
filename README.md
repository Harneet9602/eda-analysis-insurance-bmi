 EDA Analysis on Insurance BMI Data

This repository contains a Jupyter notebook performing detailed exploratory data analysis (EDA) on an insurance dataset. The focus is on BMI-based feature engineering and statistical analysis of the data.

 📌 Objectives

The notebook answers the following questions:

1️⃣ Are there missing values, duplicate rows, and what are the data types?  
👉 The notebook inspects the dataset for missing data, duplicates, and identifies the type of each feature.

2️⃣ How can we categorize BMI values?  
👉 A new feature `BMI_Category` is created using BMI thresholds:
- Underweight (BMI < 18.5)
- Normal (18.5 ≤ BMI < 24.9)
- Overweight (25 ≤ BMI < 29.9)
- Obese (BMI ≥ 30)

3️⃣ Are charges, BMI, and age normally distributed?  
👉 Normality is checked using the Shapiro-Wilk test on:
- `charges`
- `bmi`
- `age`

4️⃣ How does the BMI category relate to charges?  
👉 The notebook explores this via grouped statistics and visualization (e.g. boxplots or barplots).

5️⃣ What is the correlation between numeric variables?  
👉 Correlation coefficients between key features are computed.

6️⃣ What is the effect of outlier removal (if any is done)?  
👉 The notebook optionally explores IQR-based outlier detection (if code is included).

 📂 Files

- `insurance.ipynb` — Full notebook containing all code, outputs, and plots
- `insurance.csv` — (you may add or link to the dataset source)

 ⚡ Requirements

```bash
pip install pandas numpy matplotlib seaborn scipy
