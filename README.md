# FRED API Financial and Economic Data Analysis

This project explores, retrieves, and visualizes various economic and financial indicators using the Federal Reserve Economic Data (FRED) API. The analysis focuses on key U.S. metrics such as the S&P 500, unemployment rates, Index Funds, and Gross Domestic Product (GDP).

## 📊 Features
* Data Sourcing: Connects to the FRED API to fetch real-time and historical economic datasets.
* Interactive Exploration: Implements multi-attribute filtering and parsing of the FRED dataset catalog.
* Advanced Visualization: Leverages Matplotlib, Seaborn, and Plotly Express for time-series analysis and market trend plotting.

## 🛠️ Tech Stack & Libraries
* Python (Core Environment)
* fredapi (Official FRED API wrapper)
* pandas & numpy (Data cleaning and preprocessing)
* matplotlib & seaborn (Static statistical charts)
* plotly.express (Interactive dynamic data charting)
* python-dotenv (Secure API key environment management)

## 🚀 Getting Started

### 1. Prerequisites & Installation
Install the required dependencies directly via pip:
pip install fredapi pandas numpy matplotlib seaborn plotly python-dotenv

### 2. API Key Setup
1. Get a free API key from the St. Louis Fed (FRED) website.
2. Create a .env file in your root directory.
3. Add your key into the file:
FRED_API_KEY=your_actual_api_key_here

### 3. Usage
Run your Jupyter Notebook cells to execute the data pipeline:
* Load your environment credentials using dotenv.
* Initialize the FRED client with your API key.
* Use fred.search('S&P', order_by='popularity') to find and filter your target datasets.

## 📈 Pipeline Overview
1. API Initialization & Authentication: Loads secure configurations and instantiates the FRED client connection.
2. Metadata Discovery: Searches and sorts historical macroeconomic listings based on indexing metrics like popularity and seasonal adjustments.
3. Data Acquisition: Extracts U.S. financial indicators (e.g., S&P 500 daily market closes) across specified date constraints.
4. Visualization Engine: Generates analytical time-series graphs to track asset performance and macro-level trends over time.
