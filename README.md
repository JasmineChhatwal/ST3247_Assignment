# ST3247_Assignment

This repository contains the implementation and analysis of Approximate Bayesian Computation (ABC) methods applied to a network-based SIR model with rewiring.

---

## Overview

The project investigates parameter inference for a stochastic SIR network model using:

- ABC Rejection
- Regression Adjustment
- Sequential Monte Carlo ABC (SMC-ABC)
- Bayesian Optimisation for Likelihood-Free Inference (BOLFI)

The focus is on understanding **parameter identifiability**, **effect of summary statistics**, and **posterior refinement**.

---

## Repository Structure

This repository contains 3 data files and a single Python script 'main.py':

### Data Files
Includes:
1. infection_timeseries.csv
2. rewiring_timeseries.csv
3. final_degree_histograms.csv
   
### `main.py`
Includes:
1. **Simulator**
   - Network-based SIR model with rewiring
   - Optimised using Numba

2. **ABC Rejection**
   - Run 1: Initial summary statistics
   - Run 2: Reduced summary statistics
   - Posterior analysis (correlation plots, corner plots)

3. **Advanced Methods**
   - Regression Adjustment
   - SMC-ABC (adaptive tolerance + perturbation)
   - BOLFI

---

## Requirements

Install required packages before running:

```bash
! pip install numpy matplotlib seaborn numba joblib scikit-learn scikit-optimize

```
