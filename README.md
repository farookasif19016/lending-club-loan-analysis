# Loan Risk & Credit Portfolio Analysis — LendingClub Dataset

## Project Overview

This end-to-end data analytics project investigates how borrower risk characteristics influence loan default behaviour, portfolio exposure, and loan pricing within a fintech lending environment. Using 39,000+ LendingClub loan records, the analysis focuses on identifying default drivers, evaluating borrower risk segments, and understanding how lending decisions impact portfolio stability and financial risk.

The project combines exploratory data analysis, data cleaning, validation, statistical reasoning, and business-focused analysis to simulate a real-world credit risk investigation workflow.

## Business Objectives

The analysis was designed to answer the following lending and portfolio-risk questions:

Which borrower characteristics most strongly influence interest rates?
Which borrower segments contribute disproportionately to charge-offs and default risk?
Does verification status genuinely influence default behaviour, or are underlying risk variables driving the relationship?
How are portfolio losses concentrated across borrower grades and risk segments?
Which variables appear to be strong vs weak indicators of borrower default risk?

## Analytical Approach

The project followed a structured analytical workflow commonly used in fintech and lending analytics:

Business understanding and risk framing
Exploratory Data Analysis (EDA)
Data cleaning and preprocessing
Data validation and consistency checks
Borrower segmentation and risk analysis
Portfolio-level business interpretation
Dashboard visualisation in Power BI
Tools & Technologies
Python — data analysis workflow
Pandas — cleaning, manipulation, aggregation
Jupyter Notebook — analysis environment
Power BI — dashboard and visual storytelling
Dataset Information
Source: Kaggle LendingClub Loan Dataset
Original dataset: 39,717 rows × 111 columns
Final analytical dataset: 39,715 rows × 49 validated columns

The dataset contains borrower financial profiles, loan characteristics, repayment behaviour, interest rates, verification status, and charge-off outcomes.

## Data Cleaning & Validation

The project included:

Removal of fully empty and low-value columns
Missing value treatment using median, mode, zero-fill, and logical handling
Data type correction for percentage-based variables
Range validation for loan amounts, DTI, and interest rates
Consistency validation between funded amounts, grades, and pricing behaviour
Validation of borrower segmentation logic before analysis

Examples of validation checks:

Interest rates must remain between 0–100%
Funded amount cannot exceed loan amount
Higher loan grades should correspond to higher average interest rates
Negative DTI and impossible loan values investigated separately

## Key Business Findings
## 1. Loan Grade Is the Strongest Risk Indicator

Loan grade showed the clearest relationship with both interest rate pricing and charge-off behaviour.

Grade A borrowers averaged 7.33% interest rates
Grade G borrowers averaged 21.31%
Charge-off rates increased materially across lower grades

This suggests the grading system effectively captures borrower risk and plays a central role in underwriting and pricing decisions.

## 2. Portfolio Losses Are Concentrated in Lower-Grade Borrowers

Overall charge-off rate across completed loans was approximately 14.58%, meaning nearly 1 in 7 borrowers defaulted.

Charge-off behaviour accelerated significantly from Grade D onward, indicating a potential portfolio risk threshold where losses begin increasing disproportionately.

This highlights the importance of controlling exposure concentration within higher-risk borrower segments.

## 3. DTI Alone Was a Weak Standalone Predictor

Although charged-off borrowers showed slightly higher DTI levels, the difference between charged-off and fully paid borrowers was relatively small.

This suggests:

DTI alone has limited predictive power
Affordability pressure may not independently explain default behaviour
Additional behavioural and credit-risk variables are required for stronger risk assessment

## 4. Income Stability Influences Repayment Behaviour

Charged-off borrowers earned approximately 10.6% less on average compared to fully paid borrowers.

Charged-off average income: ~£62,427
Fully paid average income: ~£69,862

While income was not the strongest predictor independently, lower income levels appeared associated with weaker repayment stability.

## 5. Home Ownership Correlates with Repayment Stability

Renters defaulted more frequently than mortgage holders.

This may indicate that borrowers with greater long-term financial stability or established financial profiles demonstrate more consistent repayment behaviour.

Home ownership status may therefore provide additional segmentation value during borrower risk assessment.

## 6. Surface-Level Correlations Can Be Misleading

Initial analysis suggested that verified borrowers defaulted more frequently.

However, further segmentation showed that loan grade — rather than verification status itself — was the primary underlying driver of elevated charge-off rates.

This demonstrates the importance of deeper segmentation analysis before drawing causal conclusions from surface-level correlations.

## 7. Small Business Loans Carry Higher Pricing Risk

Small business loans exhibited some of the highest average interest rates within the portfolio.

This likely reflects:

unpredictable revenue patterns
higher operational uncertainty
elevated repayment risk compared to standard consumer borrowing

The finding highlights how lenders incorporate uncertainty into risk-based pricing strategies.

## Credit Risk Concepts Applied

The project explored several core fintech and lending-risk concepts:

Probability of Default (PD)
Exposure at Default (EAD)
Loss Severity / Loss Given Default (LGD)
Delinquency and charge-off behaviour
Portfolio exposure concentration
Borrower segmentation
Risk-based pricing
Underwriting quality and portfolio deterioration

## Dashboard Preview

The Power BI dashboard was designed to visualise:

default distribution across borrower grades
interest rate segmentation
borrower income and DTI comparisons
charge-off concentration
portfolio-level risk trends

<img width="1169" height="657" alt="image" src="https://github.com/user-attachments/assets/20dde0c6-1f0a-47d0-af5c-66971b6ec431" />
<img width="1164" height="657" alt="image" src="https://github.com/user-attachments/assets/3fb23a92-6a60-47a8-887a-c5f0b044c3a5" />
<img width="1164" height="656" alt="image" src="https://github.com/user-attachments/assets/7290a03b-724d-44bb-8084-4f7801faaf90" />

## Project Structure

notebook/     -> Full Python analysis workflow
data/         -> Cleaned and validated dataset
dashboard/    -> Power BI dashboard (.pbix)

## Dataset
LendingClub loan data sourced from Kaggle — 39,717 rows, 111 original columns 
reduced to 49 analytical columns after cleaning and validation.

## Key Takeaways

This project demonstrates:

structured analytical thinking
fintech and lending-domain understanding
portfolio-risk reasoning
borrower segmentation analysis
business-focused interpretation of financial datasets

Beyond technical analysis, the project focuses on explaining how borrower characteristics influence lending risk, pricing behaviour, and portfolio stability within a real-world fintech context.
