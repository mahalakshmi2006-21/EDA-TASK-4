# 📊 Shopify Stock Data – Exploratory Data Analysis

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** on historical stock market data of **Shopify Inc. (SHOP)**.

The analysis focuses on understanding Shopify's stock price movements, daily returns, trading range, and market activity using statistical analysis and data visualizations.

The dataset contains historical Shopify stock data from **May 21, 2015 to March 14, 2025**.

---

## 🎯 Objectives

* Understand the structure and characteristics of Shopify stock data.
* Perform data cleaning and preprocessing.
* Analyze Shopify's historical **Open, High, Low, and Close (OHLC)** prices.
* Study Shopify's closing-price movement over time.
* Calculate and analyze daily price changes and daily returns.
* Analyze Shopify's moving average to observe price trends.
* Examine the distribution of daily returns using **KDE (Kernel Density Estimation)**.
* Study price range and trading volume.
* Identify patterns and variations in Shopify's stock performance.

---

## 📂 Dataset

**Dataset:** `SHOP_2015-05-21.csv`

The dataset contains **2,469 records** and **7 columns**.

| Column      | Description                        |
| ----------- | ---------------------------------- |
| `date`      | Trading date                       |
| `open`      | Opening stock price                |
| `high`      | Highest stock price during the day |
| `low`       | Lowest stock price during the day  |
| `close`     | Closing stock price                |
| `adj_close` | Adjusted closing price             |
| `volume`    | Number of shares traded            |

**Date Range:** May 21, 2015 – March 14, 2025

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statistical Analysis

---

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the Shopify stock dataset using Pandas.
2. Inspected the dataset using shape, head, and data types.
3. Checked for missing values.
4. Checked for duplicate records.
5. Converted the `date` column into a datetime format.
6. Sorted the data according to the trading date.
7. Set the `date` column as the DataFrame index.
8. Removed any remaining null values.

The original dataset contained **no missing values**.

---

## ⚙️ Feature Engineering

Three additional features were created for the analysis.

### 1. Daily Price Change

```text
Daily Price Change = Close - Open
```

This represents the change in Shopify's stock price during a trading day.

### 2. Daily Return %

```text
Daily Return % = ((Close - Open) / Open) × 100
```

This measures the percentage change between the opening and closing prices.

### 3. Price Range

```text
Price Range = High - Low
```

This represents the difference between the highest and lowest price during a trading day.

---

## 📈 Statistical Analysis

The daily return and price range were analyzed using descriptive statistics.

| Statistic                 |          Value |
| ------------------------- | -------------: |
| Mean Daily Return         |       ~0.0864% |
| Return Variance           |        ~9.7331 |
| Return Standard Deviation |       ~3.1198% |
| Minimum Daily Return      |     ~-12.1998% |
| Maximum Daily Return      |      ~20.0222% |
| Mean Price Range          |        ~2.1577 |
| Mean Trading Volume       | ~16,570,491.78 |

These statistics provide an overview of Shopify's daily price variation and trading activity during the analyzed period.

---

# 📊 Data Visualizations

## 1. Shopify OHLC Prices

This visualization shows Shopify's **Open, High, Low, and Close prices** over the analyzed period. It helps in understanding the overall movement and variation of Shopify's stock prices.

<img width="501" height="244" alt="Screenshot 2026-09-17 201919" src="https://github.com/user-attachments/assets/af95134f-725a-49ad-be3d-13a455c683b3" />


---
---

## 2. Shopify Moving Average

The moving average visualization helps observe the underlying trend of Shopify's stock price by smoothing short-term fluctuations.
<img width="503" height="245" alt="Screenshot 2026-09-17 201901" src="https://github.com/user-attachments/assets/b98d5168-7437-49a3-88ed-2536bcfd3f50" />



---

## 3. KDE of Shopify Daily Returns

The KDE (Kernel Density Estimation) plot shows the estimated distribution of Shopify's daily returns and helps visualize the concentration and spread of returns.

<img width="425" height="233" alt="Screenshot 2026-09-17 201841" src="https://github.com/user-attachments/assets/ce4e11d7-cfc8-4de7-a3b0-f3e6688d9471" />


---

## 🔍 Key Findings

* Shopify's stock price experienced substantial changes throughout the analyzed period.
* Daily returns showed noticeable variation, indicating fluctuations in daily stock performance.
* The daily return distribution can be examined using KDE to understand the concentration and spread of returns.
* The OHLC visualization provides an overview of the relationship between opening, closing, high, and low prices.
* Moving averages help identify broader price trends by reducing short-term fluctuations.
* Trading volume varied considerably across the analyzed period.
* The price range provides insight into the level of daily price movement.

---

## 📁 Project Structure

```text
Task3&4EDA/
│
├── Task3&4EDA.ipynb
├── SHOP_2015-05-21.csv
├── README.md
│
└── images/
    ├── shopify_ohlc_prices.png
    ├── shopify_closing_prices.png
    ├── shopify_moving_average.png
    └── kde_shopify_daily_returns.png
```

---


---

## 📝 Conclusion

This project demonstrates the application of **Exploratory Data Analysis techniques to Shopify stock market data**.

Through data preprocessing, feature engineering, statistical analysis, and visualization, the project examines Shopify's historical price movements, daily returns, trading activity, and overall price trends.

The analysis provides a clear understanding of the characteristics and variability of Shopify's stock data over the selected period.
