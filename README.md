# Banking-Analysis
A comprehensive data analysis and visualization project focused on risk analytics in banking and financial services, designed to explore how data can minimize the risk of losing money while lending to customers
# problem statment
Develop a basic understanding of risk analytics in banking and analyze how financial institutions can leverage data to make informed lending decisions.
# Dataset we used for analysis
- <a href="https://github.com/VivekMane57/Banking-Analysis/blob/main/Banking.xlsx">Dataset</a>
# The dataset contains multiple interlinked tables with banking and client details:
Banking Relationship
Client-Banking
Gender
Investment Advisor
Period

# ✅ Solution
We built interactive Power BI dashboards that analyze client profiles and provide insights into:
If an applicant is likely to repay a loan.
Total deposits, loans, and fees at client and bank levels.
Segmentation of customers by income bands and engagement length.
Banking KPIs like deposits, savings, credit card balances, and business lending

# Data Cleaning & Feature Engineering
Created Engagement Timeframe column for client-bank relationships.
Added Engagement Days (time since joining).
Binned Estimated Income into Low (<100k) and Mid (<300k).
Introduced Processing Fees column (based on fee structure).

# Calculated Functions
SUM → e.g., Bank Deposit = SUM('Clients - Banking'[Bank Deposits])
DISTINCTCOUNT → e.g., Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])
SUMX → e.g., Total Fees = SUMX('Clients - Banking', [Total Loan] * [Processing Fees])
DATEDIFF → e.g., Engagement days per client

# KPIs & Metrics
Total Clients
Total Loan (Bank Loan + Business Lending + Credit Cards Balance)
Total Deposits (Bank Deposits + Savings + Foreign Currency + Checking Accounts)
Total Fees
Checking, Savings, and Foreign Currency Accounts
Credit Card Balances & Business Lending

# Dashboards
Loan Analysis
<img width="1327" height="741" alt="image" src="https://github.com/user-attachments/assets/b151c65e-28d5-4252-b056-56c423bc6f7e" />

Deposit Analysis
Summary Dashboard
Home Dashboard
