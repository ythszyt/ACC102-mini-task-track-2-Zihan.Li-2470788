# ACC102-mini-task-track-2-Zihan.Li-2470788
# A Python Workflow for Financial Ratio-Based Company performance Comparison

## Project Overview
This project develops a **reusable Python-based workflow** to analyse and compare the recent financial performance of different companies using financial ratios.

The workflow allows users to input any two company tickers (from the WRDS Compustat database) and automatically generate simple ratio analysis and visual comparisons.

---

## Analytical Problem
How can financial ratios be used to analyse and compare the recent performance of different companies in a simple and structured way?

---

## Target User
This tool is designed for beginner users (e.g., business or accounting students) who want a simple and structured way to analyse recent company performance using Python.

---

## Data Source
Data is obtained from the WRDS Compustat database (`comp.funda`), which provides financial statement information for mainly US-listed companies.

Access date: 20/4/2026

---

## Methods
The workflow includes the following steps:

- Data retrieval from WRDS
- Data cleaning (removing duplicates and missing values)
- Variable renaming for readability
- Financial ratio calculation:
  - ROE (Return on Equity)
  - Profit Margin
  - Asset Turnover
  - Leverage
- Visualisation using line charts
- Automated rule-based comparison

- (The selected financial ratios are aligned with the logic of DuPont analysis, which decomposes ROE into profitability, efficiency, and leverage components.However, this project focuses on simplified comparison rather than a full DuPont decomposition.)

---

## Key Findings (Example)
Using PepsiCo (PEP) and Coca-Cola (KO) as an example:

- One company may show higher profitability (ROE)
- The other may demonstrate more stable financial structure (leverage)
- Differences reflect business model and financial strategy

---

## How to Run
1. Open the notebook file
2. Run all cells
3. Enter two company tickers (e.g., `PEP` and `KO`)
4. View generated charts and automated conclusions

---

## Demo Video
[把你的视频链接粘在这里]

---

## Limitations
- Missing data may lead to incomplete analysis
- Using average values may hide short-term fluctuations
- Results depend on correct ticker input
- Cross-industry comparisons may be less meaningful

---

## Note
**Users should enter valid company tickers available in the Compustat database.**  
Invalid or inconsistent inputs may result in missing or incomplete data.

---

## Future Improvements
- Add more financial ratios
- Improve visualisation (e.g., interactive charts)
- Expand to support more than two companies
