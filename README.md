# DFGR-Longevity-Derivatives-Project
This project explores the pricing of longevity-linked derivatives using continuous-time mortality models calibrated on Portuguese mortality data.

We calibrate both the **Cox-Ingersoll-Ross (CIR)** and **CIR-Jump (CIR-J)** models to model the force of mortality for a cohort aged 65 from 1990 to 2022 — capturing long-term dynamics including the impact of COVID-19.

## Contents:

- **Mortality Model Calibration**
  - CIR and CIR-J parameter estimation
  - Survival curve comparison
- **Risk-Neutral Simulation**
  - Monte Carlo estimation of survival under \(\mathbb{Q}\)
- **Derivative Pricing**
  - Longevity swaps (floating vs fixed)
  - Caplets pricing via Monte Carlo and Fourier-Laplace transform
- **Fourier-Based Analytics**
  - Laplace transform implementation
  - Limitations of Fourier inversion for caplets

## Files

- `DFGR_Project_Pricing_Longevity_Derivatives_Portugal.ipynb` — the full Colab notebook (cleaned, commented)
- `portugal_life_table.txt` — mortality dataset (HMD 2022)
- `DFGR.Project-2.pdf` — final report with results & plots

## Key Insights

- CIR-J improves fitting over CIR, even when jumps are small
- Monte Carlo pricing agrees well with Fourier for forwards and swaps
- Fourier pricing of caplets is challenging but informative

## Acknowledgments

- Human Mortality Database (HMD)
- Bravo & Nunes (2021) for Laplace transform formulation
- Final-year project in **Financial Derivatives & Risk Management**

