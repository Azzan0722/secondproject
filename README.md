📈 Data-Driven Stock Analysis: Organizing, Cleaning, and Visualizing Market Trends
Overview
This project provides a comprehensive Stock Performance Dashboard to analyze and visualize the Nifty 50 stocks' performance over the past year. It extracts, cleans, and processes stock data, computes key performance metrics, and presents insights via interactive dashboards using Streamlit and Power BI.

The solution empowers investors, analysts, and traders to make informed decisions based on historical stock performance and market trends.

Skills Learned
Python & Pandas for data cleaning and transformation

SQL for data storage and queries

Streamlit for building interactive dashboards

Power BI for business intelligence visualizations

Data Analysis (Volatility, Correlation, Sector Performance)

Statistical Insights for investment decision-making

Domain
Finance / Data Analytics

Problem Statement
The goal is to analyze daily stock data (Open, Close, High, Low, Volume) of Nifty 50 stocks and:
✅ Rank top 10 best and worst-performing stocks
✅ Provide a market summary and sector-wise insights
✅ Visualize volatility, cumulative returns, and correlation
✅ Build interactive dashboards for decision support

Business Use Cases
Stock Performance Ranking – Identify top/bottom 10 stocks

Market Overview – Average stock performance & green vs. red ratio

Investment Insights – Detect consistent growth vs. significant decline

Decision Support – Guide institutional and retail traders

Approach
1. Data Extraction & Transformation
Data provided in YAML format, organized by months and dates

Extract and transform data into CSV files, one for each stock

Merge CSV files into a consolidated Pandas DataFrame

Save processed data in SQL Database

2. Data Analysis & Metrics
Top 10 Gainers & Losers based on yearly return

Market Summary (green vs. red stocks, average price & volume)

Volatility Analysis – Standard deviation of daily returns

Cumulative Returns – Trend over the year for top 5 stocks

Sector-wise Performance – Average returns by sector

Correlation Matrix – Stock price relationship

Visualization Requirements
✅ Volatility Analysis
Calculate daily returns:

python
Copy
Edit
daily_return = (close_price - prev_close_price) / prev_close_price
Compute standard deviation for each stock

Bar Chart: Top 10 most volatile stocks

✅ Cumulative Return Over Time
Calculate cumulative returns using:

python
Copy
Edit
cumulative_return = (1 + daily_return).cumprod()
Line Chart: Top 5 performing stocks

✅ Sector-wise Performance
Map stocks to sectors

Compute average yearly return per sector

Bar Chart: Sector vs. Avg Return

✅ Stock Price Correlation
Compute correlation matrix:

python
Copy
Edit
df.corr()
Heatmap: Correlation of closing prices

✅ Top 5 Gainers & Losers (Month-wise)
Group by month, calculate monthly returns

Identify top 5 gainers & losers for each month

Bar Charts: 12 charts for each month

Dataset
Historical Nifty 50 stock data for 1 year (YAML format → CSV → SQL DB)

Deliverables
✅ SQL Database – Clean, processed stock data

✅ Python Scripts – For ETL (Extract, Transform, Load) & Analysis

✅ Streamlit App – Interactive dashboard with filters & visualizations

✅ Power BI Dashboard – Market trends and performance summary

Tools & Technologies
Languages: Python

Database: MySQL / PostgreSQL

Visualization: Streamlit, Power BI

Libraries: Pandas, Matplotlib, Seaborn, SQLAlchemy

