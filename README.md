# MICE-Foreign-Demand-TimeSeries-Stat-Analysis

This repository contains the code and methodology for analyzing the short-term dynamics of foreign MICE (Meetings, Incentives, Conventions, and Exhibitions) demand using time-series analysis. The analysis is based on the Vector Autoregression (VAR) model, as discussed in the paper "MICE 외국인 수요의 단기적 동태 분석에 관한 시계열 분석 –VAR 모델을 중심으로" by 추민수, **김병민**, 윤유식, presented at the The 98th TOSOK International Tourism Conference.

## Introduction
The MICE industry is a high-value sector with a significant impact on the tourism and related industries. However, there has been limited empirical analysis of the short-term dynamics of foreign MICE demand, particularly in relation to economic factors such as exchange rates and international oil prices. This research uses quarterly time-series data from 2009 to 2019 to explore these dynamics.

The primary aim of the study is to evaluate the short-term impact of economic indicators (e.g., international oil prices, exchange rates) on foreign MICE demand. The Vector Autoregression (VAR) model is used for this analysis, focusing on the relationships between these variables and MICE demand.

## Methods

### Data Description and Data Source
- **Time Period:** Quarterly data from Q1 2009 to Q4 2019.
- **International Oil Prices**: The data for international oil prices is based on Dubai crude oil, which accounts for 80% of Korea's oil imports. The quarterly average values of international oil prices from the Korea National Oil Corporation (KNOC) were used, and the natural logarithm was applied to the values.
- **Exchange Rates**: Due to the difficulty in tracking exchange rates for all countries, the exchange rate data was sourced from the Bank of Korea’s Economic Statistics System, using the exchange rate against the US Dollar. The natural logarithm of the exchange rate was then computed.
- **Foreign Tourist Demand**: Data for foreign tourist demand was obtained from the Korea Tourism Organization’s Korea Tourism Data Lab.
- **Foreign MICE Tourist Demand**: The data for foreign MICE tourist demand was derived from the MICE Industry Statistics and Research reports published by the Korea Tourism Organization, covering the period from 2009 to 2022.

### Statistical Tests and Models Used
1. **ADF (Augmented Dickey-Fuller) Test**: To check for stationarity in the time-series data.
2. **Johansen Cointegration Test**: To determine the long-term relationships between the variables.
3. **Granger Causality Test**: To examine the causal relationships between the variables.
4. **VAR Model**: To model the dynamic interaction between the variables.
5. **Impulse Response Function (IRF)**: To analyze the impact of shocks to one variable on others over time.
6. **Forecast Error Variance Decomposition (FEVD)**: To examine how much of the variability in each variable can be explained by others.
