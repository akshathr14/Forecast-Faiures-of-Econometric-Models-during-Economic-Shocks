\# Econometric Forecast Failures During Economic Shocks



\### Project Objective

This research evaluates the forecasting limitations of statistically significant econometric models during extreme market volatility, specifically focusing on the \*\*2007-08 Global Financial Crisis\*\* and the \*\*2020 COVID-19 Pandemic\*\*.



\### Technical Stack

\* \*\*Language/Environment:\*\* R / RStudio

\* \*\*Model Architecture:\*\* ARIMAX (ARIMA with Exogenous Regressors)

\* \*\*Data Source:\*\* Daily historical values from Yahoo Finance (1998–2020)



\### Methodology \& Rigor

\* \*\*Variable Selection:\*\* Modeled the S\&P 500 index using the Dow Jones Industrial Average (DJIA), Nasdaq Composite, Russell 2000, VIX (CBOE Volatility Index), and 10-year Treasury bond yields.

\* \*\*Statistical Diagnostics:\*\*

&nbsp;   \* \*\*Stationarity:\*\* Verified using \*\*Augmented Dickey-Fuller (ADF)\*\* tests and \*\*ACF/PACF plots\*\*, justifying first-order differencing ($d=1$).

&nbsp;   \* \*\*Heteroskedasticity:\*\* Identified via \*\*Breusch-Pagan\*\* tests and treated using \*\*Log-Log Transformations\*\*.

&nbsp;   \* \*\*Autocorrelation:\*\* Evaluated using the \*\*Durbin-Watson\*\* test.



\### Key Results

The project utilized $ARIMA(1,1,1)$ models to compare forecasting performance:

\* \*\*2007-08 Financial Crisis:\*\* Identified a statistically significant failure in mean predictions (Paired T-test p-value: $5.8 \\times 10^{-7}$).

\* \*\*COVID-19 Pandemic:\*\* Confirmed forecast failure during the February 2020 market crash (T-test p-value: $3.9 \\times 10^{-7}$).

