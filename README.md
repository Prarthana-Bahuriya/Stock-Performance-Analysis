# Stock Performance Analysis of Leading Technology Companies

## Project Overview

This project undertakes the role of a data scientist at an investment firm, focusing on an in-depth analysis of the stock performance of ten influential technology companies: Meta, Apple, Amazon, Netflix, Google, Nvidia, Microsoft, Tesla, Palantir, and Broadcom. These firms are selected for their significant market impact, innovation, and their pivotal role in the modern digital economy.

To provide a broader market context, each company's stock performance is benchmarked against the S&P 500 Index (GSPC), a widely recognized indicator of the overall health and direction of the U.S. economy.

The project follows a complete end-to-end data science pipeline, encompassing data extraction, comprehensive exploratory data analysis (EDA), advanced statistical analysis, and robust time series forecasting. By applying sophisticated modeling techniques, including ARIMA, LSTM (Long Short-Term Memory) neural networks, and Facebook Prophet, the aim is to uncover underlying trends and predict future stock movements.

The ultimate objective is to generate actionable insights for investors and financial analysts, facilitating data-driven decision-making by highlighting both individual company strengths and their alignment with macroeconomic trends within the technology sector.

## Features

* **Automated Data Extraction**: Utilizes `yfinance` and `yahoo_fin` APIs to scrape historical stock data for selected tech companies and the S&P 500 index, ensuring a daily updated dataset.

* **Comprehensive Exploratory Data Analysis (EDA)**: In-depth analysis of key stock metrics including Date, Open, High, Low, Close, and Volume to understand data characteristics and identify initial trends.

* **Advanced Statistical Analysis**: Application of statistical methods to derive meaningful insights from historical stock performance.

* **Time Series Forecasting**: Implementation of three distinct and powerful time series forecasting models:

  * **ARIMA (AutoRegressive Integrated Moving Average)**: A classical statistical method for time series prediction.

  * **LSTM (Long Short-Term Memory) Neural Networks**: A type of recurrent neural network particularly well-suited for learning long-term dependencies in sequential data.

  * **Facebook Prophet**: A forecasting procedure designed for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects.

* **Actionable Insights**: The project's findings are geared towards providing practical information for investors and financial analysts to make informed decisions.

## Technologies Used

* **Python**: The primary programming language for the project.

* **Jupyter Notebook**: For interactive development, data exploration, and presentation of findings.

* **Data Handling**:

  * `pandas`: For data manipulation and analysis.

  * `numpy`: For numerical operations.

  * `yfinance`: For fetching historical stock data.

  * `yahoo_fin`: (Note: The notebook indicates `ModuleNotFoundError` for this library. Ensure it's installed or consider alternative scraping methods if issues persist.)

* **Data Visualization**:

  * `matplotlib.pyplot`: For creating static, interactive, and animated visualizations.

  * `seaborn`: For high-level interface for drawing attractive and informative statistical graphics.

  * `mplfinance`: For financial market visualizations like candlestick charts.

* **Machine Learning & Statistical Modeling**:

  * `scikit-learn` (`MinMaxScaler`): For data preprocessing.

  * `tensorflow` / `keras`: For building and training LSTM neural networks.

  * `statsmodels`: For ARIMA and SARIMAX models, and statistical tests (`adfuller`).

  * `pmdarima`: For auto-ARIMA functionality.

  * `prophet`: For time series forecasting.

* **Utilities**:

  * `os`, `math`, `warnings`, `datetime`, `dateutil.parser`, `IPython.display`.

## Getting Started

To set up and run this project locally, follow these steps:

### Prerequisites

Ensure you have Python installed (preferably Python 3.8+).


### Data Acquisition

The project utilizes web scraping to acquire historical stock data. The `Capstone_2025 (6).ipynb` notebook contains the necessary code to scrape data using `yfinance` and `yahoo_fin` and save it as CSV files into the `data/stock_data/` directory.

1. **Run the data scraping section** in the `Capstone_2025 (6).ipynb` notebook. This will create the `stock_data` directory (if it doesn't exist) and populate it with the scraped CSV files.


## Contributing

Contributions are welcome! If you have suggestions for improvements, bug fixes, or new features, please open an issue or submit a pull request.

---

**Disclaimer**: This project is for educational and analytical purposes only and should not be considered financial advice. Stock market predictions are inherently uncertain, and past performance is not indicative of future results.
