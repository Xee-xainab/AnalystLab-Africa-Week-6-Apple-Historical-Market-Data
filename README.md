# 📈 Apple Inc. (AAPL) Historical Stock Market Analysis Using Python

## 📌 Project Overview

This project was completed as part of **Week 6 of the AnalystLab Africa Batch B Internship Program (1st June – 1st August 2026)**.

The objective of this project was to analyze **Apple Inc. (AAPL) historical stock market data** using Python by applying advanced data transformation, time-series analysis, feature engineering, and data visualization techniques to uncover meaningful insights into stock performance.

---

## 🎯 Project Objectives

- Clean and preprocess historical stock market data.
- Perform advanced data transformation using Pandas.
- Conduct time-series analysis on stock prices.
- Engineer new features to improve analysis.
- Create insightful visualizations.
- Generate actionable business insights and recommendations.

---

## 📂 Dataset Information

- **Dataset:** Apple Inc. (AAPL) Historical Stock Data
- **Source:** Yahoo Finance
- **Period:** Five Years
- **Records:** 1,252
- **Features:**
  - Date
  - Open Price
  - High Price
  - Low Price
  - Close Price
  - Adjusted Close Price
  - Trading Volume

---

## 🛠 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Jupyter Notebook

---

## 📊 Project Workflow

### 1. Data Loading

- Imported required Python libraries.
- Downloaded Apple historical stock data using the **yfinance** library.
- Loaded the dataset into a Pandas DataFrame.

---

### 2. Data Exploration

Performed exploratory analysis by:

- Viewing the dataset
- Checking dataset dimensions
- Examining data types
- Generating summary statistics
- Identifying missing values

---

### 3. Data Cleaning

The following preprocessing steps were performed:

- Removed unnecessary columns
- Converted the Date column to datetime format
- Converted numeric columns to appropriate data types
- Sorted data chronologically
- Verified missing values

---

### 4. Data Transformation

Created additional variables including:

- Daily Price Change
- Percentage Price Change
- Year
- Month
- Month Number

These transformations improved the dataset for further analysis.

---

### 5. Time-Series Analysis

Performed time-series analysis including:

- Closing Price Trend
- Trading Volume Trend
- 7-Day Moving Average
- 30-Day Moving Average
- Daily Percentage Price Change

---

### 6. Feature Engineering

Created the following analytical features:

- Daily Price Change
- Percentage Price Change
- 7-Day Moving Average
- 30-Day Moving Average
- Monthly Returns
- 30-Day Volatility
- Year
- Month
- Month Number

---

## 📈 Visualizations

The project includes the following visualizations:

- 📊 Apple Stock Closing Price Trend
- 📊 Trading Volume Trend
- 📊 Closing Price vs 7-Day & 30-Day Moving Averages
- 📊 Daily Percentage Price Change
- 📊 Monthly Average Returns
- 📊 30-Day Stock Volatility

---

## 🔍 Key Findings

- Apple experienced an overall upward trend during the analysis period.
- Daily price fluctuations reflected normal stock market volatility.
- The 7-day moving average highlighted short-term trends, while the 30-day moving average captured long-term price movements.
- Trading volume varied considerably, indicating changes in investor activity.
- Monthly returns differed across the year, showing seasonal variation in stock performance.
- Volatility analysis identified periods of both market stability and increased uncertainty.

---

## 💡 Recommendations

- Monitor moving averages to identify emerging market trends.
- Combine trading volume analysis with price movements for better investment decisions.
- Use volatility measures to evaluate investment risk.
- Perform regular time-series analysis to support data-driven financial decisions.

---

## 📁 Repository Structure

```text
Apple-Stock-Analysis/
│
├── Data/
│   └── AAPL_Historical_Data.csv
│
├── Notebook/
│   └── AAPL_Stock_Analysis.ipynb
│
├── Images/
│   ├── Closing_Price_Trend.png
│   ├── Trading_Volume_Trend.png
│   ├── Moving_Averages.png
│   ├── Daily_Percentage_Change.png
│   ├── Monthly_Returns.png
│   └── Stock_Volatility.png
│
├── Report/
│   └── Insight_Summary.pdf
│
└── README.md
```

---

## 🚀 Skills Demonstrated

- Python Programming
- Pandas Data Manipulation
- Data Cleaning
- Data Transformation
- Time-Series Analysis
- Feature Engineering
- Data Visualization
- Financial Data Analysis
- Business Insight Generation

---

## 👩‍💻 Author

**Danjuma Zainab**

Data Analyst | Python | SQL | Excel | Power BI

---

## 🙏 Acknowledgements

This project was completed as part of the **Week 6 Internship Project** under the **AnalystLab Africa Batch B Internship Program**, providing hands-on experience in Python-based financial data analysis and time-series analytics.

---

⭐ If you found this project helpful, feel free to star this repository!
