# Corporate-Credit-Risk-IFRS-9-Basel-III-Integration
This project computes the calculation of Expected Credit Loss (ECL) for a portfolio of UK corporate loans. It demonstrates how to integrate Credit Ratings, Industry Sectors, and Macro-Economic Factors into a regulatory reporting framework compliant with IFRS 9 and Basel III.

I conducted a stress testing for UK Loan Portfolios in order to bridge the gap between accounting (IFRS 9) and regulatory capital (Basel III). This project automates the calculation of Expected Credit Loss (ECL) and Risk-Weighted Assets (RWA) for a 20-loan UK corporate portfolio under a 2025 high-interest-rate scenario.

📊 Business Logic & Metrics
IFRS 9 ECL: Implemented forward-looking "Stress factors" (1.5x factor for Retail) to calculate capital provisions (stage 2/3).

Basel III RWA: Applied the Standardised Approach (SA) risk weights (20% to 150%) to determine CET1 capital requirements (11% benchmark).

Weighted Average Probability of Default (WAPD): Used SQL Window Functions to calculate risk density across sectors, identifying Retail as the most capital-intensive industry (150% average risk weight).

🛠️ Tech Stack
•	Database: Google BigQuery (SQL)
•	Skills: Data modelling, CTEs, multi table join, Subqueries, Case Logic, Sector-based Risk Aggregation.
•	Domain: Credit Risk Analytics, IFRS 9, Basel III.

SQL Logic: Window functions (OVER()), conditional logic (CASE WHEN), and performance metrics.

💡 Key Finding
While Real Estate represents the highest total exposure (£75M+), Retail industry requires the most aggressive capital retention relative to its size due to a 150% risk-weight density under 2025 UK economic forecasts.
