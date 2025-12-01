# 📚 Assessing Professor Effectiveness (APE)

This repository contains a data science project that analyzes RateMyProfessor data to uncover rating patterns, identify potential biases, and build predictive models for professor evaluation outcomes.

---

## 📦 Repository Content

- Full data analysis pipeline
- Complete Python implementation
- Detailed project report with figures and statistical results

---

## 🚀 Project Highlights

- Hypothesis testing across gender, experience, and online teaching
- Correlation analysis of rating, difficulty, and take-again rate
- Regression modeling (simple & multivariate)
- Ridge regression to handle multicollinearity
- Logistic regression models for predicting “pepper” (hotness)
- ROC curves, beta comparisons, and significance testing
- Extra insight using qualitative attributes (professor majors)

---

## 📊 Dataset

**89,893 professors** compiled from RateMyProfessor.  
Two synchronized datasets:

- **Numerical features:**  
  - Average rating  
  - Average difficulty  
  - Number of ratings  
  - Percent of students who would take again  
  - Number of online ratings  
  - Gender indicators (male, female)  
  - Pepper (hotness) indicator  

- **Qualitative features:**  
  - Major / Field  
  - University  
  - U.S. state  

---

## 🧠 Method Summary

**Preprocessing**
- Merged numerical + qualitative datasets
- Removed rows with extreme missingness
- Median imputation for numerical variables
- Cleaned ambiguous gender entries
- Applied reproducible random seed
- Used α = 0.005 for all significance tests

**Statistical Analysis**
- Mann–Whitney U tests for gender bias & online teaching impact
- Correlation & regression for rating–difficulty and rating–take-again
- Group comparisons for experience effects
- Boxplots, scatter plots, and distribution visualizations

**Regression Modeling**
- Model 1: Rating ← Difficulty only
- Model 2: Rating ← All predictors (Ridge Regression)
- Demonstrates improvement in R² and RMSE with multivariable modeling

**Classification Modeling**
- Logistic regression for predicting “pepper” indicator  
  - Model A: Using rating only  
  - Model B: Using all features  
- Evaluation via accuracy, precision, recall, F1, and ROC-AUC
- Class imbalance considered during interpretation

**Extra Insight**
- Major-level analysis finds highest/lowest rated academic fields
- Reveals rating patterns not visible from numerical data alone

(Visualizations and detailed results are included in the project report.)

---

## 📊 Key Findings (High-Level)

- **Gender Bias:** Male professors receive significantly higher ratings
- **Experience Effect:** More-experienced professors rated higher
- **Difficulty Relationship:** Higher difficulty → lower rating
- **Online Teaching:** Heavy online teaching → lower average ratings
- **Pepper Model:** Full-feature classification slightly improves AUC over rating-only model
- **Major Insight:** Strong differences in ratings across academic fields

---

## 📝 Summary

This project demonstrates how statistical inference and machine learning can extract insights from large-scale human rating data. Through rigorous testing, regression, and predictive modeling, the analysis identifies meaningful rating patterns and provides interpretable, data-driven conclusions about professor effectiveness.

---
