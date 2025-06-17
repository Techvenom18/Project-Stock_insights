# Nifty 50 vs HCL Technologies: Data Analytics Project

## Overview

This project performs a comprehensive data analysis comparing the performance of the Nifty 50 index with HCL Technologies (HCLTECH.NS) stock over a period from 2011 to 2022. The analysis involves collecting historical data, performing descriptive statistics, sampling, z-score analysis, and visualizing the performance of both the index and the stock. The project demonstrates the use of Python for financial data analytics, leveraging libraries such as `pandas`, `numpy`, `matplotlib`, and `yfinance`.

---

## Table of Contents

**1. Data Collection:**

Fetched historical closing prices of Nifty 50 and HDFC Bank from Yahoo Finance using the yfinance library.

Timeframe: January 1, 2010, to January 1, 2024.

**2. Descriptive Statistics:**

Calculated mean, median, mode, standard deviation, variance, skewness, and kurtosis.

Analyzed range and Z-scores for both datasets.

**3. Data Cleaning:**

Handled missing values by dropping NA entries.

Verified data integrity using isna() and describe().

**4. Z-Score Analysis:**

Evaluated the latest and 5 random data points to interpret performance relative to the mean.

**5. Visualizations:**

Included plots (not shown in the notebook) to compare trends between Nifty 50 and HDFC Bank.


---

## Features

- Fetches historical stock/index data using `yfinance`
- Supports multiple indices and stocks (Nifty 50, BSE Sensex, HCL Technologies)
- Computes descriptive statistics for the indices/stocks
- Performs random sampling and calculates z-scores for selected data points
- Provides visualizations to compare the performance of Nifty 50 and HCL Technologies
- Interprets z-scores to assess how selected values perform compared to the average

---

## Setup and Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/<your-username>/nifty-vs-hcl-analysis.git
    cd nifty-vs-hcl-analysis
    ```

2. **Install the required Python libraries:**
    ```sh
    pip install pandas numpy matplotlib yfinance
    ```

3. **Run the main script:**
    ```sh
    python nifty_vs_hcl_analysis.py
    ```

---

## Data Collection

The project fetches historical data for:
- **Nifty 50 Index (`^NSEI`)**
- **BSE Sensex (`^BSESN`)**
- **HCL Technologies (`HCLTECH.NS`)**

The data is collected using the `yfinance` library from January 1, 2011, to December 31, 2022. Both full price data and closing prices are retrieved and organized into pandas DataFrames for further analysis.

---

## Descriptive Statistics

For both Nifty 50 and HCL Technologies, the following statistics are calculated:
- Count
- Mean
- Standard deviation
- Minimum and maximum values
- 25th, 50th (median), and 75th percentiles

These statistics help summarize the overall performance and volatility of each security.

---

## Random Sampling & Z-Score Analysis

- **Random Sampling:** Selects 5 random data points each from Nifty 50 and HCL's closing prices (seeded for reproducibility).
- **Z-Score Calculation:** For each random data point, the z-score is calculated to determine how far the value is from the mean in units of standard deviation.
- **Interpretation:** Each z-score is interpreted as:
    - Above average (z > 0): Performing well
    - Below average (z < 0): Performing poorly
    - At average (z = 0): At mean performance

---

## Visualization

An optional matplotlib plot (can be uncommented in the code) visualizes the price movement of Nifty 50 and HCL Technologies over the selected period on the same graph, providing a clear comparative trend analysis.

---

## Interpretation

The project provides insights into:
- How HCL Technologies' stock price has performed relative to the broader Nifty 50 index.
- The statistical characteristics (mean, volatility) of both securities.
- How randomly selected data points compare to the overall average using z-score analysis.

By running this analysis, you can understand both the absolute and relative performance of a constituent stock (HCL) compared to the index it belongs to (Nifty 50).

---

## Project Structure

```
nifty-vs-hcl-analysis/
│
├── nifty_vs_hcl_analysis.py   # Main Python analysis script
└── README.md                  # Project documentation
```

---

## License

This project is open source and available under the [https://github.com/Techvenom18](GITHUB-ID).

---

## Author

**SUMIT RATHORE**  
ID: 240312060027

---

## Contact

For any query, contact: [sumitrathore45528@gmail.com](mailto:sumitrathore45528@gmail.com)

---
