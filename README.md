# Module-3-Challenge

For this project, I collected, prepared, and analyzed historical trade data for Bitcoin on two exchanges: Bitstamp and Coinbase. I went through the three phases of financial analysis to determine if any arbitrage opportunities exist for Bitcoin.

---

## Technologies

This project uses pandas programming language and utilizes Anaconda, Git Bash, Jupyter Lab, and Github.

---

## Installation Guide

You must install and git for Jupyter Lab. Run the following commands in Git Bash before importing them in your code.

*pip install --upgrade jupyterlab jupyterlab-git

These must also be imported before running the code:

import pandas as pd
from pathlib import Path
%matplotlib inline

---

## Usage

I brought in historical data:

bitstamp = pd.read_csv(
    Path(r'C:\Users\abcar\Desktop\Challenge_3_Starter_Code\Module-3-Challenge\Resources\bitstamp.csv'), 
    index_col="Timestamp", 
    parse_dates = True, 
    infer_datetime_format = True
)

Cleaned the data:

coinbase = coinbase.fillna('Unknown')

Analyzed the data:

bitstamp_sliced.loc['2018-01-28'].plot(color='red', title='Bitstamp and Coinbase Closing Price 1/28/18', figsize=(10,5), legend=True, label='Bitstamp')
coinbase_sliced.loc['2018-01-28'].plot(color='blue', figsize=(10,5), legend=True, label='Coinbase')

---

## Contributors

Allyssa Carmin

---

## License

SMU Fintech Course