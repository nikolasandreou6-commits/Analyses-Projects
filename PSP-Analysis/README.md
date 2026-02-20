PSP Analyst Portfolio Project
Overview
This project simulates a real-world Payment Service Provider (PSP) analyst task. The dataset contains 1,000 transactions across 5 PSP providers, 10 countries, and 5 payment methods covering the full year of 2024.
The goal was to analyse payment traffic, identify performance trends, and provide actionable recommendations — the core responsibilities of a PSP Analyst role.

Skills Demonstrated

Data import and consolidation using Power Query (merging two source files)
Advanced Excel functions: COUNTIFS, SUMIF, AVERAGEIFS, XLOOKUP, INDEX/MATCH, UNIQUE, FILTER, SORT, TAKE
Data analysis and KPI reporting
Dashboard creation with charts
Business insight generation from raw transaction data


Dataset
Two datasets were used, imported and combined using Power Querry.


Analysis & Key Findings
Task 1 — Conversion Rate by PSP Provider
Calculated success rate for each provider. Clear differences in conversion performance were identified across providers, with one provider significantly outperforming the rest and another consistently underperforming.
Recommendation: Prioritise routing traffic through the highest-converting provider to improve overall transaction success rates.

Task 2 — Revenue & Fee Analysis by Provider
Analysed total transaction volume, fees charged, and net revenue per provider. The analysis revealed that the most expensive provider in terms of fees does not deliver proportionally better conversion, making it a less cost-efficient choice.
Recommendation: Review usage of high-fee providers and consider shifting volume to providers with a better fee-to-performance ratio.

Task 3 — Performance by GEO
Evaluated transaction volume, success rate, and average transaction value across 10 countries. Significant variation in conversion rates was found between markets, with some GEOs performing well above average and others showing consistently weak results.
Recommendation: Investigate underperforming markets to determine whether poor results are driven by provider choice, payment method mix, or local market factors.

Task 4 — Decline Reason Analysis
Identified and ranked the root causes of failed transactions. Fraud-related declines were found to be the leading reason, followed by card declines and technical errors — suggesting both fraud rule calibration and provider reliability as areas for improvement.
Recommendation: Review fraud detection thresholds to reduce false positives, and investigate providers with high technical error rates.

Task 5 — Best PSP Provider per GEO
For the top 3 markets by volume, identified the best-performing PSP provider in each. Results showed that no single provider dominates across all markets — performance varies significantly by GEO.
Recommendation: Implement geo-based routing logic to direct traffic to the best-performing provider in each market, rather than using a single global provider.

Task 6 — Dashboard
Interactive dashboard built in Excel.
<img width="2228" height="1147" alt="image" src="https://github.com/user-attachments/assets/23a7e1a3-b8df-4564-8a9b-49eda9aec9de" />



Tools Used

Microsoft Excel (Power Query, Advanced Formulas, Charts)
Data source: Simulated PSP transaction dataset (1,000 records)


Author
Nikolas Andreou
https://www.linkedin.com/in/nikolasandreou/| naandreou2@hotmail.com
