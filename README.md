# River Water Quality – Statistical Analysis

## About the Project

This project was developed as part of my application to the **M.Sc. Data Science program at TU Dortmund University (Summer Semester 2027)**.

It focuses on the statistical analysis of river water quality data, investigating seasonal and spatial variations in oxygen and nitrate concentrations.

## Research Questions

The analysis addresses the two questions of the task:

1. Is there a statistically significant difference between spring and autumn regarding the concentration of oxygen and nitrate?
2. Is there a difference in the concentrations between the river sections? Which groups are different from each other?

## Dataset

The dataset contains **900 observations**, covering:

- 5 river sections (A1–A5), from headwaters to mouth.
- 4 seasons (Spring, Summer, Autumn, Winter).
- Nitrate concentration (mg/L).
- Oxygen concentration (mg/L).

The dataset is balanced, with 45 observations for each section-season combination.

## Methods & Techniques

- Descriptive Statistics and Data Visualization.
- Shapiro-Wilk Test for Normality.
- Levene Test for Equal Variances (median-centred, i.e. the Brown-Forsythe variant).
- Independent-Samples t-Test.
- Mann-Whitney U Test.
- One-Way ANOVA.
- Kruskal-Wallis Test.
- Tukey's HSD and Bonferroni Correction for Post-hoc Comparisons.

## Key Findings

### 1. Seasonal Comparison (Spring vs. Autumn)

- **Nitrate:** A statistically significant difference was found (Mann-Whitney U, p = 0.00078). The mean concentration was higher in spring (9.289 mg/L) than in autumn (8.418 mg/L).
- **Oxygen:** No statistically significant difference was found (independent-samples t-test, p = 0.0654).

### 2. Differences Between River Sections

- **Nitrate:** One-way ANOVA revealed significant differences between the five sections (p < 0.001). The mean concentration increased from A1 (5.350 mg/L) to A5 (11.467 mg/L). Tukey's HSD confirmed significant differences between all pairs of sections.
- **Oxygen:** The Kruskal-Wallis test showed a significant overall difference (p = 0.0202). After Bonferroni correction, only the comparison between A1 and A4 was statistically significant.

### 3. Additional Analysis: Seasonal Oxygen Patterns

An additional analysis explored spatial differences in oxygen concentrations within each season. The four seasonal Kruskal-Wallis p-values were Bonferroni-adjusted (m = 4), and the pairwise tests were adjusted within each season (m = 10):

- **Summer:** Significant differences were found, with A4 and A5 showing lower oxygen concentrations than A1, A2, and A3.
- **Autumn:** A4 differs significantly from A5 and, marginally, from A1 (adjusted p = 0.0498).
- **Spring and Winter:** No statistically significant differences were detected between the sections.

## Tools & Libraries

- Python 3.10.0
- pandas 2.3.3
- SciPy 1.15.3
- Matplotlib 3.10.9 & Seaborn 0.13.2
- Jupyter Notebook

## Significance Level

All hypothesis tests were conducted using a significance level of **α = 0.05**.

## Project Goal

The project demonstrates the application of statistical methods to environmental data, including assumption checking, hypothesis testing, post-hoc analysis, data visualization, and interpretation of statistical results.
