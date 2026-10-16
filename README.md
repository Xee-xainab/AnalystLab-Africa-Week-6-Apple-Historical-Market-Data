# 📈 Apple Inc. (AAPL) Historical Stock Market Analysis Using Python 

**Week 6 Internship Project | AnalystLab Africa (Batch B, 1 June to 1 August 2026)**
**Author:** Danjuma Zainab

Can five years of Apple stock data show how the price trends, when trading spikes, how risky the stock is, and which months behave differently? This project answers those questions with Python.

## The Business Problem

Investors and analysts need clear, data-backed answers on trend, trading activity, risk and seasonality before deciding when to hold, trim or add exposure to a stock.

## Dataset

- **Source:** Yahoo Finance via the `yfinance` library
- **Period:** 6 Aug 2021 to 4 Aug 2026 (5 years)
- **Size:** 1,253 trading days after cleaning
- **Columns:** Date, Open, High, Low, Close, Adj Close, Volume

## Tools

Python, Pandas, NumPy, Matplotlib, yfinance, Jupyter Notebook

## Data Cleaning

The raw file loaded as 1,254 rows x 8 columns with every price column stored as text.

1. Removed the stray first row (the ticker "AAPL" repeated in every column) added by yfinance
2. Dropped the redundant `index` column
3. Converted Open, High, Low, Close and Adj Close to numeric, and Volume to integer
4. Converted `Date` to datetime
5. Checked for missing values (none remained)
6. Sorted the data chronologically
7. Final dataset: **1,253 rows x 7 columns**

## Feature Engineering

| Feature | Definition |
|---|---|
| Daily Price Change | Close - Open |
| Percentage Price Change | (Close - Open) / Open x 100 |
| Year, Month, Month Number | Extracted from Date |
| 7-Day and 30-Day Moving Average | Rolling mean of Close |
| Volatility | 30-day rolling standard deviation of Percentage Price Change |

## Key Statistics

| Metric | Value |
|---|---|
| Average close | $199.12 (median $187.87) |
| Highest close | $340.08 on 28 Jul 2026 |
| Lowest close | $125.02 on 5 Jan 2023 |
| Highest volume | 318.68M shares on 20 Sep 2024 |
| Average daily change | 0.12% (std. dev. 1.50%) |
| 30-day volatility | Average 1.40%, range 0.64% to 3.87% |

## Insights

1. **The price more than doubled.** Apple rose from $146.14 (Aug 2021) to a peak of $340.08 (28 Jul 2026), about +133%, and closed above both its 7-day ($330.27) and 30-day ($310.46) averages at the peak, showing a sustained uptrend rather than a one-day spike.
2. **The 2023 low was followed by a strong recovery.** The close bottomed at $125.02 on 5 Jan 2023, below its 30-day average of $138.49 during the broad 2022 sell-off, then climbed about 172% to the peak.
3. **The heaviest trading day was not a big price day.** Volume hit 318.68M on 20 Sep 2024, over five times the median, yet price moved only -0.77%, pointing to a mechanical event such as index rebalancing or options expiry rather than company news.
4. **Risk arrives in bursts.** 30-day volatility averaged 1.40% but ranged from 0.64% to 3.87%, with 75% of readings below 1.70%, because market-wide shocks hit in short clusters while calm periods dominate.
5. **July, November and October were the strongest months** (+0.32%, +0.28%, +0.25% average daily gain) while September was weakest (-0.14%), though five years of data is too short to treat this as proven.

## Recommendations

1. **Use moving averages as a trend filter:** treat price above the 30-day average as confirmation, and a close below it as a prompt to review.
2. **Read volume together with price:** flat-price volume spikes are usually mechanical, not signals.
3. **Size positions by volatility:** consider reducing exposure when 30-day volatility rises above about 1.70%.
4. **Do not trade on seasonality alone:** validate on 10+ years of data and close-to-close returns first.
5. **Extend the analysis:** benchmark against the S&P 500, add RSI and Bollinger Bands, and backtest any rule.

## Visualizations

The notebook produces: closing price trend, trading volume trend, closing price with 7- and 30-day moving averages, daily percentage change, average monthly percentage change, and 30-day volatility.

## Repository Structure

```
.
├── AAPL_Stock_Analysis.ipynb   # Full analysis notebook
├── AAPL_Historical_Data.csv    # Downloaded dataset
├── AAPL_Stock_Analysis_Report.pdf
└── README.md
```

## How to Run

```bash
pip install yfinance pandas numpy matplotlib jupyter
jupyter notebook AAPL_Stock_Analysis.ipynb
```

## Disclaimer

This project is for learning purposes only and is not financial advice.

