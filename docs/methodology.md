# Methodology / Методика

This document describes the approach evidenced by the four supplied research notebooks. It is **not a copy of proprietary code**.

| Stage | Inputs and methods | Output |
|---|---|---|
| 1. Data profiling | Excel-based tables, numeric conversion, missingness, IQR outliers, boxplots | Data-quality summaries |
| 2. Factor selection | Spearman rank correlation, correlation between predictors, Logistic Regression, Decision Trees, Random Forest, Gradient Boosting | Ranked features and model comparisons |
| 3. Threshold estimation | DecisionTreeRegressor split points, Mann–Whitney comparison, effect estimates, bootstrap intervals | Candidate thresholds and significance checks |
| 4. Risk reporting | Ridge / Random Forest / Gradient Boosting regression comparisons; threshold-based flags and rule aggregation | Explainable Excel risk report |

## Decision-support principle

The system uses geological and technical attributes already available before the workover to identify combinations of risk factors. A flag count offers **decision support**, not automatic operational authorization. Domain review is essential.

## Distinguishing the methods

- **Correlation** describes association; it does not prove causation.
- **Threshold rules** are interpretable but need calibration on independent observations.
- **Regression** aims to predict duration; reported cross-validation did not establish stable high accuracy.
- **Recommendations** reflect an analytical rule and are not a replacement for engineering approval.

## Reproducibility

The original notebooks reference production spreadsheets that are not distributed in this portfolio. Thus a third party cannot reproduce the original fitted values from this repository alone. A future public demonstration should use explicitly generated synthetic data and clearly labeled example results.
