# Candlestick Chart Visualization
This GitHub repository contains a Python script for generating a candlestick chart of stock data using the Plotly and Dash libraries. The script downloads stock data from Yahoo Finance for a user-specified company code and time range, and generates a candlestick chart of the company's stock price movements during that time period. The chart can be displayed with or without a range slider using a toggle button in a Dash web app. The repository can be useful for anyone interested in visualizing stock price data in a clear and concise manner using Python.

## Installation
This script requires the following libraries to be installed:

* plotly
* pandas
* yfinance
* dash

You can install these libraries using pip with the following command:
``pip install plotly pandas yfinance dash``

## Usage
To use this script, you need to specify the company code for the stock you want to visualize. Run the script and enter the code when prompted.

``company_name=input('Enter Company Code: ')``

The script will then download the stock price data from Yahoo Finance and create a candlestick chart visualization. By default, the chart includes a rangeslider, which can be toggled on and off using the checkbox provided.


``dcc.Checklist(
    id='toggle-rangeslider',
    options=[{'label': 'Include Rangeslider', 
              'value': 'slider'}],
    value=['slider']
),``

The visualization will be displayed in an interactive web page using the Dash library.

``
app.run_server(debug=True)
``

## Examples:
Here are some examples of the generated charts:


<img width="1310" alt="Jepretan Layar 2023-04-19 pukul 13 52 07" src="https://user-images.githubusercontent.com/86939625/232990441-f9383386-c62b-4f90-8c90-847f897b497a.png">


<img width="1310" alt="Jepretan Layar 2023-04-19 pukul 13 53 22" src="https://user-images.githubusercontent.com/86939625/232991051-1576d978-346a-43eb-acb9-bc5a4eee8623.png">


