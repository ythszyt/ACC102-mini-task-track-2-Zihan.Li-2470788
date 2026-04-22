# ACC102-mini-task-track-2-Zihan.Li-2470788
# A Python Workflow for Financial Ratio-Based Company performance Comparison

## 1. Problem & Target User

This project develops a reusable Python-based workflow to analyse and compare the recent (from 2018 onwards) financial performance of different companies using financial ratios.

It addresses the analytical problem of how financial ratios can be used to compare the performance of two companies in a simple and structured way.

It is mainly designed for beginner users, such as business or accounting students, who want a simple and structured way to analyse company performance.

## 2. Data Source

Data is obtained from the WRDS Compustat database (`comp.funda`), which provides financial statement information for mainly US-listed companies.

Access date: 20/4/2026

## 3. Methods

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

The selected financial ratios are aligned with the logic of DuPont analysis, which decomposes ROE into profitability, efficiency, and leverage components. However, this project focuses on simplified comparison rather than a full DuPont decomposition.

## 4. Key Findings (Example)

Using PepsiCo (PEP) and Coca-Cola (KO) as an example:

- PepsiCo generally shows higher ROE in recent years, indicating stronger overall returns to shareholders.
- This stronger ROE does not appear to be driven by profit margin alone, because PepsiCo’s profit margin is relatively lower in some years. This suggests that PepsiCo is not necessarily generating more profit from each unit of revenue.
- Instead, PepsiCo’s higher asset turnover indicates that it uses its assets more efficiently to generate sales. This stronger operating efficiency is an important factor supporting its ROE.
- In addition, PepsiCo’s higher leverage suggests greater reliance on debt or external financing, which can further increase returns to equity holders, although it may also imply higher financial risk.
- Overall, the comparison shows that PepsiCo’s stronger ROE is better explained by the combined effect of higher asset turnover and higher leverage rather than higher profit margin, which is consistent with the logic of DuPont analysis.

## 5. Installation

Before running the project, install the required libraries:
pip install wrds pandas matplotlib

## 6. How to Run

1. Open the notebook file
2. Run all cells
3. Enter two company tickers (e.g., `PEP` and `KO`)
4. View generated charts and automated conclusions

## 7. Demo Video

[https://video.xjtlu.edu.cn/Mediasite/Channel/50381bcaa0e74d9582215a01776a3d8d5f/headless/watch/3ca24966381347fdbcf3aed9b0f0a1391d]

## 8. Limitations
- Missing data may lead to incomplete analysis
- Using average values may hide short-term fluctuations
- Results depend on correct ticker input
- Cross-industry comparisons may be less meaningful

## 9. Note

**Users should enter valid company tickers available in the Compustat database.**  
Invalid or inconsistent inputs may result in missing or incomplete data.

## 10. Future Improvements

- Add more financial ratios
- Improve visualisation (e.g., interactive charts)
- Expand to support more than two companies
