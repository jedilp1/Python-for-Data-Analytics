# ESG vs. Non-ESG Stock Performance Analysis

This project is a data-driven investigation into the financial performance of companies with an ESG (Environmental, Social, and Governance) designation compared to their non-ESG peers. The analysis focuses specifically on the **Petrochemical & Chemical sector in Thailand**.

This was developed as a project for a Python course, demonstrating a complete, end-to-end data analysis workflow: from data acquisition and cleaning to statistical analysis and interactive visualization.

## Analysis & Key Features

The notebook executes several key analytical steps to compare the two groups of stocks:

* **Data Acquisition:** Fetches historical stock price data from the Yahoo Finance (`yfinance`) API.
* **Data Processing:** Cleans and structures the data using `pandas`, preparing it for analysis.
* **Financial Metrics Calculation:** Computes a comprehensive set of performance and risk metrics for each stock, including:
    * Annualized Returns
    * Annualized Volatility (Risk)
    * Beta (vs. SET Index)
    * Sharpe Ratio (Risk-Adjusted Return)
    * Cumulative Growth ("Growth of 1 Baht")
* **Fundamental Analysis:** Compares key fundamental ratios between the groups:
    * Price-to-Earnings (P/E) Ratio
    * Return on Equity (ROE)
    * Debt-to-Equity (D/E) Ratio
* **Statistical Testing:** Employs the **Mann-Whitney U test** (a non-parametric test) to determine if observed differences in metrics (like Sharpe Ratio and ROE) are statistically significant.
* **Interactive Visualization:** Uses `Plotly` to generate an interactive line chart showing the cumulative growth of every stock, allowing for dynamic exploration of the data.

## Tools & Libraries Used

* **Python 3.x**
* **Jupyter Notebook:** For interactive development and analysis.
* **Pandas:** For data manipulation and analysis.
* **yfinance:** For downloading historical stock market data.
* **SciPy:** For statistical analysis (specifically, `scipy.stats.mannwhitneyu`).
* **Plotly:** For creating interactive, web-ready visualizations.
* **Matplotlib:** For static plots (bar charts, box plots).

## Key Findings

Based on the analysis within the notebook, the key finding for this specific dataset was:

**There is no statistically significant difference** in the risk-adjusted returns (Sharpe Ratio) or profitability (Return on Equity) between the ESG-designated group and the non-ESG group in the Thai Petrochemical & Chemical sector.

While individual stocks showed wide variations in performance, an ESG designation was not found to be a reliable indicator of superior (or inferior) financial performance for this particular sample.

## Limitations & Disclaimer

This is the most important section for understanding the scope of this project.

* **Small Sample Size:** The primary limitation of this analysis is the very small sample size. The conclusions are drawn from a handful of companies within a single, niche sector. This means the results are highly sensitive to outliers and **cannot be generalized** to the broader market in Thailand or other sectors.
* **Academic Purpose:** This project was created as an academic exercise to demonstrate a data analysis workflow.
* **Not Financial Advice:** The findings and analysis presented here are for informational and educational purposes only. They do **not** constitute financial advice, and should not be used as the basis for any investment decisions.
