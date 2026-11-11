# River-Water-Quality-Statistical-Analysis
Statistical analysis of river water quality data, investigating seasonal and spatial variations in oxygen and nitrate concentrations using Python, hypothesis testing, and data visualization.


# River Water Quality – Statistical Analysis

## About the Project

This project was developed as part of my application to the **M.Sc. Data Science program at TU Dortmund University (Summer Semester 2027)**.

It focuses on the statistical analysis of river water quality data, investigating variations in oxygen and nitrate concentrations across different seasons and river sections.

## Research Questions

The analysis addresses two main questions:

1. **Seasonal Differences:** Do oxygen and nitrate concentrations differ significantly between spring and autumn?
2. **Spatial Differences:** Do oxygen and nitrate concentrations differ significantly across the five river sections? If so, which sections show significant differences?

An additional seasonal analysis was conducted to explore how spatial differences in oxygen concentrations vary throughout the year.

## Dataset

The dataset contains **900 observations** covering:

- 5 river sections (A1–A5).
- 4 seasons (Spring, Summer, Autumn, Winter).
- Nitrate concentration (mg/L).
- Oxygen concentration (mg/L).

The dataset is balanced, with 45 observations for each section-season combination.

## Methods & Techniques

The project applies several statistical methods, including:

- Descriptive Statistics and Data Visualization.
- Shapiro-Wilk Test for Normality.
- Brown-Forsythe Test for Homogeneity of Variances.
- Independent-Samples t-Test.
- Mann-Whitney U Test.
- One-Way ANOVA.
- Kruskal-Wallis Test.
- Tukey's HSD and Bonferroni Correction for Post-hoc Comparisons.

## Tools & Libraries

- Python
- Pandas & NumPy
- SciPy
- Statsmodels
- Matplotlib & Seaborn
- Jupyter Notebook

## Significance Level

All hypothesis tests use a significance level of **α = 0.05**.

## Project Goal

The main goal is to apply statistical analysis techniques to real-world environmental data, evaluate statistical assumptions, select appropriate hypothesis tests, and interpret the results.
