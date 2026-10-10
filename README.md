# PE_portfolio_monitoring
Rule-based portfolio creation and monitoring of 14 mid-cap companies from open S&P 500 data, PE-style screening, and MOIC analysis in Python.

Private Equity Portfolio Monitoring: Hypothetical Mid-Market Fund

I built a rule-based portfolio of 14 mid-cap companies from the open S&P 500 financials dataset (snapshot of 3 October 2026), using screening criteria inspired by how PE firms select buyout targets:

Market cap of $2B–$10B (mid-cap)
EBITDA margin of 15% or higher
Pays a dividend (dividend yield above 0), as a sign of stable cash flow
P/E ratio above 0 and at most 30, to avoid overpaying for growth

I then monitored the portfolio as a PE fund would: MOIC per holding, simple vs weighted fund-level MOIC, sector averages, EBITDA margin vs MOIC, and distance from the 52-week high. Results are visualised in Python.

Data Link: https://raw.githubusercontent.com/datasets/s-and-p-500-companies-financials/af7220f04c70c401dff2b8efeb3c7261cae5dcc0/data/constituents-financials.csv.
