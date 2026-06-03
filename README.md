# Bank Loan Portfolio Analytics Dashboard

[View Power BI Dashboard](https://app.powerbi.com/links/SD74Sak5j-?ctid=a8eec281-aaa3-4dae-ac9b-9a398b9215e7&pbi_source=linkShare)

## Overview

This project analyzes bank loan application and repayment data using SQL and Power BI. The dashboard tracks loan applications, funded amount, amount received, interest rates, debt-to-income ratio, loan status, borrower segments, and portfolio performance.

This is a business intelligence and financial analytics project, not a machine learning project.

## Business Problem

Financial institutions need reliable reporting to monitor loan portfolio health, repayment performance, bad loans, borrower segments, and lending trends. Without a structured dashboard, analysts must manually query loan records and rebuild recurring reports, slowing down portfolio review and decision-making.

This project turns loan-level data into executive-ready dashboards for tracking loan performance, portfolio risk, and borrower behavior.

## Dataset

* **Dataset:** Financial loan dataset
* **Core Table:** `bank_loan_data`
* **Domain:** Bank loan applications and repayment performance
* **Key Fields:** Loan ID, issue date, loan amount, funded amount, amount received, interest rate, debt-to-income ratio, loan status, state, term, purpose, grade, subgrade, home ownership, employee length

## Key KPIs

The dashboard tracks the following loan portfolio metrics:

* Total loan applications
* Month-to-date loan applications
* Month-over-month loan application change
* Total funded amount
* Month-to-date funded amount
* Month-over-month funded amount change
* Total amount received
* Month-to-date amount received
* Month-over-month amount received change
* Average interest rate
* Average debt-to-income ratio
* Good loan percentage
* Bad loan percentage
* Good loan funded amount and received amount
* Bad loan funded amount and received amount

## Dashboard Pages

### 1. Summary Dashboard

![Summary Dashboard](Dashboard/SUMMARY.png)

The Summary Dashboard provides a high-level view of portfolio performance.

It includes:

* Total loan applications, funded amount, and amount received
* Month-to-date and month-over-month KPI tracking
* Average interest rate and average DTI ratio
* Good loan vs. bad loan segmentation
* Loan status breakdown for fully paid, charged-off, and current loans

### 2. Overview Dashboard

![Overview Dashboard](Dashboard/OVERVIEW.png)

The Overview Dashboard breaks down loan applications across borrower and loan dimensions.

It includes:

* Loan applications by month
* Loan applications by state
* Loan applications by loan term
* Loan applications by employee length
* Loan applications by loan purpose
* Loan applications by home ownership

### 3. Details Dashboard

![Details Dashboard](Dashboard/DETAILS.png)

The Details Dashboard provides a granular loan-level view for deeper portfolio review.

It includes:

* Loan ID
* Loan purpose
* Home ownership
* Grade and subgrade
* Funded amount
* Interest rate
* Installment
* Amount received

## Filter Options

The dashboard allows users to drill down by:

* State
* Grade
* Loan purpose
* Good vs. bad loan status

## SQL Analysis

SQL was used to query, aggregate, and validate the dashboard KPIs.

Examples of SQL analysis include:

* Total loan applications
* Month-to-date loan applications
* Total funded amount
* Month-to-date funded amount
* Total amount received
* Month-to-date amount received
* Average interest rate
* Average debt-to-income ratio
* Good loan and bad loan segmentation
* Loan status breakdown
* Borrower and loan-purpose segmentation

## Tools Used

SQL, Power BI, Data Cleaning, KPI Reporting, Dashboard Design, Financial Analytics, Business Intelligence

## Repository Structure

```text
Bank_Loan_Report/
├── Dashboard/
├── Bank_Loan_Dashboard.pbix
├── Query Doc.pdf
├── financial_loan.csv
└── README.md
```

## How to Use

1. Open the live Power BI dashboard link to view the published report.
2. Open `Bank_Loan_Dashboard.pbix` in Power BI Desktop for the full dashboard file.
3. Review `financial_loan.csv` to inspect the source loan dataset.
4. Use `Query Doc.pdf` to review the SQL logic used for KPI calculations.
5. Navigate through the Summary, Overview, and Details dashboard pages.
6. Use filters to analyze loan performance by state, grade, purpose, and loan quality.

## Business Impact

This dashboard helps analysts and financial managers monitor loan portfolio performance in one place. It reduces manual reporting effort by centralizing application volume, funded amount, repayment metrics, interest rates, DTI, good/bad loan segmentation, and borrower-level breakdowns into an interactive Power BI report.

## Limitations

* This project is descriptive analytics only and does not predict loan default risk.
* Good and bad loan classifications are based on loan status logic, not a trained risk model.
* The dashboard depends on the available historical loan data.
* Automated refresh is not configured in the repository.
* Profitability, loss severity, and expected credit loss are not modeled.

## Future Improvements

* Add SQL scripts as `.sql` files instead of PDF-only documentation
* Add automated Power BI refresh documentation
* Add loan vintage analysis
* Add delinquency and charge-off trend analysis
* Add borrower risk segmentation by grade, purpose, and DTI bands
* Add profitability metrics such as net return or loss-adjusted return
* Add a separate default prediction model as an ML extension


**Interactive Data Drill-Downs:** Enabling users to click through visual elements for more detailed views.

**Additional KPIs:** Incorporating more financial health indicators, such as profit margins and return on investment for loans.

## Acknowledgments

This project was developed to assist financial analysts and managers in tracking loan performance and identifying trends in loan applications. Special thanks to the data and finance teams for providing valuable feedback during the development process.
