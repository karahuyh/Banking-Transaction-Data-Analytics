<div align="center">
  
# Banking Transaction Data Analytics

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white)
![JupyterLab](https://img.shields.io/badge/JupyterLab-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

## 📖 Project Overview

This project is a retail banking transaction analytics with 20,000 synthetic transactions across products like checking/saving accounts, loans, mortgages, and credit cards, spanning Jan 2023 - May 2026, across 8 Spanish cities and 4 channels (Mobile, Branch, ATM, Online).

The objective is to uncover customer behaviour, transaction patterns, revenue drivers, and operational insights that banks can use to make better business decisions.

The analysis aims to help the bank:
- Personalize financial products and services.
- Assess customer profitability and risk.
- Improve marketing campaigns.
- Optimize branch and transactional channel performance.
- Increase customer engagement and retention.

## Project Questions:
**1. Customer insights & Segmentation**
- Which customer segment (e.g., High Income vs. Low Income) performs the most transactions?
- Which financial products are most popular within each customer segment?
- Is there a relationship between customer credit score and transaction frequency/total accumulated fees?

**2. Transaction Behaviour Analysis**
- Which transaction type contributes the highest? (number of transaction or transaction value)
- Which branch cities are transaction hotspots and which underperform?
- How do customers differ in using mobile banking/ATM/branch services?

**3. Revenue & Cost insights**
- Which transaction types generate the most fee revenue (e.g., credit card fees, insurance fees, late payment fees)?
- Are certain customer groups paying disproportionately high fees?
- Which recurring customer frictions also generate significant revenue?
  
**4. Trend & Performance Analysis**
- Are there seasonal or monthly transaction trends?
- Are the recommended banking offers aligned with customer needs and behaviours?
- What emerging trends appear across customer segments or transactional channels over time?
  
## 📶 Dataset Snapshot
The dataset contains 20,000 transaction records with 19 columns (Data dictionary in **Appendix 1**)

| Column  | Values |
| ------------- | ------------- |
| TransactionID  | 20,000  |
| CustomerID  | 8,025  |
| Time Span  | 01-01-2023 to 20-05-2025  |
| Total Amount USD | $109,578,807  |
| Total Fee Revenue USD | $691,286  |
| Total Credit Card Fees USD | $113,266  |
| Total Insurance Fees USD | $216,512  |
| Total Late Payment Amount USD | $361,509 |
| Transactions with any fee | 10,106 (50.5%)  |
| Reporting Currency | USD (post-cleaning) |

### Column Types
| Type  | Columns |
| ------------- | ------------- |
| Identifiers  | 	TransactionID, CustomerID  |
| Datetime  | 	TransactionDate  |
| Categorical  | 		TransactionType, ProductCategory, ProductSubcategory, BranchCity, Channel, Currency, CustomerSegment, RecommendedOffer  |
| Numeric  | 		Amount, CreditCardFees, InsuranceFees, LatePaymentAmount, CustomerScore, MonthlyIncome, BranchLat, BranchLong  |

### Categorical breakdown
| Field | Number of Categories | Values |
|---|---:|---|
| TransactionType | 6 | Card Payment, Deposit, Fee, Loan Payment, Transfer, Withdrawal |
| ProductCategory | 5 | Checking Account, Credit Card, Loan, Mortgage, Savings Account |
| ProductSubcategory | 5 | Business, Gold, Platinum, Standard, Student |
| BranchCity | 8 | Madrid, Barcelona, Valencia, Seville, Zaragoza, Malaga, Murcia, Bilbao |
| Channel | 4 | ATM, Branch, Mobile, Online |
| CustomerSegment | 3 | High / Middle / Low Income Segment |
| RecommendedOffer | 7 | Exclusive Platinum Package, Premium Investment Services, Mid-tier Savings Booster, Gold Card w/ Travel Benefits, Financial Literacy Program Access, Personal Loan Cashback Offer, No-Fee Basic Account |





# Steps
1. Assess data quality (Appendix 2 and 3)
2. Convert all EUR transactions to USD using [Google Finance](https://www.google.com/finance/beta/quote/EUR-USD) fixed exchange rate (Jul 2026) of 1 EUR = 1.10 USD (Appendix 4)
3. Use to converted dataset to design dashboards and visualisations


# Power BI Dashboard:
Link

# Key Findings

# Limitations

# Future Improvements



# List of Appendices
### Appendix 1. Dictionary 
| Column Name  | Description |
| ------------- | ------------- |
| TransactionID  | Unique identifier for each transaction  |
| CustomerID  | Unique identifier for each customer  |
| TransactionDate  | Date when the transaction occured  |
| TransactionType  | Type of transaction (e.g., Deposit, Withdrawal, Transfer, Card Payment, Fee) |
| Amount  | Monetary value of the transaction  |
| ProductCategory  | Category of the financial product involved in the transaction |
| ProductSubcategory  | Subcategory within the product category  |
| BranchCity  | City where the transaction occured or branch is located  |
| BranchLat  | Latitude of the branch location  |
| BranchLong  | Longtitude of the branch location  |
| Channel  | Channel used for the transaction (e.g., Branch, ATM, Mobile |
| Currency  | Currency in which the transaction was made  |
| CreditCardFees  | Fees incurred from credit card usage  |
| InsuranceFees | Insurance-related fees associated with the transaction  |
| LatePaymentAmount  | Fees incurred from credit card usage  |
| CustomerScore  | Customer's credit score or internal rating  |
| MonthlyIncome  | Customer's reported monthly income  |
| CustomerSegment  | Customer's assigned income segment  |
| RecommendedOffer  | Product or offer recommended to the customer  |

### Appendix 2. Checked for nulls
<div align="center">

<img width="526" height="498" alt="Screenshot 2026-07-06 at 5 19 48 PM" src="https://github.com/user-attachments/assets/7e5e169e-585c-4075-842a-d733e0a62ce2" />

### Appendix 3. Checked for missing values
<img width="601" height="713" alt="Screenshot 2026-07-07 at 1 48 26 PM" src="https://github.com/user-attachments/assets/3375118b-2fee-4644-ab69-d83c72b8a230" />


<img width="643" height="721" alt="Screenshot 2026-07-07 at 1 49 37 PM" src="https://github.com/user-attachments/assets/186c8d25-d13c-4556-bfca-f0d7aea4a986" />


### Appendix 4. Converted all EUR transactions to USD
<img width="378" height="716" alt="Screenshot 2026-07-07 at 3 39 32 PM" src="https://github.com/user-attachments/assets/383f4113-6d13-4e3c-bc03-303c45f32761" />

</div>
