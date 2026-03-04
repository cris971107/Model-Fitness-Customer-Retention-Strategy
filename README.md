# Model Fitness: Data-Driven Customer Retention
The "Model Fitness" gym chain is developing a data-driven strategy to combat customer churn. This project analyzes digitalized customer profiles to predict the probability of attrition for the next month

---

## ⚙️ Project Type Flags

- [x] Exploratory Data Analysis (EDA)
- [ ] SQL Analysis / Querying
- [ ] Dashboard / Data Visualization
- [ ] Data Pipeline / ETL
- [x] Predictive Modelling / Machine Learning
- [x] Data Cleaning / Wrangling
- [ ] End-to-End (multiple of the above)
- [ ] Other: ___________

---

## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Repository Structure](#3-repository-structure)
4. [Data Processing & Methodology](#4-data-drocessing-and-methodology)
5. [Key Insights](#5-key-insights)
6. [Deliverables](#6-deliverables)
7. [Final Verdict & Recommendations](#8-final_recomendations)
8. [Author](#7-author)

---

## 1. Project Overview

This project focuses on analyzing customer behavior for the "Model Fitness" gym chain to combat churn (customer attrition). By analyzing digitalized user profiles, the goal is to predict the probability of loss for the next month, identify typical user segments, and design a data-driven retention strategy.

---

## 2. Objectives

Primary Objective:
Develop a binary classification model to predict the likelihood of customer churn for the upcoming month, enabling proactive intervention.

Secondary Objective 1:
Perform user segmentation using unsupervised learning (K-means clustering) to create detailed personas and understand the distinct characteristics of loyal vs. at-risk members.

Secondary Objective 2:
Identify and analyze the key factors that impact retention, such as social ties, age, and gym usage, to provide actionable recommendations for the marketing and customer service teams.


---

## 3. Repository Structure

```
[project-root]/
│
├── docs/                     # Original, unmodified source data - never edited
│
├── notebooks/                # Jupyter, R Markdown, or Colab notebooks
│
└── visuals/                  # Exported charts, dashboard screenshots, ERD diagrams


```



---



## 4. Data processing and methodology

The dataset includes user data from the previous month, visit logs, and current membership status.

Exploratory Data Analysis (EDA): Cleaned the dataset and analyzed mean values for Churn vs. Non-Churn groups.

Predictive Modeling: Compared Logistic Regression and Random Forest models. Evaluated performance using Accuracy, Precision, and Recall metrics.

User Clustering: * Standardized features and created a distance matrix (dendrogram).

Applied K-means (n=5) to group users by behavioral patterns.

Correlation Analysis: Built a correlation matrix to identify features with high impact on the target variable (Churn).

# Methods Used

Descriptive statistics for event distribution per user.

Funnel analysis (Login -> Product Page -> Cart -> Purchase).

Z-test for independent proportions (Alpha = 0.05).

`visuals/Captura de pantalla 2026-03-04 000520.png`


<img width="1237" height="347" alt="Captura de pantalla 2026-03-04 000520" src="https://github.com/user-attachments/assets/099547b0-04fa-453f-9509-09ed71cd0560" />

---


## 5. Key insights

<!--
  Findings + implications. Not just what happened - what it means.

  WHAT GOOD LOOKS LIKE:
  ✅ "Return rates, not sales volume, explain Region A's underperformance.
      Region A's return rate on home goods was 34% - more than double the
      company average. Revenue was not lost at the point of sale; it was
      lost post-sale through refunds. This points to a fulfilment or
      product quality issue specific to that region, not a demand problem."

  WHAT TO AVOID:
  ❌ "Region A had lower revenue than other regions in Q4."
     (That's an observation. It describes what happened.
      An insight says what it means and where to look next.)

  Aim for 3–6 insights. Quality over quantity.
-->

The analysis reveals that the most at-risk customers are typically younger individuals (averaging 26-27 years old) who join the gym without social ties, such as "Bring a Friend" promotions or corporate partner discounts. These users tend to work or live further away from the facility and rarely participate in group sessions, leading to a lack of community integration. In contrast, loyal members are generally older (30+), live or work in the immediate vicinity, and are highly engaged in group activities. Proximity and social engagement emerge as the strongest predictors of long-term commitment, suggesting that churn is largely driven by a lack of social habit and the physical inconvenience of distance.

`visuals/Captura de pantalla 2026-03-03 234335.png`
<img width="1013" height="541" alt="Captura de pantalla 2026-03-03 234335" src="https://github.com/user-attachments/assets/2779e75f-c676-41e7-954f-43ae299933a9" />

---


## 6. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| Code | Jupyter Notebook containing EDA, Funnel Visualizations, and Z-test results. | `notebooks/Sprint-15S-2.ipynb` |



---


## 7. Final verdict and recommendations

Verdict: The Random Forest model provided the best balance of precision and recall for predicting churn. Social engagement and location remain the strongest predictors of long-term loyalty.

Recommendations: * Targeted Social Programs: Create referral incentives for younger members to increase their "Social Ties."

Group Class Onboarding: Focus on converting solo members into group session participants during their first month.

Location-Based Ads: Focus marketing efforts on a tight radius around the gym to attract members with higher "Near_Location" scores.

---


## 8. Author

**Cristian Barrientos**

- 🔗 [https://www.linkedin.com/in/cristian-barrientos-pomposo/](https://www.linkedin.com/in/cristian-barrientos-pomposo/)
- 💼 [https://github.com/cris971107](https://github.com/cris971107)
- 📧 cristian971107@hotmail.com



