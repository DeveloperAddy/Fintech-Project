# Stock Portfolio Analysis and Value Investing

This repository contains three Python-based projects for stock portfolio analysis, focusing on value investing and dividend-based shortlisting.  These projects utilize the `yfinance` library to fetch stock data and `pandas` for data manipulation and analysis.

## Project Descriptions

### 1. Stock Quantity Shortlisting

This project takes a user-defined investment amount as input and calculates the quantity of each stock that can be purchased within that budget.  It retrieves the latest stock prices and then determines the maximum number of shares that can be bought for each ticker without exceeding the total investment.

*   **Key Features:**
    *   Takes user input for the total investment amount.
    *   Fetches real-time stock prices using `yfinance`.
    *   Calculates the affordable quantity of each stock.
    *   Provides a clear output of stock tickers and their corresponding quantities.

### 2. Value Investing Stock Screener

This project implements a value investing strategy to shortlist potentially undervalued stocks. It calculates key financial ratios (P/E, P/B, P/S, EV/EBITDA, EV/GP) and uses these metrics to identify stocks that might be trading below their intrinsic value.

*   **Key Features:**
    *   Retrieves financial data for a list of tickers.
    *   Calculates essential value investing ratios.
    *   Handles missing data gracefully using `numpy.nan`.
    *   Provides a DataFrame with the calculated ratios for further analysis.

### 3. Top 10 Dividend Stocks

This project shortlists the top 10 stocks based on their dividend scores. It retrieves dividend yield data and identifies the top performers, providing a list of high-dividend-paying stocks.

*   **Key Features:**
    *   Fetches dividend yield information for a set of tickers.
    *   Calculates a composite dividend score (potentially combining multiple dividend-related metrics if available).
    *   Sorts stocks based on the dividend score.
    *   Returns the top 10 dividend-paying stocks.

## Technologies Used

*   Python
*   `yfinance`
*   `pandas`
*   `numpy`
*   `scipy` (for percentile calculations in value investing project)

## Installation

1.  Clone the repository:

    ```bash
    git clone [[https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/DeveloperAddy/Fintech-Project.git)]
    ```

2.  Navigate to the project directory:

    ```bash
    cd FINTECH-PROJECT
    ```

3.  Create a virtual environment (recommended):

    ```bash
    python3 -m venv .venv  # Or python -m venv .venv depending on your system
    ```

4.  Activate the virtual environment:

    *   **Linux/macOS:**

        ```bash
        source .venv/bin/activate
        ```

    *   **Windows:**

        ```bash
        .venv\Scripts\activate
        ```

5.  Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```
    (Create a `requirements.txt` file in your project root with the package names: `yfinance`, `pandas`, `numpy`, `scipy`)

## Usage

Provide instructions on how to run each of the projects.  For example:

```bash
python stock_quantity_shortlisting.py  # Example
python value_investing_screener.py     # Example
python top_10_dividend_stocks.py      # Example
