# Bayesian Analysis of Air Pollution: Causal Impact of Area C in Milan

## Overview
This project was developed as part of a university course in Bayesian Statistics.  
It investigates the causal impact of the introduction of Area C (a traffic restriction policy in Milan) on air pollution levels, using Bayesian time series models and spatial analysis.

## Objective
The goal of the project is to evaluate whether the introduction of Area C led to a reduction in air pollution (PM10 and PM2.5), and to understand how this effect varies across space.

## Dataset
The analysis combines multiple data sources:
- Air pollution data (PM10, PM2.5) from ARPA monitoring stations (2010–2017)
- Weather data (temperature, rain, wind) from Open-Meteo

Data were aggregated at weekly level and processed to ensure consistency and completeness.

## Methods
The project applies advanced Bayesian and statistical techniques, including:

- Bayesian Structural Time Series (BSTS) for causal inference
- Causal Impact framework for counterfactual analysis
- Custom Bayesian modeling in Stan
- Hierarchical spatio-temporal modeling
- Autoregressive processes (AR)
- Spatial Gaussian processes with distance-based covariance
- MCMC sampling and posterior inference
- Conformal-style uncertainty interpretation through credible intervals

## Key Results
- The introduction of Area C shows evidence of a reduction in PM10 levels within the restricted area.
- The estimated effect is sensitive to modeling assumptions, particularly prior specification.
- Spatial analysis reveals strong heterogeneity across Lombardy, with localized effects and possible spillover dynamics.
- Air pollution dynamics are driven by a combination of temporal persistence, spatial structure, and policy interventions.

## Tools
- R
- Stan
- CausalImpact package

## Project Structure
- `Final_report_bayesian.pdf`: full report with methodology and results
- `causal_impact.R`,`causal_impact_stan_model.stan`,`causal_impact_with_stan.R`,`exploratory_analysis.R`,`spatial_stan_model.R`: implementation of models and data analysis in R and using Stan

## Authors
- Ester Maiocchi, Miguel Gutierrez, Alessandra Luca, Marianna Mazza, Amedeo Sottanella, Federico Travaglini
