# Trader Performance vs Market Sentiment Analysis

## Objective
The objective of this assignment is to analyze how Bitcoin market sentiment (Fear vs Greed)
influences trader behavior and performance on the Hyperliquid trading platform.
The goal is to uncover patterns that can inform more sentiment-aware trading strategies.

## Datasets
1. Bitcoin Fear & Greed Index  
   - Columns: timestamp, value, classification, date  
   - Provides daily market sentiment classified as Fear or Greed

2. Historical Trader Data (Hyperliquid)  
   - Columns include: Account, Coin, Execution Price, Size Tokens, Size USD, Side,
     Timestamp, Closed PnL, Direction, etc.
   - Contains trade-level execution and performance details

## Methodology
- Loaded and inspected both datasets for missing values and duplicates
- Converted timestamps and aligned both datasets at a daily level using the `date` column
- Merged trade data with daily market sentiment
- Engineered key metrics such as:
  - Daily PnL per trader
  - Win rate
  - Trade frequency
  - Position size / exposure proxy
  - Long vs Short bias
- Compared trader behavior and performance across Fear and Greed regimes
- Segmented traders based on exposure and trading frequency
- Derived actionable strategy recommendations from observed patterns

## Key Outputs
- Comparison of PnL and win rates between Fear and Greed days
- Analysis of behavioral changes such as trade frequency and position sizing
- Trader segmentation insights
- Two actionable strategy recommendations

## How to Run
1. Install required libraries:

2. Open the Jupyter notebook:

3. Run all cells sequentially to reproduce the analysis and charts

## Notes
This project focuses on clarity of reasoning, correctness of data alignment,
and actionable insights rather than complex modeling.
