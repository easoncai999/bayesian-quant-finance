# Bayesian Asset Pricing: A Bayesian Statistical Modeling Approach

Welcome to the repository for **Bayesian Statistical Modeling: Quantitative Asset Pricing Through a Bayesian Approach**. This project proposes a novel framework to enhance asset price predictions by integrating macroeconomic fundamentals with technical trading signals using Bayesian methods.

---

## Overview

Financial markets are complex and driven by both long-term macroeconomic factors (like GDP growth and interest rates) and short-term trading signals (such as the Relative Strength Index, RSI). Traditional models, including CAPM or Fama-French, typically focus on one of these perspectives. Our project bridges this gap by developing a Bayesian model that unifies these different information sources for improved asset pricing and risk assessment.

---

## Project Motivation & Background

- **Challenge:**  
  Most existing asset pricing models treat macroeconomic data and technical indicators separately, potentially missing crucial interactions that occur during market bubbles or crashes.
  
- **Our Solution:**  
  By fusing qualitative insights (e.g., sentiment analysis and economic trends) with quantitative signals (e.g., RSI, historical returns) into a Bayesian framework, this model aims to provide:
  - A more precise prediction of asset returns.
  - Robust quantification of uncertainty.
  - Enhanced decision-making support for both short-term traders and long-term investors.

- **Impact:**  
  With potential applications across finance, insurance, economic forecasting, and public policy, this approach not only improves market efficiency but also fosters a deeper understanding of asset pricing dynamics.

---

## Methodology

The project development is structured in three main phases:

1. **Data Acquisition and Preprocessing:**
   - **Data Sources:**  
     - **Alpha Vantage API:** Provides both real-time and historical financial data, including technical indicators and macroeconomic variables.
     - **Economic Indicators:** Supplementary macroeconomic data (e.g., GDP growth, interest rates) help construct informative priors.
   - **Data Cleaning & Alignment:**  
     - Historical price data is cleaned, and key metrics like the RSI are computed.
     - Macroeconomic and sentiment data are aggregated to form a coherent dataset.

2. **Bayesian Model Development:**
   - **Prior Distribution:**  
     - Derived by blending macroeconomic indicators with qualitative insights (e.g., news sentiment).
   - **Likelihood Function:**  
     - Based on historical price movements adjusted using technical indicators like the RSI.
   - **Posterior Inference:**  
     - Combining the prior and likelihood, the Bayesian update yields a posterior distribution for expected asset returns.
   - **Tools:**  
     - Python libraries such as `PyMC` or `Stan` are employed for parameter inference via Markov Chain Monte Carlo (MCMC).

3. **Evaluation and Validation:**
   - **Model Testing:**  
     - Out-of-sample datasets and cross-validation techniques are used to rigorously test the model.
   - **Benchmarking:**  
     - Comparisons with traditional non-Bayesian methods (e.g., CAPM, OLS regression) help validate the effectiveness of our approach.
   - **Robustness Checks:**  
     - Regularization techniques (L1/L2) and sensitivity analyses ensure the model's stability under varying market conditions.

---

## Preliminary Findings

The initial prototype, applied to Apple Inc. stock data, has demonstrated promising capabilities:

- **Prior Distribution:**  
  Combines macroeconomic growth rates with sentiment scores to form an informative starting point.
- **Likelihood Distribution:**  
  Uses historical price movements and RSI adjustments to capture market dynamics.
- **Posterior Distribution:**  
  Effectively updates beliefs based on new market data, yielding robust predictions of expected returns.

The success with Apple data sets the stage for broader applications and further refinement.

---

## References

1. [Alpha Vantage API Documentation](https://www.alphavantage.co/documentation/#)
2. [Alpha Vantage Relative Strength Index (RSI)](https://www.alphavantage.co/relative_strength_index_rsi/)
3. [FRED API Terms of Use](https://fred.stlouisfed.org/docs/api/terms_of_use.html)
4. [Fighting Overfitting with L1 or L2 Regularization - Neptune Blog](https://neptune.ai/blog/fighting-overfitting-with-l1-or-l2-regularization)

---

## License

This project is licensed under the GNU general public license v3.0. License – see the [LICENSE](LICENSE) file for details.

---

## Contact

For questions or feedback, please contact me at [xuchen.cai.th@dartmouth.edu].
