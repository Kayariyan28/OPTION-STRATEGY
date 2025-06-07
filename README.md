# Option Strategy Dataset and Notebook

This repository contains a sample option chain data set and a Jupyter notebook that demonstrates how to generate option trading strategies using the Black-Scholes model. The project was originally built in Google Colab, and a PDF export of the notebook output is also provided.

## Repository Contents

- `2024-12-10_option_chain_120days_student6.csv` – Historical option chain with 2,300+ rows. Columns include option type, strike, expiration date, time to expiry, bid, ask, volume, open interest, and calculated Greeks.
- `Untitled32.ipynb` – Jupyter notebook used to clean the dataset, compute Black‑Scholes prices and greeks, and generate candidate strategies (bull call spreads, bear put spreads and short iron condors).
- `Untitled32.ipynb - Colab.pdf` – Static PDF version of the notebook’s output for reference.

## Getting Started

1. Install Python 3 with `pip`.
2. Install the required libraries:
   ```bash
   pip install pandas numpy scipy plotly
   ```
3. Launch Jupyter and open `Untitled32.ipynb`:
   ```bash
   jupyter notebook
   ```
4. Run the notebook cells in order. It loads the CSV, removes illiquid contracts, calculates Black‑Scholes values, and suggests option strategies.

The notebook can also be run on Google Colab using the badge at the top of the first cell.

## File Overview

| File | Description |
|------|-------------|
| `2024-12-10_option_chain_120days_student6.csv` | Option chain example containing call and put data for multiple expiries. |
| `Untitled32.ipynb` | Analysis notebook that calculates greeks, generates heatmaps and finds spreads/condors. |
| `Untitled32.ipynb - Colab.pdf` | PDF version of the executed notebook. |

## Notes

The data set is provided for educational purposes only. Prices, greeks and spreads are computed using simple Black‑Scholes assumptions and do not constitute trading advice.

