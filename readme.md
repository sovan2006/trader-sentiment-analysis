# Trader Performance vs Market Sentiment Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader performance on the Hyperliquid platform. The objective is to identify behavioral patterns and performance differences based on market sentiment, and propose actionable trading strategies.

This analysis was completed as part of the Primetrade.ai Data Science Intern assignment.

---

## Dataset Description

Two datasets were used:

### 1. Bitcoin Market Sentiment Dataset
- Columns:
  - date: Date of sentiment measurement
  - value: Fear/Greed index value
  - classification: Sentiment category (Fear, Greed, Extreme Fear, Extreme Greed)

### 2. Historical Trader Dataset
- Columns include:
  - Account: Trader account address
  - Coin: Trading symbol
  - Execution Price: Price at execution
  - Size USD: Trade size in USD
  - Side: Buy/Sell
  - Timestamp IST: Trade timestamp
  - Closed PnL: Profit or loss per trade
  - Fee: Transaction fee

---

## Methodology

### Data Preparation
- Loaded both datasets using pandas
- Cleaned column names and removed duplicates
- Converted timestamps to datetime format
- Created daily Date column for alignment
- Merged trader data with sentiment data on Date

### Feature Engineering
Created key metrics including:
- Daily PnL per trader
- Win rate per trader
- Average trade size
- Trade frequency
- Long vs Short ratio

---

## Analysis & Key Findings

### Insight 1: Profitability varies with market sentiment
- Traders show higher average profit during Greed periods compared to Fear periods.

### Insight 2: Trade frequency increases during Greed sentiment
- Traders are more active when market sentiment is positive.

### Insight 3: Trade size influences profit volatility
- Larger trades contribute significantly to overall profit variability.

---

## Trader Segmentation

Traders were segmented based on:

- Frequent vs Rare traders
- Consistent vs Inconsistent traders
- Trade size behavior

Consistent traders demonstrated better long-term performance.

---

## Strategy Recommendations

### Strategy 1: Increase trading activity during Greed periods
Greed sentiment correlates with higher profitability and better trading outcomes.

### Strategy 2: Reduce position size during Fear periods
Fear periods show increased volatility and risk exposure.

---

## Visualizations Included

- PnL distribution
- Trade size distribution
- Profit by sentiment
- Trade frequency by sentiment
- Long vs Short ratio

---

## Project Structure

Trader-Sentiment-Analysis/
│
├── Analysis.ipynb
├── fear_greed_index.csv
├── historical_data.csv
├── README.md
└── requirements.txt

---

---

## How to Run

### Step 1: Clone repository

git clone <your-github-repo-link>
cd Trader-Sentiment-Analysis

### Step 2: Install dependencies

pip install -r requirements.txt

### Step 3: Run notebook

jupyter notebook Analysis.ipynb

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Author

Sovan Barik  
B.Tech Artificial Intelligence and Machine Learning  
