# Introduction

Download financial data of the stocks in OMXSPI (390ish stocks listed in Stockholm), store the information in SQL database and rank the companies based on the financial metric EV / EBIT. 

More information about OMXSPI: https://indexes.nasdaqomx.com/Index/Overview/OMXSPI

## EV / EBIT definition

EV := Enterprise Value = Market Cap + Total Debt - Cash  
EBIT := Earnings Before Interest and Taxes  

In the context of quantative value, lower EV / EBIT is better as it indicates cheaper companies. 

## What is quantative value?

Quant value is a set of strategies that are based on buying cheap companies defined as companies with low valuations relative to company fundamentals. 

The strategy is based on the seminal paper  
Fama, Eugene F., and Kenneth R. French. "Common risk factors in the returns on stocks and bonds." Journal of Financial Economics 33.1 (1993): 3-56.

What they did was show that two portfolios with the same exposure to Market Beta had different expected returns (this breaks the Capital Asset Pricing-model) based on their exposure to small stocks and cheap stocks (value stocks).  

This model has since been refined and updated to include exposure to quality stocks and companies with different investment strategies in  
Fama, Eugene F., and Kenneth R. French. "A five-factor asset pricing model." Journal of Financial Economics 116.1 (2015): 1-22.

EV / EBIT has been shown to be the best performing value metric because it takes debt into account. This makes it more informative than something like Price / Earnings or Price / Sales.
Fama / French used Book Value / Market Cap as a value metric but other ones are possible as well and the results are roughly the same.
