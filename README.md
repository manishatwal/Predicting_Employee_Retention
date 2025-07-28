# Predicting Employee Retention (Logistic Regression Model)

This repository contains an end-to-end data science pipeline to predict **employee attrition** using a **Logistic Regression model**. The project provides HR departments with actionable insights to enhance employee retention and workforce stability.

---

##  Project Objective

To develop a predictive model that identifies the likelihood of employees leaving the organization based on demographics, job satisfaction, performance, and tenure features.

---

##  Business Goal

To assist HR teams in:

* Reducing employee turnover.
* Identifying key factors leading to attrition.
* Making data-driven decisions for improving employee satisfaction and retention.

---

##  ML Pipeline Highlights

### 1. Data Preparation

* Dataset: 74,610 rows × 24 columns.
* Features include: demographics, work experience, job satisfaction, performance ratings, etc.
* Missing values handled in `Distance from Home` and `Company Tenure` (\~5% dropped).
* Irrelevant columns like `Employee ID` were dropped.

### 2. Exploratory Data Analysis (EDA)

* **Univariate** and **bivariate** analysis using visualizations (histograms, count plots).
* **Class Balance**: Attrition levels were relatively balanced.
* **Correlation Analysis**: Low correlation among numerical features observed.

### 3. Feature Engineering

* One-hot encoding for all categorical variables.
* Feature scaling using `StandardScaler`.
* Recursive Feature Elimination (RFE) used to select top 15 predictors.

### 4. Model Development

* Logistic Regression using `statsmodels`.
* Key selected features include:

  * `Job Satisfaction_Low`, `Overtime_Yes`, `Remote Work_Yes`, etc.
* All predictors had statistically significant p-values.
* Variance Inflation Factor (VIF) analysis confirmed no multicollinearity.

### 5. Evaluation

* **Training Accuracy**: 0.74
* **Validation Accuracy**: 0.74
* **Sensitivity**: 0.75
* **Specificity**: 0.72
* **AUC**: 0.83
* **Precision**: 0.75

ROC curve and Precision-Recall curve were used to choose optimal threshold (0.5).

---

##  Business Recommendations

* Focus on improving **work-life balance** and **job satisfaction** to reduce attrition.
* Target interventions for **single employees** and **those with lower job levels**.
* Emphasize remote work and structured promotion pathways to retain talent.

---

##  Visualizations

* Histograms and count plots for EDA.
* Correlation heatmap.
* ROC and Precision-Recall curves.
* VIF table and model summary for feature evaluation.

---

##  Repository Contents

| File Name                                                  | Description                                         |
| ---------------------------------------------------------- | --------------------------------------------------- |
| `Predicting_Employee_Retention_Starter_Manish_Atwal.ipynb` | Full Jupyter Notebook implementation                |
| `Report_Manish_Atwal.pdf`                                  | Executive report with analysis summary and insights |

---

##  Author

**Manish Atwal**
