# insurance-charges-eda-regression
End-to-end exploratory data analysis, statistical feature engineering, and multiple linear regression to predict medical healthcare charges.
# Medical Insurance Charges Prediction

An end-to-end data analysis and machine learning workflow predicting individual healthcare insurance expenses using statistical feature engineering and multiple linear regression

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

---

## Overview

This project analyzes personal healthcare demographic data (age, sex, BMI, smoking status, region, and dependents) to isolate primary cost drivers and evaluate a predictive regression baseline

### Key Workflow Steps
* **Exploratory Data Analysis (EDA):** Feature distribution modeling via Seaborn/Matplotlib histograms, box plots, and correlation heatmaps
* **Feature Engineering:**
  * Categorical mapping and one-hot encoding for non-numeric features (`sex`, `smoker`, `region`)
  * Custom BMI binning into demographic categories (`underweight`, `normal`, `overweight`, `obese`)
* **Statistical Preprocessing:**
  * Standard scaling (`StandardScaler`) across continuous variables (`age`, `bmi`, `children`)
  * Pearson correlation coefficient ranking (`scipy.stats.pearsonr`) against target charges
* **Model Training & Evaluation:**
  * Multiple Linear Regression fitted on an 80/20 train-test split
  * Model evaluation using $R^2$ and Adjusted $R^2$ to control for multi-variable penalties.

---

## Results

* **Adjusted $R^2$ Score:** `~0.776`
* **Primary Cost Drivers:** Smoking status and categorized BMI index showed the highest statistical correlation with escalated medical costs

---

## Tech Stack

* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Modeling & Stats:** `scikit-learn`, `scipy`

---

## How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/aadiaaaa/](https://github.com/aadiaaaa/)<your-repo-name>.git
   cd <your-repo-name>
