Stroke Risk Analysis Dashboard
Project Overview

This project focuses on cleaning, preparing, and visually analyzing a healthcare dataset related to stroke risk.
The goal is to create a clear and interpretable Tableau dashboard that highlights how demographic and clinical factors are associated with stroke occurrence.

🔗 Interactive Dashboard (Tableau Public):
https://public.tableau.com/app/profile/rayan.ra4401/viz/StrokeRiskAnalysisDashboard_17657359236590/Dashboard1

Dataset

The dataset contains demographic, lifestyle, and clinical variables, including:

Age

Gender

Body Mass Index (BMI)

Average glucose level

Hypertension

Heart disease

Smoking status

Work type

Stroke outcome (binary)

The data was treated as observational, and all original categories were preserved.

Data Cleaning

The following cleaning steps were performed:

Structural inspection using info(), describe(), shape, and missing-value checks

Missing values in BMI were imputed using the median, which is appropriate for skewed continuous health data

Duplicate records were checked; no duplicates were removed

Categorical variables were reviewed using frequency counts without semantic modification

These steps follow standard data-preparation practices recommended for health datasets.

Feature Engineering

To improve interpretability and analysis:

Age was divided into five groups:
Child, Young Adult, Adult, Middle Age, Senior

A Risk Score was computed by aggregating key clinical risk indicators:

Hypertension

Heart disease

High glucose level

High BMI

Older age

A Risk Level (Low, Medium, High) was derived from the Risk Score

All engineered features were created strictly for analytical purposes.

Exploratory Analysis

Exploratory Data Analysis (EDA) included:

Descriptive statistics for numerical variables

Distribution analysis for categorical variables

Pearson correlation analysis among numeric features

Focus on rates and proportions rather than raw counts to allow fair comparison across groups

Dashboard Description

The Tableau dashboard presents:

Key KPIs (total records, total strokes, mean age, mean BMI)

Stroke rate by age group and gender

Risk-level distribution across work types

Visual summaries highlighting how stroke risk increases with age

Interactive filters for demographic and risk-related variables

The dashboard is designed for clarity, accessibility, and healthcare-style reporting.

Key Observations

Stroke risk increases sharply with age, with the highest rates among individuals aged 65 and above

Stroke rates between males and females are similar in this dataset

Higher stroke counts in the private work sector reflect group size rather than higher individual risk

The Risk Score effectively summarizes multiple health conditions into clear risk categories

Tools & Technologies

Python (Pandas, Matplotlib, Seaborn) – data cleaning and analysis

Tableau Public – dashboard creation and visualization

References

World Health Organization – Stroke
https://www.who.int/news-room/fact-sheets/detail/stroke

World Health Organization – Body Mass Index (BMI)
https://www.who.int/data/gho/data/themes/theme-details/GHO/body-mass-index-(bmi)

Pandas Documentation – Data Cleaning
https://pandas.pydata.org/docs/user_guide/missing_data.html

CDC – Data Visualization Best Practices
https://www.cdc.gov/dataviz/index.html
