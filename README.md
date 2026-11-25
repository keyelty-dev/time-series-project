# Time Series Analysis – AirPassengers

## Project Overview
This project explores time series analysis using the **AirPassengers dataset**, which contains monthly international airline passenger numbers from 1949 to 1960.

The main goal is to identify trends and seasonal patterns, apply different smoothing techniques, and perform time series forecasting using Python.

## Dataset
- **Dataset:** AirPassengers
- **Time Period:** January 1949 – December 1960
- **Frequency:** Monthly
- **Number of Observations:** 144
- **Target Variable:** Number of Passengers

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Jupyter Notebook

## Analysis Steps

### 1. Exploratory Data Analysis (EDA)
- Loading and inspecting the dataset
- Converting the date column to datetime format
- Setting the date column as the index
- Visualizing passenger numbers over time
- Analyzing average passenger numbers by month

### 2. Time Series Decomposition
Decomposing the time series into three main components:
- **Trend:** Long-term movement in passenger numbers
- **Seasonality:** Repeating patterns over time
- **Residual:** Remaining variations not explained by trend and seasonality

### 3. Smoothing Techniques
Applying and comparing three smoothing methods:

- **Simple Moving Average (SMA):** Using a 12-month rolling window to smooth short-term fluctuations.
- **Simple Exponential Smoothing:** Applying exponential weights to past observations.
- **Holt-Winters Exponential Smoothing:** Modeling trend and seasonality together.

Residual analysis and histograms were also used to examine the performance of the smoothing methods.

### 4. Forecasting
The dataset was divided chronologically into training and testing sets:

- **Training Set:** January 1949 – December 1959
- **Testing Set:** January 1960 – December 1960

A Holt-Winters model was trained on the training data to forecast passenger numbers for the next 12 months. The predicted values were then compared with the actual passenger counts.

## Key Findings
- Passenger numbers show a clear upward trend over time.
- The dataset contains a strong yearly seasonal pattern.
- July and August generally have the highest average passenger numbers.
- February and November generally have some of the lowest average passenger numbers.
- Holt-Winters performed better than the other smoothing methods in this analysis.
- The forecasted values were reasonably close to the actual passenger numbers in 1960.

## Project Structure

```text
.
├── time series/
│   ├── AirPassengers_Time_Series_Analysis.ipynb
│   └── airline-passengers.csv
│
└── README.md
```

## Conclusion
This project demonstrates the application of time series analysis, including exploratory data analysis, decomposition, smoothing techniques, and forecasting.

By comparing different smoothing methods, we explored how trend and seasonality can be identified and modeled. Finally, the Holt-Winters method was used to forecast future passenger numbers based on historical data.
