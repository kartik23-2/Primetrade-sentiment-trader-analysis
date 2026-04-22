# Primetrade.ai Technical Assignment  
## Bitcoin Market Sentiment vs Trader Performance Analysis

**Candidate:** Kartik Baliyan  

---

# Overview

This project analyzes the relationship between **market sentiment** and **trader performance** using two datasets provided in the assignment:

1. **Fear & Greed Index Dataset** – captures daily market sentiment.  
2. **Hyperliquid Historical Trader Data** – contains real trade execution records.

The goal is to uncover hidden behavioral patterns and generate actionable insights that can improve trading strategies.

---

# Assignment Objective

> Explore the relationship between trader performance and market sentiment, uncover hidden patterns, and deliver insights that can drive smarter trading strategies.

---

# Datasets Used

## 1. Fear & Greed Index Dataset

Columns include:

- `date`
- `classification` (Fear / Greed / Neutral / etc.)
- `value`

Used as a proxy for crypto market psychology.

---

## 2. Historical Trader Dataset

Columns include:

- `Account`
- `Coin`
- `Execution Price`
- `Size Tokens`
- `Size USD`
- `Side`
- `Timestamp IST`
- `Closed PnL`
- `Fee`
- `Direction`

Used to evaluate real trader behavior and performance.

---

# Methodology

## Step 1: Data Cleaning

- Removed formatting issues
- Converted timestamps to datetime
- Converted numeric columns
- Checked missing values

## Step 2: Data Integration

Merged both datasets using common trading date.

## Step 3: Feature Engineering

Created new features:

- `win_trade`
- `net_pnl`
- `sentiment_score`

## Step 4: Exploratory Data Analysis

Analyzed:

- Average profit by sentiment
- Win rate by sentiment
- Trade activity levels
- Buy vs Sell behavior
- Top profitable coins
- Top performing traders

## Step 5: Strategic Interpretation

Converted findings into business recommendations.

---

# Key Questions Answered

1. Do traders perform better in Fear or Greed markets?  
2. Does sentiment impact win rate?  
3. Are traders more aggressive during Greed periods?  
4. Which assets perform consistently?  
5. Can sentiment be used as a trading signal?

---

# Project Structure

```text
Primetrade_Assignment/
├── Primetrade_Final_Humanized_Notebook.ipynb
├── Primetrade_Final_Report_Updated.pdf
├── README.md
├── requirements.txt
├── fear_greed_index.csv
└── historical_data.csv