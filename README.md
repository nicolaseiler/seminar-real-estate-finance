# Same Shock, Different City

**Drivers of House Prices: The Role of Location, Land, and Construction Costs**

Research Seminar in Real Estate Finance — University of St. Gallen (HSG), Spring 2026  
Group 4 · Prof. Dr. Roland Füss

## Research Question

*What macroeconomic and structural factors drive U.S. metro-level house prices, and does local supply restrictiveness — as measured by land use regulation — amplify their impact?*

## Methodology

We estimate a two-way fixed effects panel model (metro + time FE) on 187 U.S. metropolitan areas from January 2001 to January 2026. Because the Wharton Residential Land Use Regulatory Index (WRLURI) is time-invariant and absorbed by metro fixed effects, identification comes from interacting WRLURI with time-varying macroeconomic variables (mortgage rates, construction costs, unemployment). All regressors are lagged six months. Standard errors are clustered at the metro level.

**Three empirical layers:**
1. Cross-sectional OLS — regulation and average house price growth
2. Panel two-way FE with interaction terms — differential cyclical sensitivity
3. Pre/post-2020 structural break analysis

## Data Sources

| Variable | Source |
|---|---|
| House prices (ZHVI) | [Zillow Research](https://www.zillow.com/research/data/) |
| WRLURI 2006 & 2018 | Gyourko, Saiz & Summers (2008); Gyourko, Hartley & Krimmel (2021) via [Duranton & Puga replication package](https://diegopuga.org/data/urbangrowth/) |
| Saiz geographic unavailability & elasticity | Saiz (2010) |
| Mortgage rate (MORTGAGE30US) | [FRED](https://fred.stlouisfed.org/) |
| Unemployment rate (UNRATE) | [FRED](https://fred.stlouisfed.org/) |
| Construction cost index | BLS via [FRED](https://fred.stlouisfed.org/) |

The panel dataset is not included in this repository due to size constraints. It can be fully reconstructed using the code and sources listed above.

## Repository Contents

| File | Description |
|---|---|
| `Code_Final.ipynb` | Jupyter notebook with full empirical analysis |
| `Empirical_analysis_code_final.py` | Python script version of the analysis |

## Key Packages

`pandas` · `linearmodels` · `statsmodels` · `matplotlib` · `scipy`

## Authors

Nicola Seiler · Leonardo Accardi · Simone Caputo
