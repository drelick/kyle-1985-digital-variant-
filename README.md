# Kyle Lambda in Crypto (BTC–USD, Coinbase)

This repository contains an empirical implementation of the Kyle (1985) price impact model using high-frequency cryptocurrency trade data.

## Project Overview

We estimate the reduced-form Kyle regression:

Δm_t = α + Λ Q_t + ε_t

Where:
- m_t = log price
- Q_t = signed order flow (net buy minus sell volume)
- Λ = Kyle's lambda (price impact / inverse market depth)

The project demonstrates:
- Construction of signed order flow from trade-level data
- Estimation of price impact using OLS
- HAC (Newey–West) standard errors for robust inference
- Robustness across time aggregations
- Volatility regime comparison

## Repository Structure (Recommended)

kyle-lambda-crypto/
│
├── notebooks/
│   └── your_notebook.ipynb
│
├── paper/
│   └── your_paper.tex
│
├── figures/
│
├── requirements.txt
└── README.md

## Installation

pip install -r requirements.txt

## Running

Open the notebook in Jupyter or Google Colab and run all cells.

## Notes

This is a reduced-form empirical implementation of the Kyle (1985) framework, not a structural equilibrium estimation.
