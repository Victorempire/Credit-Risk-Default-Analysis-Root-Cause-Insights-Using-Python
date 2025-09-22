# Credit Risk Default Analysis:Root Cause Insights Using Python
# Overview
This project analyzes **credit risk defaults** using a dataset of 25,000 loan events across multiple branches, loan products, and officers. The analysis identifies key drivers of default, showing that lower credit scores, certain loan products (particularly SME and Personal Loans), and specific branches and officers are linked to higher default rates. Losses are concentrated, with a small number of defaults contributing disproportionately to total financial loss, highlighting areas that require attention.
Tests and analyses confirm these patterns: defaulters have significantly lower credit scores than non-defaulters, and defaults are strongly associated with branch, product type, and loan officer. Pareto analysis shows that just a few products account for most of the losses, revealing that risk is not evenly spread but concentrated in certain segments. These insights help focus efforts where they will have the greatest impact.
Based on the findings, the project recommends strengthening credit checks for borrowers with low scores, monitoring high-risk products and branches more closely, and reviewing lending policies to reduce exposure to large losses. Regular tracking of repayment trends and early identification of unusual patterns can also help prevent defaults. By taking these actions, financial institutions can reduce losses, improve product performance, and manage overall risk more effectively.
# Introduction
In today’s financial industry, lending institutions face one of their greatest challenges: managing the risk of loan defaults.
When customers fail to repay their loans, organizations not only lose revenue but also suffer from operational inefficiencies and strained resources.
To remain competitive, businesses must go beyond tracking numbers  they need to uncover why defaults happen, who is driving them, and what patterns exist beneath the surface.
The dataset contains customer credit scores, loan product types, branch performance, officer assignments, repayment behavior,
and financial losses. By analyzing these variables, we can ascertain the financial institution risk exposure and pinpoint the key drivers of default.
The goal of this project is not only to measure performance but also to conduct a **root-cause analysis of loan defaults** using statistical tests, visualization,
and anomaly detection. This provides a foundation for actionable insights helping decision-makers strengthen credit policies, optimize product offerings,
and improve portfolio risk management.
# Problem Statement
Loan defaults remain a critical threat to financial institutions, often arising from hidden patterns across products, customer profiles, or operational practices.
While raw data captures repayment outcomes, it rarely explains the underlying **root causes** of default. 
Without a structured analytical approach, organizations risk making decisions based on assumptions rather than evidence.
This project addresses that gap by systematically analyzing loan data to identify the most significant drivers of default, quantify their impact, and highlight actionable areas for risk mitigation.
# Objectives

The objectives of this project are to:
Identify key drivers of loan defaults through Pareto analysis (branches, product types, and loan officers).
Detect unusual repayment behaviors by applying anomaly detection on default trends.
Quantify differences in borrower creditworthiness using statistical tests (T-test on credit scores of defaulters vs non-defaulters).
Assess associations between categorical drivers and default rates using Chi-Square tests (branch, product type, and officer).
Provide actionable insights for strengthening credit policies, optimizing product offerings, and improving portfolio risk management.
# Hypotheses
### T-Test Hypotheses (Credit Score vs Default)
H₀ (Null): There is no significant difference in the mean credit scores of defaulters and non-defaulters.

H₁ (Alternative): The mean credit scores of defaulters are significantly lower than those of non-defaulters.
### Chi-Square Test Hypotheses (Categorical Drivers vs Default)
**Branch**

H₀: There is no significant association between branch location and default rates.

H₁: Branch location is significantly associated with default rates.

**Product Type**

H₀: There is no significant association between loan product type and default rates.

H₁: Loan product type is significantly associated with default rates.

**Loan Officer**

H₀: There is no significant association between loan officers and default rates.

H₁: Loan officers are significantly associated with default rates.

### The dataset contains the following key features:

Customer Features → Unique customer IDs and credit scores, allowing us to profile borrowers.

Loan Features → Product type, loan amount, and repayment outcomes, which show how lending decisions perform across customer segments.

Operational Features → Branches and officers responsible for loan disbursement, enabling performance tracking and accountability.

Performance Metrics → Financial losses (loss_ngn) linked to defaults, helping quantify the business risk.

Time Features → Loan dates and derived weekdays, which allow anomaly detection and time-based trend analysis.
