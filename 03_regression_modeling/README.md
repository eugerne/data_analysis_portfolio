# Students’ Social Media Addiction & Mental Health
Regression Modeling Project

## Project Overview

This stage of the project extends the prior statistical analysis by implementing multivariate linear regression modeling to quantify the joint influence of behavioral factors on students’ mental health.

While the previous stage focused on statistical association and hypothesis testing, the current analysis introduces explanatory modeling to evaluate the independent contribution of behavioral variables and to assess predictive performance under a linear framework.

The emphasis remains on interpretability, model diagnostics, and conceptual validity rather than complex machine learning techniques.

## Modeling Objective

The primary outcome variable is Mental_Health_Score, a self-reported measure of student well-being on a 1–10 scale.

This stage addresses the following modeling questions:

- Do social media usage and sleep duration jointly explain variation in mental health?
- Does their effect remain stable under multivariate modeling?
- How does model performance compare to a naive mean baseline?
- What is the incremental impact of including social media addiction score?
- Does the addiction variable introduce conceptual overlap or multicollinearity?

## Dataset

The dataset consists of 705 student survey responses, including:

- Mental_Health_Score (1–10 scale)
- Avg_Daily_Usage_Hours
- Sleep_Hours_Per_Night
- Addicted_Score
- Relationship_Status
- Academic_Level
- Gender

All variables are self-reported and cross-sectional in nature.

## Methodology

The modeling process includes:

1. Baseline Specification

- Linear regression model with:
  - Avg_Daily_Usage_Hours
  - Sleep_Hours_Per_Night
- Train/test split (80/20)
- Naive mean baseline comparison

1. Model Evaluation

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² score
- Train vs test comparison (generalization check)

3. Diagnostic Analysis

- Actual vs Predicted plots
- Residuals vs Predicted plots
- Residual distribution assessment
- Overfitting evaluation

4. Extended Model Specification

- Inclusion of Addicted_Score
- Comparative performance analysis
- Coefficient stability assessment
- Conceptual overlap interpretation

## Key Findings

- The baseline behavioral model explains approximately 64% of the variance in mental health scores.
- Daily social media usage exhibits a strong negative independent effect.
- Sleep duration shows a positive but smaller effect under multivariate control.
- The model demonstrates stable generalization and no evidence of overfitting.
- Adding the addiction score increases predictive performance substantially (R² ≈ 0.89), but largely absorbs the explanatory power of other behavioral variables.
- The sharp performance increase likely reflects conceptual overlap between addiction and mental health constructs rather than an independent causal mechanism.

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

### Modeling

- scikit-learn
- LinearRegression
- train_test_split
- mean_squared_error
- r2_score

### Statistical & Modeling Concepts Applied

- Train/test validation
- Baseline comparison
- Multivariate regression
- Coefficient interpretation
- Multicollinearity effects
- Residual diagnostics
- Explanatory vs predictive modeling distinction

## Project Type

Explanatory regression modeling project focused on interpretability, specification comparison, and conceptual validity assessment.