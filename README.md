Multi-Cap Portfolio Optimization Using Riskfolio-Lib
This repository contains the code and analysis for a project that applies portfolio optimization techniques to different pools of assets filtered by market capitalization. The project focuses on small-cap, mid-cap, and large-cap stocks, applying various financial filters to select the best assets from each category before optimizing the portfolio using the Sharpe ratio as the objective.

Project Overview
The primary goal of this project is to create and optimize portfolios composed of small, mid, and large-cap stocks, filtered by financial metrics such as Free Cash Flow Yield, EPS Growth, and Revenue Growth. The project uses Python's Riskfolio-Lib to perform portfolio optimization based on historical returns and covariance matrices. The analysis is divided into three main sections based on market capitalization groups, followed by an overall portfolio optimization.

Key Steps:
Filtering Assets: Stocks are filtered based on a series of financial metrics (e.g., CAGR, FCF Yield, EPS Growth) to select high-performing assets from small-cap, mid-cap, and large-cap categories.

Data Collection: Stock price data is collected using yfinance for the selected stocks over a specified period.

Portfolio Optimization: Each market capitalization group (small-cap, mid-cap, large-cap) undergoes a Sharpe ratio-based optimization using historical returns and covariance. The results are plotted on an efficient frontier graph.

Visualization: The project includes several visualizations to highlight the portfolio weights by sector, market capitalization group, and geographic distribution.

Libraries Used
yfinance: For pulling historical stock data.
Riskfolio-Lib: Used for portfolio optimization, including calculating asset statistics and generating efficient frontiers.
Quantstats: For financial performance reporting.
matplotlib & seaborn: For data visualization.
empyrial: For engine-based portfolio analysis.
How to Run the Project
Prerequisites
Ensure you have the required Python libraries installed:

bash
Copy code
pip install empyrial
pip install quantstats
pip install Riskfolio-Lib
Running the Analysis
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/multi-cap-portfolio-optimization.git
cd multi-cap-portfolio-optimization
Run the Jupyter Notebook:
The analysis is conducted in a Python notebook, which you can run after setting up the dependencies.

Explore Results:
The notebook generates several reports and visualizations, including:

Efficient frontiers for each market capitalization group.
Portfolio weight distributions by sector and market capitalization group.
Scatter and pie charts highlighting geographic distribution of assets.
Financial Filters Used
Small-Cap Stocks
10-Year CAGR > 7%
FCF Yield > 0.5%
Revenue Growth 5Y > 5%
EPS Growth 5Y > 1%
P/E Ratio > 4
Positive Net Income and EPS
Mid-Cap Stocks
10-Year CAGR > 7%
FCF Yield > 1%
FCF Growth 5Y > 5%
Positive Net Income and EPS
EPS Growth 5Y > 1%
Large-Cap Stocks
10-Year CAGR > 10%
FCF Yield > 2%
FCF Growth 5Y > 7%
ROIC (5Y) > 12%
EPS Growth 5Y > 3%
Results and Visualizations
Portfolio Weights by Market Cap
A pie chart shows the percentage of the portfolio allocated to small-cap, mid-cap, and large-cap stocks.

Sector Weights
Another pie chart illustrates the sector allocations of the portfolio, providing insights into sector diversification.

CAGR by Market Cap Group
A bar chart shows the average compound annual growth rate (CAGR) for different market cap groups (small, mid, large) over 3, 5, 10, and 15 years.

Geographic Distribution
A scatter plot shows the portfolio weight distribution by state, helping visualize geographic exposure.

Future Enhancements
Rebalancing Simulation: Future versions may include rebalancing the portfolios periodically to observe the impact on returns.
Risk Measures: Include more advanced risk measures like Conditional Value at Risk (CVaR).
Sector-Specific Analysis: Further refinement of sectors for more detailed sector analysis.
License
This project is licensed under the MIT License - see the LICENSE file for details.
