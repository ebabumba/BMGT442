# Quant Backtest Project

This project builds and backtests a long-short equity strategy using factor models.

## Team Members
- Eria Babumba
- Brendan Auville
- Eros Bittick
- Jennifer Carrer Pena 

## Plan
- Collect data
- Build factor model
- Run backtest
- Evaluate performance


## Project Structure
data/
    raw/            ← place raw CRSP data here (NOT included in repo)
    processed/      ← cleaned datasets
notebooks/          ← data cleaning and analysis notebooks
src/                ← reusable code (future)
outputs/            ← results, charts, tables

## Data

Raw CRSP data is NOT included in this repository.

Download the dataset from the shared Google Drive:
https://drive.google.com/drive/folders/1hFJtHIXBGrMZ0g8QNeGDalM_vkrO_HpF?usp=sharing 

After downloading, place the file in:

data/raw/crsp_monthly_raw.csv

## Setup

1. Clone the repository
2. Create and activate a virtual environment
3. Install dependencies:

pip install -r requirements.txt

## How to Run

1. Open the notebook:
notebooks/01_clean_crsp_momentum.ipynb

2. Run all cells to:
- clean CRSP data
- create market equity
- prepare dataset for strategy

## Current Progress

- CRSP monthly data loaded and cleaned
- Market equity calculated
- Data sorted and stored in processed format

## Next Steps

- Construct momentum signal (12-month lookback, skip 1 month)
- Form decile portfolios
- Backtest long-short strategy
- Evaluate performance (returns, Sharpe ratio)

## Notes

- Raw data is large and stored externally (Google Drive)
- Only cleaned data and code are tracked in GitHub
