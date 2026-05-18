# Loan Risk & Borrower Analysis — LendingClub Dataset

## Project Overview
End-to-end data analysis project examining 39,000+ LendingClub loan records 
to identify borrower risk profiles, default drivers, and interest rate factors 
in a fintech lending context.

## Business Questions
1. What factors most strongly correlate with higher interest rates?
2. Which borrower profile has the highest likelihood of default?
3. Does verification status correlate with charge-off outcomes?

## Tools Used
- Python — EDA, data cleaning, validation, analysis
- Pandas — data manipulation
- Power BI — interactive dashboard
- Jupyter Notebook — development environment

## Key Findings
- Loan grade is the strongest predictor of both interest rate and default risk
- Grade A borrowers pay 7.33% interest vs Grade G at 21.31% — nearly 3x more
- 14.58% overall charge off rate — nearly 1 in 7 borrowers defaulted
- Grade D is the risk threshold — charge off rate exceeds 20% from Grade D onwards
- Charged off borrowers earn 10.6% less on average — £62,427 vs £69,862
- Verified borrowers default more on the surface — but grade is the real driver
- Small business loans attract highest interest rates due to unpredictable revenue

## Project Structure
- notebook/ — Jupyter notebook with full Python analysis
- data/ — cleaned and validated dataset
- dashboard/ — Power BI .pbix file

## Dashboard Preview
<img width="1169" height="657" alt="image" src="https://github.com/user-attachments/assets/20dde0c6-1f0a-47d0-af5c-66971b6ec431" />
<img width="1164" height="657" alt="image" src="https://github.com/user-attachments/assets/3fb23a92-6a60-47a8-887a-c5f0b044c3a5" />
<img width="1164" height="656" alt="image" src="https://github.com/user-attachments/assets/7290a03b-724d-44bb-8084-4f7801faaf90" />

## Dataset
LendingClub loan data sourced from Kaggle — 39,717 rows, 111 original columns 
reduced to 49 analytical columns after cleaning and validation.
