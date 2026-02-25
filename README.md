# Bank Deposit Portfolio BI Dashboard

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

## Tech Stack

- Power BI
- Power Query
- DAX
- Data Modeling

---

## Skills Demonstrated

- Financial metric calculation
- Daily interest accrual modeling
- Multi-currency reporting
- Dynamic currency conversion
- Data transformation
- Interactive dashboard design
