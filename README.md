# COMPAS Fairness Audit

## Individual Homework 3



### A) Purpose of the Analysis



This repository contains a fairness audit of the COMPAS risk assessment model using the cleaned dataset and prediction outputs developed in Lecture 02. The analysis evaluates whether model outcomes exhibit disparities across protected demographic groups using legally grounded fairness metrics aligned with EEOC guidance and the burden-shifting framework.



The Python notebook implements the following analytical workflow:



1. Creation of a binary decision outcome variable (high-risk classification) from COMPAS score categories
2. Computation of Adverse Impact Ratio (AIR) across race and sex relative to designated reference groups
3. Estimation of Marginal Effect (ME) using logistic regression to assess statistical significance of subgroup differences
4. Calculation of Standardized Mean Difference (SMD) to measure effect-size differences in predicted risk scores
5. Intersectional fairness analysis combining race and sex categories to identify the worst-off subgroup
6. Evaluation of False Positive Rate (FPR) and False Negative Rate (FNR) disparities across racial groups
7. Statistical testing of FPR and FNR differences using two-proportion z-tests
8. Visualization of subgroup error-rate disparities using grouped bar charts for publication-quality reporting
9. Preparation of a regulatory-style compliance memo interpreting findings under the burden-shifting framework



Results indicate measurable disparities across demographic groups under multiple fairness metrics. Intersectional analysis identifies the subgroup with the lowest selection rate relative to the reference category, demonstrating the importance of evaluating fairness across combined protected attributes rather than single attributes alone.



### B) Python Libraries Used


B) Python Libraries Used
1) Pandas- Data cleaning, subgroup filtering, and aggregation
2) Numpy- Numerical operations and statistical calculations
3) Matplotlib- Visualization of fairness metrics
4) Statsmodels	Logistic regression for Marginal Effect estimation
5) Solas-disparity	Computation of AIR fairness metric
6) Scipy / statsmodels.stats	Two-proportion z-tests for error-rate comparison




### 

### C) Instructions for Reproducing the Results (Google Colab)

1\) Open Google Colab

2\) Upload Individual\_Assignment\_3\_Ria\_Mathur.ipynb

3\) Run all cells using Runtime → Run all

