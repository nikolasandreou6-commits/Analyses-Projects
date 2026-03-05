# 📊 PSP Performance Architecture — FY2024

**Payment Service Provider Transaction Analysis**  
*Excel · Power Query · Dynamic Dashboard · Multi-Currency*

---

## 📌 Project Overview

This is a self-initiated end-to-end data analysis project built to demonstrate analytical skills in the fintech/payments space. Having no prior experience in the payments industry, I came across the PSP domain and decided to dive straight in — researching how payment service providers work and building a full analysis from scratch.

The project simulates a real-world PSP performance review across 5 providers, 10 European markets, and 5 payment methods for FY2024 — covering everything from data architecture and currency normalization to KPI dashboards and provider routing recommendations.

---

## 🗂️ Dataset

| Property | Detail |
|----------|--------|
| Transactions | 1,000 synthetic records |
| Period | January – December 2024 |
| PSP Providers | Stripe, Adyen, Checkout.com, Worldpay, PaySafe |
| Markets | FR, GB, DE, NL, IT, ES, PL, NO, SE, CY |
| Payment Methods | Credit Card, Debit Card, E-Wallet, Bank Transfer, Crypto |
| Currencies | EUR, GBP, SEK, NOK, PLN |
| FX Rates | ECB 2024 annual averages |

> Data is fully synthetic and generated for portfolio purposes only.

---

## 🛠️ Tools & Techniques

**Power Query (M language)**
- Merged two source tables (Jan–Jun, Jul–Dec) into a single combined dataset
- Live FX rate lookup from a dedicated FX Rates reference table
- Multi-currency normalization to EUR using ECB 2024 average rates
- Automated column type transformations and blank row removal

**Advanced Excel**
- `COUNTIFS`, `SUMIFS`, `AVERAGEIFS` — for segmented KPI calculations
- `XLOOKUP`, `INDEX/MATCH` — for provider and GEO lookups
- `UNIQUE`, `FILTER`, `SORT` — for dynamic data extraction
- Pivot Tables — for revenue trends, status breakdown, geographic and payment method analysis
- Conditional formatting, custom number formatting, structured table references

**Dashboard Design**
- Static KPI dashboard with provider performance table and monthly trends
- Dynamic dashboard with slicers (PSP Provider, Payment Method) and timeline filter
- Dark navy theme with consistent colour coding and icon headers

---

## 📋 Analysis Tasks

| # | Task | Description |
|---|------|-------------|
| 1 | Conversion Rate by PSP | Success rate per provider across all transactions |
| 2 | Revenue & Fee Analysis | Net revenue, fees paid, and fee rate benchmarking per provider |
| 3 | Geographic Performance | Success rate, avg ticket size, and net revenue per market |
| 4 | Decline Reason Analysis | Breakdown of failure causes as % of total failed transactions |
| 5 | Best PSP per Market | Highest-converting provider for the top 3 GEOs by volume |
| 6 | Pending Transaction Analysis | Pending rate by provider, GEO, and payment method |

---

## 📈 Key Findings

- **Overall success rate: 55.4%** — significant room for improvement vs industry benchmarks of 70–85%
- **Checkout.com** leads conversion at **58.8%** with the lowest fee rate (1.9%), generating **€249K** net revenue
- **France** tops geographic performance at **63.4%** conversion; Sweden and Germany lag at ~49%
- **22.8% of transactions remain Pending** — a significant operational concern, with Worldpay (24.7%) and Stripe (24.2%) having the highest pending rates
- **Fraud Suspected (23.4%)** and **Card Declined (22.5%)** account for nearly half of all declines
- A **multi-PSP routing strategy** could materially lift overall conversion — optimal providers vary significantly by market (Adyen in NL, Checkout.com in GB, PaySafe in CY)

---

## 🗃️ File Structure

```
PSP-Analysis/
│
├── PSP_Performance_Architecture_2024_V2.xlsx   # Main workbook
│
│   Sheets:
│   ├── Documentation        # Project overview, methodology, assumptions & key findings
│   ├── Raw Data (Jan-Jun)   # Source transactions Jan–Jun 2024 (485 rows)
│   ├── Raw Data (Jul-Dec)   # Source transactions Jul–Dec 2024 (515 rows)
│   ├── FX Rates             # ECB 2024 average exchange rates (EUR reference)
│   ├── Raw_Data_Combined    # Power Query output — merged & normalized (1,000 rows)
│   ├── Tasks                # All 6 analytical tasks with formulas
│   ├── Dashboards           # Static KPI dashboard
│   ├── Pivot Tables         # Supporting pivot table outputs
│   └── Dynamic Dashboard    # Interactive dashboard with slicers & timeline
```

---

## ⚙️ How to Open

1. Download the `.xlsx` file
2. Open in **Microsoft Excel 2019 or Microsoft 365** *(required — XLOOKUP and Power Query not supported in older versions)*
3. Click **"Enable Content"** when prompted — this allows Power Query to run
4. To refresh data after changing FX rates: **Data → Refresh All**

> ⚠️ Not compatible with Google Sheets or LibreOffice

---

## 👤 Author

**Nikolas Andreou**  
*Data & Business Intelligence Analyst*  
[LinkedIn](https://www.linkedin.com/in/) · [GitHub](https://github.com/nikolasandreou6-commits)

---

*Prepared for portfolio and recruitment purposes · Data is entirely synthetic*
