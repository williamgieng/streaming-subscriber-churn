# Predicting Early Subscriber Churn in a Streaming Service

This repository contains a Staff / FAANG-level portfolio case study analyzing early
subscriber churn in a subscription-based streaming service. The analysis focuses on
understanding early churn drivers and identifying opportunities for targeted retention
interventions.

## Overview
- Dataset: ~29.7K subscribers (Jan–Apr 2023 cohort)
- Focus: Early churn (Month 1) vs retained subscribers
- Signals: Engagement, acquisition, billing, and lifecycle behavior
- Methods: Survival analysis, interpretable modeling, Random Forest comparison

## Key Findings
- Churn is heavily concentrated in the **first month**
- High early engagement does **not** guarantee retention (“binge-and-leave” behavior)
- Signup platform and acquisition biller materially impact survival
- Even simple models can effectively prioritize high-risk cohorts

## Repository Contents
- 📓 **Notebook:** [`notebooks/churn_analysis.ipynb`](notebooks/churn_analysis.ipynb)
- 📊 **Slides:** [`slides/streaming_churn_case_study.pdf`](slides/streaming_churn_case_study.pdf)

## Modeling Approach
- Logistic Regression as an interpretable baseline
- Random Forest for non-linear comparison
- Proper preprocessing with pipelines and imputation (leak-safe)

## Notes
- Survival curves are smoothed, capped at April 2023, and labeled for interpretability
- Data is synthetic/anonymized; no proprietary or confidential data is included
