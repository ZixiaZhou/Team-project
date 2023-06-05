---
editor_options: 
  markdown: 
    wrap: 72
---

# Team-project

## 1. Introduction

This repository is working for reproducing the main finding of paper "A
Vector Error Correction Model (VECM) Approach in Explaining the
Relationship Between Interest Rate and Inflation Towards Exchange Rate
Volatility in Malaysia". The paper can be found in the repository named
"RR_paper".

The paper discusses the importance of exchange rates in trade and the
challenges of controlling them. It introduces a study that examines the
factors influencing exchange rate volatility in Malaysia, focusing on
the relationship between exchange rates, interest rates, and inflation
rates.

## 2. Data

The monthly exchange rate in Malaysia (RM/USD) is represented by EXC,
while IR represents the monthly interest rate and INF represents the
inflation rate with the time trend. The data used in the analysis
consists of 132 monthly observations from 1999 to 2009. It was obtained
from the Bank Negara Malaysia and Trading Economics. All the data can be
found in RR_data.xls in the repository. \## 3.Methodology and Result
Stationarity Test: We use ADF and PP test to examine the stationarity.
It shows both EXC and INF integrated \~ I(1), and IR integrated \~I(0).
In order to conduct the Vector Error Correction Model, we should
determine the lags of the order and test the cointegrating of the
variables. By using VARselect function, we obtained that we should
include 2 lags in our model. The Johansen test is a statistical
procedure utilized to assess whether a group of time series variables
exhibit cointegration. The results is equal to 1, which is greater than
zero but less than the number of variables, it indicates that the series
are cointegrated. Therefore, we can proceed with estimating the VECM.
VECM presents IR has positive relationship with EXC and INF has negative
relationship which is same as the finding of the paper. The equation is
as below: EXC = 0.179788IR - 0.038686INF The Granger causality test is a
statistical test used to determine whether one time series variable can
predict another time series variable. We can reach the same conclusion
as the article, which is that the relationship between inflation rates
and exchange rate fluctuations is unidirectional. Interest rates and
exchange rates also exhibit a unidirectional relationship. More specific
codes and discussions could be found in "RR_proejct1.RMD".

## Note: AI support Chatgpt gives us some brief concepts of methodology and part of the interpretations.
