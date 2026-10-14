ICE TTF Gas Options Analytics

Python/SQL quantitative research project for ICE TTF natural gas options, focusing on trade reconstruction, implied volatility extraction, gamma exposure, and multi-leg transaction analysis.

Overview

Developed a data-driven analytics pipeline to reconstruct option trades and associated futures hedges, infer traded implied volatility from market prices, and analyse exposure and positioning across strikes, expiries, and intraday intervals.

Key Features

1. Trade and Hedge Reconstruction

* Processed 12,736 option contracts and 5.85M historical observations using SQL and Python.
* Matched option transactions with associated futures hedges and structured trade-level datasets for downstream analytics.

2. Implied Volatility Modelling

* Numerically inverted the Black-76 pricing model to recover implied volatility from traded option prices.
* Designed 5-minute intraday volatility comparisons against desk marks to analyse deviations in market-implied volatility across strikes and maturities.

3. Gamma Exposure Analysis

* Calculated option gamma exposure across strikes and maturities to identify concentrations of convexity exposure.
* Analysed the distribution of exposure across the options surface to assess sensitivity to underlying futures price movements.

4. Multi-Leg Trade Classification

* Classified multi-leg ICE transactions to identify complex option structures and aggregate related trading activity.
* Analysed strike-, maturity-, and structure-level concentrations to investigate market positioning.

Methodology

1. Data processing: SQL-based extraction, filtering, and joining of historical options and futures observations.
2. Trade reconstruction: Matching option executions with associated futures hedges and normalising trade-level records.
3. Volatility calibration: Numerical inversion of Black-76 using observed option prices and relevant contract parameters.
4. Exposure analytics: Gamma calculation and aggregation across strikes and maturities.
5. Intraday analysis: Five-minute alignment of trade-implied volatility with desk marks and classification of multi-leg transactions for positioning analysis.

Technology Stack

Python · SQL · Black-76 · Numerical Optimisation · Derivatives Analytics · Time-Series Analysis
