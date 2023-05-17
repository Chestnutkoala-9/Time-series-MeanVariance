# Time Series Mean Variance Project

This project aims to improve the traditional mean-variance problem by incorporating time series analysis techniques, such as ARMA and GARCH models, into the portfolio optimization process. The project utilizes historical time series data of multiple assets to generate forecasts of mean and volatilities. The estimated votalities and mean are then used to optimize portfolio weights. By leveraging ARMA (Autoregressive Moving Average) and GARCH (Generalized Autoregressive Conditional Heteroskedasticity) models, the project aims to capture the time-dependent patterns and volatility clustering in asset returns, resulting in improved risk-return trade-offs for portfolio allocation.

# Steps:

### 1. Stock Return

Based on the pattern of sample autocorrelation function (ACF) and partial autocorrelation function (PACF), tentative
models can be specified from each stock returns. The estimation results indicate that the best models
are all ARMA(0,1). The significance test for parameters and significance tests for models indicate that the mean model for all
stocks analyzed have significance. Generate forecasts for future asset returns using the trained ARMA models.

### 2. Stock Volatility

The order of GARCH model is determined by the residuals of the ARMA model prediction from my last step. Estimate the volatility of asset returns using the trained GARCH models.

### 3. Prediction of Mean and Variance Values

Models of mean and volatility estimation results of five stocks in the previous stage, is then used to perform one step ahead prediction for the mean and variance values.

### 4. Portfolio Optimization

Perform portfolio optimization by incorporating the forecasts and volatilities to improve the mean-variance problem.

### 5. Evaluation Metrics

Evaluate the performance of the optimized portfolio using appropriate metrics, such as risk-adjusted returns and Sharpe ratio

# Conclusion:


