---
layout: single
title: "Computer codes"
permalink: /code/
author_profile: true
classes: wide
---

This page contains replication codes for some of my papers, written in R and Rcpp. Most of them are easy to use and allow to replicate the main findings of the corresponding paper. Note that these models are fairly complex and some knowledge of Bayesian econometrics / statistics is needed to understand the effect of priors. I do not offer any support for these codes. Although I try to keep them error-free, I can't guarantee this — if you find an error, please contact me.

> **Note:** some of the codes below rely on an older version of the R package `stochvol` and may be incompatible with the latest version. A workable solution is to install an older version of `stochvol` (2.0.4).

## Packages and replication code

- **BART-based VARs** — R code for estimating various BART-based VAR versions, as proposed in Clark et al. (2023, *IER*).
- **BGVAR** — R toolbox for fast and easy estimation of Bayesian GVAR models. Includes several priors, stochastic volatility, and functions for forecasting and structural analysis. [CRAN](https://cran.r-project.org/package=BGVAR) (with a detailed vignette).
- **Nowcasting in a Pandemic using Non-Parametric Mixed-frequency VARs**, with G. Koop, M. Pfarrhofer, L. Onorante and J. Schreiner (*Journal of Econometrics*, forthcoming). Estimates the mixed-frequency BAVART model and, beyond the paper, more general BART-based VARs via our SVD-based algorithm with mixture state-equations. [GitHub](https://github.com/mpfarrho/mf-bavart).
- **Investigating Growth-at-Risk Using a Multicountry Non-parametric Quantile Factor Model**, with M. Pfarrhofer (*JBES*, 2024). R code implementing the QF-BART model for jointly estimating quantiles of GDP growth across multiple countries using nonparametric Bayesian methods and a common factor structure. [GitHub](https://github.com/mpfarrho/qf-bart).
- **Inducing Sparsity and Shrinkage in Time-Varying Parameter Models**, with G. Koop and L. Onorante (*JBES*). Univariate and multivariate state-space models using the SAVS estimator.
- **Should I stay or should I go? A latent threshold approach to large-scale mixture innovation models**, with G. Kastner and M. Feldkircher (*JAE*, 2019). R package for the TTVP regression model (including a VAR variant) and impulse-response analysis.
- **Adaptive shrinkage in Bayesian vector autoregressive models**, with M. Feldkircher (*JBES*, 2019). Estimates a VAR with a Normal-Gamma prior (and alternative priors) plus impulse responses and forecasts.
- **Threshold cointegration in international exchange rates: a Bayesian approach**, with T. O. Zörner (*IJF*, 2019). Estimates a threshold VECM; includes the original dataset.
- **Spillovers from US monetary policy: Evidence from a time-varying parameter GVAR model**, with J. Crespo Cuaresma, G. Doppelhofer and M. Feldkircher (*JRSS A*, 2019). Inference in a TTVP-GVAR model. *Caution:* high-dimensional — cluster computing recommended.
- **The International Transmission of US Shocks — Evidence from Global Vector Autoregressions**, with M. Feldkircher (*EER*, 2016). Estimates a GVAR with Bayesian shrinkage priors and sign-restricted impulse responses.
