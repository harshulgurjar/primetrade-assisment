# primetrade-assisment

🧭 Project Overview

This project explores the relationship between trader performance and Bitcoin market sentiment (Fear vs. Greed).
The goal is to uncover behavioral and performance patterns that can help design smarter trading strategies aligned with market psychology.

You will analyze and merge two datasets:

Fear & Greed Index — Daily Bitcoin sentiment (Fear or Greed)

Historical Trader Data (Hyperliquid) — Records of individual trades with profit/loss and trade details

📂 Datasets
Dataset	Description	Key Columns
fear_greed_index.csv	Daily Bitcoin market sentiment	Date, Classification
historical_data.csv	Hyperliquid trader performance data	account, symbol, execution_price, size, side, time, start_position, event, closedPnL, etc.
🧩 Objective

To determine how market sentiment (Fear vs Greed) affects:

Trader profitability (closedPnL)

Trade behavior (size, side)

Volume and activity patterns

Risk tendencies under different emotional market phases

🧠 Key Questions

Do traders earn more during Greed or Fear periods?

Do they take larger positions during Greed?

Is there a bias toward buying or selling depending on sentiment?

Which sentiment phase shows more volatile profits/losses?

Can we extract insights to optimize strategy rules based on market mood?

⚙️ Steps Performed

Data Loading & Inspection

Load both datasets using pandas

Inspect column types, missing values, duplicates

Data Cleaning & Preparation

Convert timestamps to date format

Remove missing and irrelevant rows

Standardize column names

Merge datasets on Date

Exploratory Data Analysis (EDA)

Compare average & median closedPnL across Fear/Greed

Examine trade size and count distribution

Analyze buy vs sell ratios by sentiment

Plot PnL distributions and trends

Visualization (Matplotlib / Seaborn)

Boxplots of closedPnL vs sentiment

Bar charts for trade volume and size

Count plots for buy/sell ratios

Line plots for daily total PnL over time

Insights & Recommendations

Summarize behavioral patterns

Identify risk trends

Suggest sentiment-driven trading adjustments

📊 Example Insights (Expected Findings)


Traders achieve higher average profits during Greed days but with higher volatility.

Trade size increases by ~30% in Greed phases — indicating overconfidence.

Fear periods show more sell orders and smaller trade sizes — signs of risk aversion.

Sentiment flips (Fear→Greed) often precede spikes in total PnL.

🚀 Outcome

Deliverables:

analysis_notebook.ipynb — Python code with data cleaning, EDA, visualizations, and commentary

README.md — This document (project summary)

summary_report.pdf (optional) — 1–2 page summary of findings & strategy recommendations

💻 Tech Stack

Python 3.10+

pandas — data manipulation

numpy — numerical analysis

matplotlib / seaborn — visualizations

scipy — statistical tests
