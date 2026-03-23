# Students’ Social Media Addiction & Mental Health  
Statistical Analysis Project

## Project Overview

This project investigates the statistical relationships between students’ mental health and various behavioral and contextual factors, including social media usage, sleep duration, relationship status, academic level, and gender.

The analysis is conducted using classical statistical methods without machine learning modeling. The focus is on interpretability, hypothesis testing, and effect size evaluation.

---

## Research Objective

The primary outcome variable is **Mental_Health_Score**, a self-reported measure of students’ well-being on a 1–10 scale.

The project addresses the following research questions:

- Is there a statistical association between mental health and social media usage?
- Is sleep duration associated with mental health?
- Do mental health scores differ across relationship status groups?
- Are categorical variables (e.g., academic level and relationship status) statistically associated?
- Are the observed relationships robust across subgroups?

---

## Dataset

The dataset contains survey-based responses from students, including:

- Mental_Health_Score (1–10 scale)
- Sleep_Hours_Per_Night
- Addicted_Score
- Relationship_Status
- Academic_Level
- Gender
- Other behavioral variables

Sample size: 705 observations.

---

## Methodology

The analysis includes:

### 1. Exploratory Data Analysis (EDA)
- Distribution analysis
- Skewness evaluation
- Scatterplots and pairwise relationships

### 2. Numerical ↔ Numerical Relationships
- Pearson correlation (linear association)
- Spearman correlation (monotonic association)
- Regression plots
- Residual analysis (heteroscedasticity check)

### 3. Numerical ↔ Categorical Relationships
- Boxplots and violin plots
- Group medians and descriptive statistics
- Kruskal–Wallis test
- Effect size (epsilon-squared)

### 4. Categorical ↔ Categorical Relationships
- Contingency tables
- Row-normalized proportions
- Chi-square test of independence
- Cramér’s V effect size
- Standardized residuals analysis

All statistical decisions were based on:
- p-values (statistical significance)
- effect sizes (practical significance)
- visual diagnostics

---

## Key Findings

- Sleep duration shows a strong positive association with mental health.
- Social media addiction score shows a strong negative association with mental health.
- Relationship status does not meaningfully influence mental health scores.
- Academic level shows statistically significant but small differences.
- No substantial association was found between gender and relationship status.

---

## Tools & Methods

### Programming
- Python 3.x
- Jupyter Notebook

### Data Handling
- pandas
- numpy

### Visualization
- matplotlib
- seaborn

### Statistical Analysis
- scipy.stats
    - pearsonr
    - spearmanr
    - kruskal
    - chi2_contingency

### Effect Size Metrics
- Epsilon-squared (Kruskal–Wallis)
- Cramér’s V (Chi-square)

### Statistical Concepts Applied
- Correlation analysis
- Hypothesis testing
- Distribution comparison
- Homoscedasticity diagnostics
- Contingency table analysis

---

## Project Type

Statistical analysis project (non-ML), focused on hypothesis testing, interpretation, and statistical reasoning.