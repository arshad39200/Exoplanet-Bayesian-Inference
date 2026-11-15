# Bayesian Model Selection in Exoplanet Science

## Overview
This repository contains a complete Bayesian pipeline to analyze radial velocity (RV) data and determine the number of planets orbiting a star. The project progresses from synthetic mock data to real-world datasets (51 Pegasi b and the multi-planet system GJ 876).

## Key Methodologies
- **Keplerian RV Modeling:** Using the `radvel` package.
- **Maximum Likelihood Estimation (MLE):** Optimizing model fits using Differential Evolution.
- **Model Comparison:** Utilizing AIC, BIC, and Bayesian Evidence.
- **Nested Sampling:** Using `dynesty` to calculate Bayesian Evidence and Bayes Factors.
- **Savage-Dickey Density Ratio:** A shortcut to calculate Bayes factors for nested models directly from posterior samples.

## How to Run
1. Ensure the required data files (`.tbl`, `.csv`) are in the same directory as the notebook.
2. Install the dependencies:
   ```bash
   pip install numpy pandas matplotlib scipy radvel dynesty corner astroquery tqdm windows-curses
