# Exploratory Data Analysis of Student Lifestyle

## Overview
This notebook performs an exploratory data analysis (EDA) of student lifestyle survey data to understand how demographic, behavioral, and lifestyle factors relate to students’ depression status. The analysis focuses on describing feature distributions, checking data quality, and visually exploring relationships between variables (including pairwise patterns).

## Dataset
The dataset is based on student survey responses and includes:
- **Demographics** (e.g., age, gender, country, academic level)
- **Lifestyle / behavior** (e.g., sleep duration, study hours, social media usage, physical activity)
- **Target / outcome**: a **binary depression indicator** (used for group comparisons)

Source: Kaggle — *Student Depression and Lifestyle (100k data)*

## Research questions
- How is depression distributed in the sample (class balance)?
- Do students with and without depression differ in lifestyle factors (sleep, social media, physical activity, etc.)?
- Are there visible pairwise relationships between stress and behavioral variables (linear or monotonic patterns)?
- Do the results suggest clear patterns at the level of exploratory visualization?

## What is inside the notebook
The notebook follows a standard EDA workflow:
1. **Data loading and quick inspection** (shape, head/sample, column types)
2. **Data quality checks** (missing values, plausibility of ranges)
3. **Univariate analysis** (distributions of numerical features; categorical counts where relevant)
4. **Target distribution** (depression class balance)
5. **Bivariate analysis**
   - **Boxplots**: feature distributions split by depression status
   - **Scatter plots / pairwise views**: visual inspection of relationships (e.g., stress vs lifestyle factors)
6. **Final EDA conclusions / key takeaways**

## Key findings (high-level)
- Numerical features show **plausible, well-behaved distributions** overall; no missing data were detected.
- Across the examined variables, **group-wise distributions for students with and without depression are highly similar**: medians and IQRs are close, and outliers (if present) do not appear group-specific.
- Pairwise scatter plots did **not** reveal clear linear/monotonic relationships between stress level and behavioral factors such as sleep duration, social media usage, or physical activity.
- Overall, **no strong patterns** associated with depression status are apparent through exploratory visualization alone; any potential relationships are likely subtle and require more formal statistical testing/modeling to detect.

## Tools and libraries used
- **Python** (Jupyter Notebook)
- **pandas / numpy**: data loading and manipulation
- **matplotlib / seaborn**: visualization (histograms, boxplots, scatter plots, pair plots)

## How to run
1. Install dependencies:
   - `pandas`, `numpy`, `matplotlib`, `seaborn`
2. Open the notebook:
   - `students_lifestyle_eda.ipynb`
3. Run cells top-to-bottom to reproduce outputs and plots.

## Notes / limitations
- This is **EDA**: results are descriptive and visual, not causal.
- If the depression classes are imbalanced, visual comparisons may look “similar” even when small effects exist; confirming subtle effects typically requires statistical testing and effect size reporting (handled in the later statistical analysis project).