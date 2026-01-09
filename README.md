# 🏢 Employee Retention Analysis: Salifort Motors
### Google Advanced Data Analytics Professional Certificate | Capstone Project

<p align="left">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Analytics-HR--Insight-blueviolet?style=for-the-badge" alt="HR Analytics">
  <img src="https://img.shields.io/badge/Random_Forest-008000?style=for-the-badge" alt="Random Forest">
</p>

---

## 📌 Project Overview
Salifort Motors is experiencing high employee turnover. The goal of this project was to analyze human resources data to uncover the key factors driving attrition and build a predictive model to identify employees at risk of leaving.

The project follows the **PACE** (Plan, Analyze, Construct, Execute) framework to provide data-driven recommendations to the HR department for improving employee satisfaction and retention.

---

## 🛠️ Data Science Pipeline (PACE)

### 1. Plan & Analyze (EDA)
During the initial exploration of the dataset, several critical patterns emerged regarding why employees leave:
* **The Overwork Correlation:** Employees working more than 240 hours/month showed significantly higher turnover rates.
* **The 4-Year Itch:** A notable spike in attrition occurs at the 4th year of tenure, often coinciding with high project loads.
* **High-Performer Burnout:** Employees with the highest evaluation scores were frequently the ones working the most hours, making them a high-risk group for resignation.

### 2. Feature Engineering
To improve model accuracy and business relevance, I engineered and refined several features:
* **`overworked`**: A binary feature identifying employees working excessive hours (above 175/month) on high project volumes.
* **Leakage Prevention**: Removed `satisfaction_level` from the final model to ensure the prediction was based on observable operational data (hours, projects, tenure) rather than subjective surveys.

### 3. Modeling & Evaluation
I implemented multiple machine learning models, with the **Random Forest (Round 2)** emerging as the champion.

| Metric | Score |
| :--- | :---: |
| **Precision** | 0.94 |
| **Recall** | 0.89 |
| **F1-Score (Champion)** | **0.91** |

> **Model Insight:** The model is highly effective at identifying the specific operational conditions—project volume and excessive hours—that lead to turnover.



---

## 📈 Key Insights & Business Recommendations

Based on the model's findings, overwork is the primary driver of attrition at Salifort Motors. I propose the following actionable steps:

* **🚨 Workload Capping:** Limit employees to a maximum of **5 concurrent projects** to prevent burnout.
* **⏱️ Hours Monitoring:** Flag employees working more than **175 hours/month** for immediate manager check-ins and workload redistribution.
* **💎 Tenure Incentives:** Create specific career-growth programs or 'stay-bonuses' for employees reaching the **3-year and 4-year marks**.
* **📈 Evaluation Alignment:** Re-examine the workload of **'High Performers'**. Current metrics reward overwork, which is currently driving the company's best talent away.

---
*This project was completed as the final Capstone for the Google Advanced Data Analytics Professional Certificate.*
