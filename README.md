# Bank Deposit BI Dashboard

## Concentration, Structure and Dynamics Analysis

---

## Project Overview

This project presents a Power BI dashboard developed to analyze the financial results of a bank department responsible for attracting deposits from corporate clients.

The dashboard allows monitoring of deposit inflows, outflows, interest accrual, debt position and average deposit size across different client segments, industries, cities and currencies.

---

## Business Context

The bank operates with three corporate client segments:

- Multinational Companies (MNC)
- Large Business (LB)
- Government Companies (GC)

The department requires a reporting tool to:

- Monitor attracted and paid funds
- Calculate daily accrued interest
- Control deposit portfolio concentration
- Analyze structure by segment, city and industry
- Work with multi-currency deposits

---

## Objectives

- Calculate key financial metrics:
  - Attracted Funds
  - Paid Funds
  - Accrued Interest
  - Debt Position
  - Average Deposit Size

- Implement daily interest accrual logic
- Build multi-currency model (RUB, USD, EUR)
- Implement dynamic currency conversion
- Enable filtering by:
  - Period (day-level granularity)
  - Segment
  - Industry
  - City
  - Reporting currency

---

## Analytical Logic

### Interest Accrual

Interest is calculated daily based on end-of-day balance.

Formula:

Daily Interest = Balance × Rate / 360

Negative balances (overdraft) do not accrue interest.

---

### Currency Conversion

- Historical exchange rates are loaded from Central Bank data
- Conversion is performed using the latest available rate at the end of the selected period
- Users can switch between:
  - Original currencies
  - Selected reporting currency

---

## Dashboard Structure

The report consists of four pages:

1. Summary – Original Currencies
2. Summary – Converted Currency
3. Industry & City Breakdown – Original Currency
4. Industry & City Breakdown – Converted Currency

---

## Data Model

The data model includes:

- Transaction table (cash inflows and outflows)
- Client registry with segment, industry and city
- Currency exchange rate table
- Calendar table for daily calculations

The model enables:

- Daily balance calculation
- Interest accrual logic
- Multi-currency aggregation
- Dynamic currency conversion

---

## Key Insights

- Moscow holds the largest share of total deposits (17.6%)
- Novosibirsk has the highest average deposit size
- Top 3 industries account for 48% of total volume
- Currency conversion significantly affects ranking positions

- Top-10 clients represent a highly concentrated share of the total deposit portfolio, indicating dependency on large clients
- Portfolio concentration ratio increased toward the end of the observed period, signaling growing concentration risk
- Interest income shows a steady upward trend, contributing positively to overall portfolio profitability
- Average deposit size remained relatively stable with moderate fluctuations, indicating consistent client behavior
- Inflows and outflows demonstrate cyclical patterns, suggesting seasonality in deposit activity
- Currency conversion enables accurate cross-currency comparison and reveals the true structure of the consolidated portfolio

---


## Tech Stack

- Power BI
- Power Query
- DAX
- Data Modeling

---


## Portfolio Concentration Analysis

The dashboard allows analysis of deposit concentration by:

- Client segment
- Industry
- City

Users can identify segments or industries that form the largest share of the portfolio and monitor structural changes over time.

---


## Skills Demonstrated

- Financial metric calculation
- Daily interest accrual modeling
- Multi-currency reporting
- Dynamic currency conversion
- Data transformation
- Interactive dashboard design

---

## Dashboard Preview

(Screenshots are available in the /screenshots folder)

---

## File

The Power BI file (.pbix) is included in the repository.

---

