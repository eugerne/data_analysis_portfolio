# Case Study #1
# Understanding the Relationship Between Social Media Usage and Mental Health Among Students

> An end-to-end analytical case study exploring how behavioral and lifestyle factors are associated with students' mental well-being using exploratory analysis, statistical inference, and regression modeling.

---

## Overview

Mental health has become one of the most important public health concerns among young adults. At the same time, social media has become an integral part of students' daily lives, raising questions about its potential impact on psychological well-being.

This project investigates whether behavioral factors such as social media usage, sleep duration, relationship status, and academic level are associated with students' mental health.

Rather than relying on a single analytical technique, the project follows a complete analytical workflow—from exploratory data analysis to statistical hypothesis testing and regression modeling—to better understand both the relationships within the data and their practical significance.

---

## Research Objectives

The project aims to answer the following questions:

- Is social media usage associated with students' mental health?
- Does sleep duration influence mental well-being?
- Which behavioral variables show the strongest relationship with mental health?
- Are observed differences statistically significant?
- Can multiple behavioral factors jointly explain variations in mental health?

---

## Dataset

**Source**

Student Lifestyle & Mental Health Survey (Kaggle)

**Sample size**

705 observations

**Main variables**

- Mental Health Score
- Social Media Addiction Score
- Average Daily Usage Hours
- Sleep Hours
- Academic Level
- Relationship Status
- Gender
- Lifestyle indicators

The dataset consists of anonymous survey responses describing students' lifestyle habits and self-reported mental health.

---

## Analytical Workflow

The project is divided into three consecutive stages.

### Stage 1 — Exploratory Data Analysis

The first stage focuses on understanding the dataset before performing any statistical analysis.

Main tasks:

- data inspection
- missing value analysis
- feature distributions
- comparison between depression groups
- pairwise visualization
- preliminary pattern identification

---

### Stage 2 — Statistical Analysis

The second stage evaluates whether the observed relationships are statistically supported.

Methods applied:

- Pearson Correlation
- Spearman Correlation
- Kruskal–Wallis Test
- Chi-square Test
- Effect Size Analysis
- Residual Analysis

The analysis emphasizes not only statistical significance but also practical significance through effect size interpretation.

---

### Stage 3 — Regression Modeling

Finally, multivariate linear regression models are built to evaluate how multiple behavioral variables jointly explain mental health outcomes.

The modeling process includes:

- baseline model
- train/test split
- model diagnostics
- residual analysis
- performance evaluation
- comparison between alternative model specifications

---

## Key Findings

The analysis revealed several important insights.

- Sleep duration demonstrates a positive association with mental health.
- Higher social media addiction scores are consistently associated with lower mental health scores.
- Relationship status has little practical influence on mental health.
- Academic level shows statistically significant but relatively small differences.
- Regression modeling explains a substantial proportion of variation in mental health, while also highlighting potential conceptual overlap between addiction measures and psychological outcomes.

---

## Tools & Technologies

Python, Jupyter Notebook, pandas, NumPy, Matplotlib, Seaborn, SciPy, scikit-learn

---

## How to Run

1. Clone the repository.
2. Install the required dependencies.

```bash
pip install -r requirements.txt
```

3. Open the notebooks in order:

- 01_eda.ipynb
- 02_statistical_analysis.ipynb
- 03_regression_model.ipynb

---

## Skills Demonstrated
- Exploratory Data Analysis
- Data Cleaning
- Data Visualization
- Statistical Inference
- Hypothesis Testing
- Effect Size Interpretation
- Regression Modeling
- Model Evaluation
- Business-Oriented Interpretation
- Scientific Reporting