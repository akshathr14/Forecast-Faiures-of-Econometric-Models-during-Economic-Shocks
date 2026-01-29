\# Econometric Forecast Failures During Economic Shocks



\### Project Objective

\[cite\_start]This research evaluates the forecasting limitations of statistically significant econometric models during extreme market volatility, specifically focusing on the \*\*2007-08 Global Financial Crisis\*\* and the \*\*2020 COVID-19 Pandemic\*\*\[cite: 25, 57]. \[cite\_start]The study demonstrates how robust models can fail to capture "unknown" variables during economic shock\[cite: 287, 321].



\### Technical Stack

\* \[cite\_start]\*\*Language/Environment:\*\* R / RStudio \[cite: 314]

\* \[cite\_start]\*\*Model Architecture:\*\* ARIMAX (ARIMA with Exogenous Regressors) \[cite: 300, 382, 418]

\* \[cite\_start]\*\*Data Source:\*\* Daily historical values from Yahoo Finance (1998–2020) \[cite: 297, 305]



\### Methodology \& Rigor

\* \[cite\_start]\*\*Variable Selection:\*\* Modeled the S\&P 500 index using the Dow Jones Industrial Average (DJIA), Nasdaq Composite, Russell 2000, VIX (CBOE Volatility Index), and 10-year Treasury bond yields\[cite: 296].

\* \*\*Statistical Diagnostics:\*\*

    \* \[cite\_start]\*\*Stationarity:\*\* Verified using \*\*Augmented Dickey-Fuller (ADF)\*\* tests and \*\*ACF/PACF plots\*\*, justifying first-order differencing ($d=1$)\[cite: 302, 358, 372, 379].

    \* \[cite\_start]\*\*Heteroskedasticity:\*\* Identified via \*\*Breusch-Pagan\*\* tests and treated using \*\*Log-Log Transformations\*\*\[cite: 309, 333, 336].

    \* \[cite\_start]\*\*Autocorrelation:\*\* Evaluated using the \*\*Durbin-Watson\*\* test\[cite: 310, 349].

    \* \[cite\_start]\*\*Multicollinearity:\*\* Assessed via \*\*Variance Inflation Factor (VIF)\*\* analysis\[cite: 311, 342].







\### Key Results

\[cite\_start]The project utilized $ARIMA(1,1,1)$ models to compare forecasting performance between normal economic periods and shock periods\[cite: 379, 381, 418]:

\* \[cite\_start]\*\*2007-08 Financial Crisis:\*\* Identified a statistically significant failure in mean predictions, with a \*\*Paired T-test\*\* yielding a p-value of $5.8 \\times 10^{-7}$\[cite: 414, 415].

\* \[cite\_start]\*\*COVID-19 Pandemic:\*\* Confirmed forecast failure during the February 2020 market crash, with a T-test p-value of $3.9 \\times 10^{-7}$\[cite: 448, 449].



\### Conclusion

\[cite\_start]The results provide empirical evidence that relying solely on historical econometric calibration is insufficient for risk management during unanticipated regime shifts\[cite: 454, 460].

