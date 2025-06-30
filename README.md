# Gender Pay Gap & Compensation Disparity Analysis

This project investigates the **gender-based compensation gap** across roles and departments, using regression modeling and exploratory data analysis (EDA) to uncover systemic inequities in base pay, bonuses, and total compensation.

---

## Project Objective

- To quantify and analyze the impact of gender on total compensation, controlling for seniority, education level, and department.
- Explore how pay disparities evolve with career progression.

---

## Dataset Overview

- **Dataset:** `salary_data.csv`
- **Location:** `data/salary_data.csv`
- **Attributes Include:** 
  - Gender
  - Seniority level
  - Department
  - Education
  - Base Pay, Bonus, Total Compensation

---

## Methodology & ML Pipeline

### Preprocessing & EDA

- Data cleaning: missing values, inconsistencies addressed.
- Derived key metrics such as `TotalCompensation`.
- Generated exploratory visuals (bar plots, histograms, box plots).

### Statistical Modeling (OLS Regression)

**Regression Equation**:

```math
\text{TotalCompensation} = \text{Gender} + \text{Seniority} + \text{Education} + \text{Department} + (\text{Gender} \times \text{Seniority}) + (\text{Gender} \times \text{Education}) + (\text{Gender} \times \text{Department})
```

- Implemented using statsmodels.OLS.

- Interaction terms included to reveal compound effects.

- Evaluated model assumptions with residual and influence diagnostics.

### Key Findings & Insights
Persistent Gender-Based Bonus Gap: Men consistently earn higher bonuses than women, irrespective of performance.

Seniority Amplifies Disparities: Gender pay gaps widen significantly at higher seniority levels.

Educational Level Does Not Equalize Pay: Women earn systematically less than men even with advanced degrees.

Departmental Disparities Evident: Tech, sales, and administration departments display significant pay gaps.

Robust Statistical Evidence: Gender strongly predicts total compensation disparities even after controlling for seniority, education, and department.

### Repository Structure

gender-pay-gap-analysis/
├── data/
│   └── salary_data.csv
├── visuals/
│   ├── gender_plot_1.png
│   ├── gender_plot_2.png
│   ├── gender_plot_3.png
│   ├── gender_plot_4.png
│   ├── gender_plot_5.png
│   ├── gender_plot_6.png
│   ├── gender_plot_7.png
│   ├── gender_plot_8.png
│   ├── gender_plot_9.png
│   ├── gender_plot_10.png
│   ├── gender_plot_11.png
│   ├── gender_plot_12.png
│   ├── gender_plot_13.png
│   └── gender_plot_14.png
├── gender_pay_gap_analysis.ipynb
├── report_summary.pdf
├── requirements.txt
└── README.md

### Technology Stack
Programming Language: Python 3.10

Libraries: pandas, seaborn, matplotlib, statsmodels

Environment: Jupyter Notebook

### Business Relevance & Applications
Human Resources: Identifies biases in promotions, compensation policies, and bonus allocations.

Executive Management: Provides empirical insights for developing equitable compensation strategies.

Investors & ESG Analysts: Evaluates company practices related to social equity and inclusion.

### Potential Future Directions
Time-series analysis of pay gap evolution.

Sentiment analysis of employee reviews to correlate with compensation disparities.

Comparative industry analysis across various sectors.

### Author Information
**Don Richardson Bayya**
