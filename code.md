---
layout: single
title: "Computer codes"
permalink: /code/
author_profile: true
classes: wide
---

This page collects software packages and replication code for my research, written in R and Rcpp. The replication packages are self-contained and reproduce the main results of the corresponding paper on simulated data. Note that these models are fairly complex and some knowledge of Bayesian econometrics / statistics is needed to understand the effect of priors. I do not offer any support for these codes. Although I try to keep them error-free, I can’t guarantee this — if you find an error, please contact me.

## R packages

- **BGVAR** — R toolbox for fast and easy estimation of Bayesian GVAR models. Includes several priors, stochastic volatility, and functions for forecasting and structural analysis. [CRAN](https://cran.r-project.org/package=BGVAR) (with a detailed vignette).

## Replication code

- **BART-based VARs** — R code for estimating various BART-based VAR versions (BART, mixBART, flexBART, fullBART) with factor stochastic volatility, as proposed in Clark, Huber, Koop, Marcellino and Pfarrhofer (2023, *International Economic Review*). [GitHub](https://github.com/fhuber7/replication-archive/tree/main/mixBART_replication).

- **Factor-augmented BART VARs**, with T. Clark and G. Koop (*Journal of Business & Economic Statistics*, forthcoming; [DOI](https://doi.org/10.1080/07350015.2026.2703238)) — R code for a flexible Bayesian VAR augmented with nonlinear BART-based factors and stochastic volatility, featuring sign-identified structural analysis. Ships the factorBART R package plus precomputed caches so all figures regenerate in seconds. [GitHub](https://github.com/fhuber7/fbart-replication).

- **Bayesian Nonparametric VARs** — R code for Bayesian VARs with Dirichlet-process mixture shocks and optional idiosyncratic stochastic volatility, as in Huber and Koop (2024, *Journal of Applied Econometrics*). [GitHub](https://github.com/fhuber7/replication-archive/tree/main/BNPVAR_replication).

- **Forecasting US Inflation using Bayesian Nonparametric Models** — R code for inflation forecasting with GP-subspace, BART, and UCSV specifications under Dirichlet-process mixture shocks, as in Clark, Huber, Koop and Marcellino (2024, *Annals of Applied Statistics*). [GitHub](https://github.com/fhuber7/replication-archive/tree/main/SubspaceInflation_replication).

- **Gaussian Process VARs**, with N. Hauzenberger, M. Marcellino and N. Petz (*JBES*, forthcoming) — R code for a nonparametric VAR with Gaussian-process conditional means, equation-wise stochastic volatility, and horseshoe-shrunk structural covariance. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/GPVAR_replication).

- **TVP-BART VARs**, with N. Hauzenberger, G. Koop and J. Mitchell (*Annals of Applied Statistics*, forthcoming) — R code for a semiparametric TVP-VAR in which time-varying coefficients and error covariances are driven by Bayesian Additive Regression Trees (BART). [GitHub](https://github.com/fhuber7/replication-archive/tree/main/TVP_BART_replication).

- **Nowcasting in a Pandemic using Non-Parametric Mixed-frequency VARs**, with G. Koop, M. Pfarrhofer, L. Onorante and J. Schreiner (*Journal of Econometrics*, forthcoming). Estimates the mixed-frequency BAVART model and more general BART-based VARs via an SVD-based algorithm with mixture state-equations. [GitHub](https://github.com/mpfarrho/mf-bavart).

- **Investigating Growth-at-Risk Using a Multicountry Non-parametric Quantile Factor Model**, with T. Clark, G. Koop, M. Marcellino and M. Pfarrhofer (*JBES*, 2024). R code implementing the QF-BART model for jointly estimating quantiles of GDP growth across multiple countries. [GitHub](https://github.com/mpfarrho/qf-bart).

- **Adaptive Shrinkage in Bayesian Vector Autoregressive Models**, with M. Feldkircher (*JBES*, 2019). Estimates a VAR with a hierarchical Normal-Gamma shrinkage prior (and alternative priors) on the autoregressive coefficients with stochastic volatility. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/NGVAR_replication).

- **Approximate Bayesian Inference and Forecasting in Huge-dimensional Multi-country VARs**, with M. Feldkircher, G. Koop and M. Pfarrhofer. Implements the Integrated Rotated Gaussian Approximation (IRGA) strategy for very large multi-country VARs combining Horseshoe-prior MCMC with VAMP. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/PVAR_IRGA_replication).

- **Combining Shrinkage and Sparsity in Conjugate Vector Autoregressive Models**, with N. Hauzenberger and L. Onorante (*Journal of Applied Econometrics*, 2020). Conjugate Bayesian VAR with Minnesota dummy-observation priors and SAVS post-processing sparsification. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/SparseVAR_replication).

- **Subspace Shrinkage in Conjugate Bayesian Vector Autoregressions**, with G. Koop (*Journal of Applied Econometrics*, forthcoming). Conjugate matrix-Normal / Inverse-Wishart VAR with a convex combination of a Minnesota prior and a principal-component subspace projection. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/SubspaceVAR_replication).

- **Threshold Cointegration in International Exchange Rates: A Bayesian Approach**, with T. O. Zörner (*International Journal of Forecasting*, 2019). Estimates a three-regime threshold Bayesian vector error correction model (TBVECM). [GitHub](https://github.com/fhuber7/replication-archive/tree/main/TBVECM_replication).

- **Fast and Flexible Bayesian Inference in Time-Varying Parameter Regression Models**, with N. Hauzenberger, G. Koop and L. Onorante (*JBES*, 2021). SVD-based fast sampler for TVP regressions with sparse-mixture g-prior on the coefficients. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/TVPSVD_replication).

- **Should I Stay or Should I Go? A Latent Threshold Approach to Large-scale Mixture Innovation Models**, with G. Kastner and M. Feldkircher (*Journal of Applied Econometrics*, 2019). Latent-threshold TVP-VAR with stochastic volatility; includes the `threshtvp` R package source. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/ThreshTVP_replication).

- **Inducing Sparsity and Shrinkage in Time-Varying Parameter Models**, with G. Koop and L. Onorante (*JBES*, 2021). TVP-VAR with global-local shrinkage priors (Horseshoe, LASSO, Normal-Gamma, SSVS, Dirichlet-Laplace) and SAVS post-processing for exact sparsification of time-varying coefficients. [GitHub](https://github.com/fhuber7/replication-archive/tree/main/SAVS_TVP_VARs_replication).
