# Banking_Risk_Analysis

📌 Project Overview
This project focuses on Risk Analytics within the banking sector. The primary objective is to minimize financial loss by analyzing client profiles and their likelihood to repay loans. Using a combination of Python for data processing and Power BI for advanced visualization, this project provides actionable insights into loan distribution, deposit trends, and client engagement.

📊 Dataset Description

The analysis is based on a relational dataset containing banking and client-specific information across five interlinked tables:

Clients-Banking: Core transactional and loan data.

Banking Relationship: Details on bank types and client-bank links.

Gender: Demographic segmentation.

Investment Advisor: Details of advisors managing client portfolios.

Period: Time-based data for longitudinal analysis.

🛠️ Tools & Technologies

Language: Python (Pandas, NumPy for Data Cleaning/EDA)

Visualization: Power BI (DAX, Power Query)

Reporting: Microsoft PowerPoint & Power BI Service

Environment: Jupyter Notebook / VS Code

🚀 Project Steps

1. Data Loading & EDA (Python)
Imported raw datasets and performed an initial check for missing values and outliers.
Conducted Exploratory Data Analysis (EDA) to understand the distribution of income, loan amounts, and credit card balances.

2. Data Cleaning & Transformation

Feature Engineering: Created Engagement Timeframe and Engagement Days using DATEDIFF logic.

Income Segmentation: Created an Income Band column to categorize clients into Low (<100k) and Mid (<300k) brackets.

Fee Logic: Derived Processing Fees based on the fee structure (High = 0.05).

3. DAX Implementation (KPIs)

Developed custom measures using Data Analysis Expressions (DAX):

Total Loan: [Bank Loan] + [Business Lending] + [Credit Cards Balance]

Total Deposit: Aggregate of Savings, Checking, and Foreign Currency accounts.

Total Fees: SUMX calculation multiplying Total Loan by Processing Fees.

4. Power BI Dashboard Development

Built a multi-page interactive dashboard:

Home: Overview of the banking ecosystem.

Loan Analysis: Deep dive into lending risks and nationality-based loan distribution.

Deposit Analysis: Breakdown of liquidity across different account types.

Summary: Executive snapshot of key banking metrics.

📈 Key Results & Insights

Risk Mitigation: Identifying high-risk applicants based on income bands and existing debt-to-deposit ratios.
Competitive Analysis: Discovered that Private Banks hold a higher client share, suggesting a need for strategy shifts in other banking sectors.
Geographic Trends: Identified specific nationalities with the highest loan volumes to assist in regional risk assessment.

📁 Repository Structure

text
├── Data/               # Raw and cleaned CSV/Excel files
├── Scripts/            # Python notebooks for EDA and Cleaning
├── Dashboard/          # Power BI (.pbix) file
├── Presentation/       # Final Project PPT and PDF Report
└── README.md           # Project Documentation

Use code with caution.


💻 How to Run

Python: Open the Jupyter Notebook in the Scripts/ folder and run all cells to see the data transformation process.
Power BI: Install Power BI Desktop. Open the .pbix file in the Dashboard/ folder to interact with the visualizations.
PPT: Refer to the Presentation/ folder for a high-level summary of findings for stakeholders.

