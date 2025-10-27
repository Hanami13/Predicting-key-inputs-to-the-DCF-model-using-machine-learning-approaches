# Predicting-key-inputs-to-the-DCF-model-using-machine-learning-approaches
Data-driven corporate valuation model integrating machine learning and Monte Carlo simulation with multi-phase DCF. 

Case study: Adobe Inc.

# Machine Learning–Enhanced Monte Carlo DCF Valuation (Adobe Inc. Case Study)

This project presents a **data-driven corporate valuation framework** that integrates  
traditional financial modeling with modern **machine learning** and **Monte Carlo simulation**.  
It was developed as part of my postgraduate research at the **University of Warsaw** and  
applies the methodology to **Adobe Inc.**  

The model demonstrates how data science can make corporate valuation more transparent,  
robust, and explainable — replacing subjective growth assumptions with data-driven forecasts.

---

## Overview

The framework combines three analytical layers:

1. **Predictive Modeling** – Machine learning algorithms (ElasticNet, Lasso, Decision Tree, XGBoost)  
   predict next-year revenue growth (`rev_growth_t+1`) using firm-level financial data.  

2. **Monte Carlo Simulation** – Uncertainty in key valuation drivers (revenue growth, margins, reinvestment rate, WACC)  
   is modeled with probability distributions to generate a range of possible outcomes.  

3. **Multi-Phase DCF Model** – A dynamic valuation engine computes intrinsic firm value  
   across multiple growth phases using mid-year discounting and reinvestment logic.  

The result is a **probability distribution of firm value**, rather than a single deterministic estimate —  
offering a modern, risk-aware view of corporate worth.

---

## Motivation

Traditional DCF models often depend on subjective inputs.  
This project replaces those assumptions with **empirically trained ML models** that forecast growth  
based on historical data. The integration of **Monte Carlo simulation** provides a realistic view  
of uncertainty — an approach inspired by **Professor Aswath Damodaran’s** teachings.

---

## Methodology Summary

**Inputs (X):**  
Revenue, EBIT, margins, ROIC, CAPEX, and other firm fundamentals.  

**Target (y):**  
Next-year revenue growth (`rev_growth_t+1`).  

**Integration:**  
1. ML forecasts feed into the DCF model;
2. Monte Carlo simulates uncertainty;
3. the output is a **distribution of intrinsic values** with expected value, variance, and confidence intervals.

---

## Technology

- **Python**: NumPy, pandas, scikit-learn, OpenTURNS, Matplotlib  
- **APIs**: Yahoo Finance, Financial Modeling Prep (FMP)  
- **Techniques**: Monte Carlo simulation, lognormal/triangular distributions, multi-phase DCF  
- **Models**: ElasticNet, Lasso, Decision Tree, XGBoost  

---

## Key Contributions

- Introduces a **machine learning–based forecasting layer** to corporate valuation.  
- Connects **statistical learning** with **Monte Carlo DCF modeling** in a reproducible Python pipeline.  
- Produces **probabilistic valuations** aligned with real-world investment uncertainty.  
- Bridges **academic theory** with **practical application** in financial data science.  

---

## Academic Note

The written thesis associated with this work was submitted as part of a postgraduate program at the  
**University of Warsaw**. The university holds archival rights to the submitted document,  
while all source code and analytical content remain © 2025 Jan Pabiszczak.

---

## License

This project is released under the **Apache License 2.0**.  
You are free to use, modify, and distribute the code under its terms, with proper attribution.  

> © 2025 Jan Pabiszczak  
> The author retains full commercial rights to this work.  
> This open-source version is shared for **educational and research purposes**.  
> The author reserves the right to release future versions under different licensing terms.

---

## Contact

For collaboration or licensing inquiries:  
- **pabiszczakjan@gmail.com**

---

- *If you find this project insightful, please consider starring the repository —  
it supports the mission of bridging data science and corporate finance.*
