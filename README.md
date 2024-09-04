# Cap-Size-Based-Optimization-

Overview
This project focuses on optimizing a portfolio composed of small, mid, and large-cap stocks using a variety of financial metrics and quantitative strategies. By dividing the market into three distinct capitalization sizes—Nano-Cap, Small-Cap, and Mega-Cap—this project aims to identify the best-performing assets based on their financial performance over a specified period.

Key performance metrics such as CAGR 5Y, FCF Yield, Revenue Growth 5Y, Profit Margin, EPS, and Average Volume are used to filter and optimize portfolios. The objective is to examine the outperformance of small-cap stocks relative to larger market capitalization stocks.

Project Structure
Data Sourcing: Data was sourced from financial databases covering a wide array of small, mid, and large-cap stocks.
Analysis: The analysis was conducted using Python libraries such as pandas, yfinance, and empyrial, leveraging key financial statistics for stock performance analysis.
Optimization: The portfolio was optimized using Modern Portfolio Theory (MPT), Sharpe Ratio optimization, and the Kelly Criterion, with simulations done over 5 and 10-year periods.
Key Features
Financial Data Collection:
Stocks ranging from Nano-Cap to Mega-Cap were filtered based on key financial metrics.
Data included variables such as 5-year revenue growth, profit margins, and FCF yield.
Portfolio Optimization:
Multiple optimization techniques were applied including Modern Portfolio Theory (MPT), Sharpe Ratio, and Kelly Criterion.
The dataset was segmented into different capitalization groups to ensure proper optimization for each market segment.
Simulations and Results:
Each portfolio was backtested and simulated over a 5-year period, with rebalancing scenarios included to test different strategies.
Performance comparisons were made between equally weighted portfolios and those optimized with various quantitative strategies.
Installation
To run this project locally, follow these steps:

Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/small-mid-large-cap-optimization.git
Navigate to the project directory:
bash
Copy code
cd small-mid-large-cap-optimization
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the optimization:
bash
Copy code
python optimize_portfolio.py
Usage
Data Preparation: Ensure you have access to financial data either through a CSV file or a financial API such as yfinance.
Optimization: Customize the optimization script based on the specific cap size you are interested in (small, mid, large).
Visualization: Results of the optimization are presented as sector breakdowns, Sharpe ratios, and other visualizations.
Requirements
Python 3.8+
pandas
yfinance
empyrial
matplotlib
numpy
Project Files
optimize_portfolio.py: The main script that performs portfolio optimization.
data/: A directory that contains stock data for small, mid, and large caps.
visualizations/: Contains graphs and sector breakdowns for the portfolios.
README.md: The documentation file (you're reading it).
Results and Analysis
The results are stored in results/ and include:

Portfolio performance metrics.
Sector weights for optimized portfolios.
Sharpe, Sortino, and Omega ratios visualized for each portfolio.
Future Work
Expand the project to include more detailed risk metrics like Treynor Ratio.
Investigate performance under different market conditions (bull vs bear markets).
Automate the data refresh process for daily or weekly updates.
Contributing
If you would like to contribute to this project, feel free to submit a pull request. Any improvements, suggestions, or bug fixes are welcome!

License
This project is licensed under the MIT License.
