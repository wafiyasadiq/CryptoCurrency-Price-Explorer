**CryptoCurrency Price Explorer**

CryptoCurrency Price Explorer is a Python-based project designed to fetch, analyze, and visualize the price trends of multiple cryptocurrencies, including Bitcoin, Ethereum, and Binance Coin, using data from the CoinGecko API. The project provides actionable insights into cryptocurrency trends and market behavior.

**🚀 Features**

Fetches real-time and historical cryptocurrency price data using the CoinGecko API.
Compares price trends across multiple cryptocurrencies.
Visualizes trends, distributions, and volatility through graphs and charts.
Provides a comprehensive analysis of market trends, including volatility and rolling averages.

**🗂️ Dataset Description**

Data Source
The dataset is fetched directly from the CoinGecko API, which provides:

Historical price data.
Market metrics such as trading volume.
Structure
The data for each cryptocurrency includes:

Timestamp: Unix timestamp of the price data.
Price: Closing price of the cryptocurrency (in USD).
Volume (optional): Trading volume during the time period.
Example JSON structure returned by the API:

json
Copy code
{
    "prices": [
        [1640995200000, 47120.34],
        [1641081600000, 47024.57],
        ...
    ],
    "total_volumes": [
        [1640995200000, 25483783982],
        [1641081600000, 24284030083],
        ...
    ]
}

**🛠️ What We Have Done**

1. Data Collection
Used the CoinGecko API to fetch historical price data for Bitcoin, Ethereum, and Binance Coin for the last 30 days.
Implemented a robust Python function to handle API calls and error handling.
2. Data Preprocessing
Converted timestamps into human-readable dates.
Extracted features such as price differences, moving averages, and volatility indicators.
3. Data Visualization
Plotted time-series graphs to compare price trends across cryptocurrencies.
Visualized price distributions and volatility.
Created heatmaps to analyze daily percentage changes.

**📊 Visualizations**

Here are some of the visualizations included in this project:

Time-Series Plots: Comparison of prices across cryptocurrencies.

Price Distribution: Histogram of price data to understand distribution and outliers.

Rolling Volatility: Analysis of market stability.

Correlation Heatmaps: Relationships between price and trading volume.

**📦 Installation**

Prerequisites
Python 3.7+
Install required libraries:
bash
Copy code
pip install requests pandas matplotlib seaborn

**🚀 Future Enhancements**

Add support for more cryptocurrencies.
Build an interactive dashboard using Streamlit or Flask for real-time insights.
Incorporate sentiment analysis from financial news or social media.

**🤝 Contributions**

Contributions are welcome! Feel free to submit a pull request or open an issue for improvements.

**🛡️ License**

This project is licensed under the MIT License. See the LICENSE file for details.

🌟 Acknowledgments
Special thanks to CoinGecko for their free cryptocurrency data API.

