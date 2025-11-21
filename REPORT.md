# Final Project — Interpretable N-BEATS Forecasting

This report accompanies the submitted notebook and code implementation.

## Overview
This project implements an interpretable N-BEATS-style forecaster on a synthetic multivariate time series.
The system includes:
- Data generator with trend, seasonality, and regime shifts
- N-BEATS dense-block model (trend + Fourier seasonal bases)
- LSTM and SARIMA baselines
- Global, per-series, and per-horizon evaluation
- Artifacts for reproducibility (plots, CSV outputs)

## Results Summary
Example run showed:
- N-BEATS MAE ≈ 0.0565, RMSE ≈ 0.0699, MAPE ≈ 4.30%
- Strong improvement over baselines
- Stable per-series performance across all 3 channels
- Per-horizon evaluation shows consistent error across future steps

## Files Included
- `final_project_nbeats.ipynb`: Full executable notebook with all code split into readable cells
- `requirements.txt`: Python dependencies
- `REPORT.md`: This summary document

## How to Run
```
pip install -r requirements.txt
jupyter notebook final_project_nbeats.ipynb
```

## Notes
All experiments are seed-controlled and reproducible.
The model is small, fast, and well-suited for coursework evaluation.

