# Candlestick Pattern Analysis

## Overview
This project involves analyzing candlestick patterns in stock data, specifically for ITC stock. The analysis is conducted using Python and Jupyter Notebooks, leveraging libraries such as `pandas`, `yfinance`, and `matplotlib`.

## Project Structure
The project consists of the following main components:

- **Data Retrieval**: Fetches historical stock data from Yahoo Finance.
- **Data Processing**: Prepares the data for analysis by formatting dates and extracting relevant price information.
- **Extrema Detection**: Implements a method to identify local maxima and minima in the stock prices using kernel regression.
- **Visualization**: Visualizes the stock price trends and detected patterns.

## Requirements
To run this project, you need to have the following Python libraries installed:
- `pandas`
- `yfinance`
- `numpy`
- `matplotlib`
- `scipy`
- `statsmodels`

You can install these libraries using pip:
```bash
pip install pandas yfinance numpy matplotlib scipy statsmodels
```

## Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/harshgupta1810/ChartVantage.git
   cd ChartVantage
   ```

2. **Open the Jupyter Notebook**:
   Launch Jupyter Notebook from your terminal:
   ```bash
   jupyter notebook
   ```
   Then open the appropriate notebook file.

3. **Run the Cells**:
   Execute each cell in the notebook sequentially to fetch and analyze the stock data.

## Code Breakdown

### Importing Libraries
The necessary libraries are imported at the beginning of the notebook:
```python
import pandas as pd
import yfinance
import numpy as np
import matplotlib.dates as mpl_dates
import matplotlib.pyplot as plt
from datetime import date
from scipy.signal import argrelextrema
from statsmodels.nonparametric.kernel_regression import KernelReg
```

### Fetching Stock Data
The code retrieves historical data for ITC stock from Yahoo Finance:
```python
stocksymbols = 'ITC.NS'
ticker = yfinance.Ticker(stocksymbols)
end = date.today()
start = "2020-01-01"
df = ticker.history(interval="1d", start=start, end=end)
```

### Data Preparation
The date is formatted, and only closing prices are retained for analysis:
```python
df['Date'] = pd.to_datetime(df.index)
df['Date'] = df['Date'].apply(mpl_dates.date2num)
df.index = pd.to_datetime(df.index, errors='coerce')
df.index = df.index.strftime('%d-%m-%y')
df = df.loc[:, ['Close']]
```

### Finding Extrema Function
A function is defined to find local extrema in the price data:
```python
def find_extrema(s, bw='cv_ls'):
    """
    Input:
    s: prices as pd.Series
    bw: bandwidth as str or array-like
    
    Returns:
    prices: with 0-based index as pd.Series
    extrema: extrema of prices as pd.Series
    smoothed_prices: smoothed prices using kernel regression as pd.Series
    smoothed_extrema: extrema of smoothed_prices as pd.Series
    """
    # Function implementation...
```

### Creating DataFrame for Prices
The closing prices are organized into a new DataFrame:
```python
price = df['Close']
index = df.index
df1 = pd.DataFrame({'Price': price}, index=index)
df1.index.name = 'Date'
```

### Executing Extrema Detection
The extrema are calculated based on the closing prices:
```python
extrema, price, smooth_extrema, smooth_prices = find_extrema(df1)
```

### Visualization of Results (Example)
Visualizations can be created using matplotlib to display stock price trends and patterns.

## Conclusion
This project provides a comprehensive approach to analyzing candlestick patterns in financial data. By leveraging Python's powerful libraries, users can effectively retrieve, process, and visualize stock market trends.

For any issues or contributions, feel free to open an issue or submit a pull request!
