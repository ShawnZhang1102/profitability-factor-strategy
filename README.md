# Profitability Factor Strategy

> Class Project · Computational Finance (BU.232.610), Johns Hopkins Carey Business School

Does operating profitability predict stock returns? This project builds long–short portfolios sorted on operating margin and tracks their performance over 2015–2023.

## What It Does

- **Data**: cleans CRSP/Compustat data for U.S. listed firms, 2010–2023.
- **Portfolio formation**: as of December 2014, sorts firms into **robust** (top-quartile operating margin) and **weak** (bottom-quartile) portfolios.
- **Performance tracking**: follows both portfolios from 2015 to 2023 and compares their returns.
- **Drift analysis**: with no rebalancing, tracks how the portfolios evolve — 438 firms changed category, 1,291 disappeared, and 1,325 appeared over the sample.
- **Robustness**: repeats the exercise using 5-year average operating margins.

## Tech Stack

Python · Jupyter Notebook · pandas

## How to Run

```bash
jupyter notebook hw4.ipynb
```

## Files

| File | What it is |
| --- | --- |
| `hw4.ipynb` | The full analysis: data cleaning, portfolio formation, performance tracking, drift analysis |

## Data Note

The CRSP and Compustat extracts (`crsp_2010_to_2023.csv`, `compustat_2010_to_2023(in).csv`) are proprietary WRDS data and are **not included** in this repository. To run the notebook, place your own WRDS extracts with those filenames in the same folder as the notebook.
