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

avg_moic_by_sector.png
This Chart compares the Average MOIC(Multiple on Invested Capital) across sectors for the selected portfolio.

distance_from_52w_high.png
This Chart shows the % below which the screened portfolio companies are performing.

ebitda_margin_vs_moic.png
The scatter plot examines the relationship between EBITDA margin and Multiple on Invested Capital(MOIC) across selected portfolio companies.It helps assess whether companies with stronger operating profitability also demonstrate higher investment multiples

moic_by_company.png

simple_vs_weighted_moic.png


# Key Findings:
Fund-level return: The 14 holdings produced a simple average MOIC of 1.24X and a market-cap-weighted average MOIC of 1.25X.The almost similar returns show the top company's performance made little difference to the overall result.
Top and Bottom Performers: Paycom led at about 2.1X, followed by Market Axess(1.5X), FactSet(1.44X), and Match Group(1.40X). Wynn, Pentair, Clorox, and Campbell were close to 1.0X. Paycom's result strongly influenced the fund's average.
Sector View: Human Resource & Employment Services (2.1X), Financial Exchanges & Data(1.47X), and Interactive Media & Services(1.40X) averaged highest.  Most sectors contain only one or two holdings, so these averages mostly reflect individual companies.
Distance from 52-week high: Paycom and Match Group trade within about 10% of their highs, while Pentair and Wynn are closer to about 50% below. This matches the MOIC ranking, since stocks near the lows have the lowest MOIC.
