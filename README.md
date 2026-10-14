ICE TTF Gas Options Analytics

A Python-based quantitative analytics project focused on ICE TTF natural gas options, historical trade analysis, implied volatility reconstruction, gamma exposure, and market positioning.

Overview

This project analyses historical ICE TTF gas-options transactions and associated futures hedges to reconstruct traded implied volatility, compare market activity against desk volatility marks, and quantify options-related exposure across strikes and maturities.

Using SQL and Python, the project processes large-scale historical market data to investigate intraday volatility dynamics, options positioning, and multi-leg transaction structures.

Key Features

1. Trade and Hedge Matching

* Processed 12,736 option contracts and 5.85 million historical observations using SQL and Python.
* Matched option trades with their associated ICE TTF futures hedges.
* Structured historical trade data for downstream volatility and exposure analysis.

2. Implied Volatility Reconstruction

* Inverted the Black-76 option pricing model to recover implied volatility from traded option prices.
* Analysed reconstructed implied volatility across strikes and maturities.
* Designed 5-minute intraday comparisons between trade-implied volatility and desk volatility marks to examine market pricing differences and intraday dynamics.

3. Gamma Exposure Analysis

* Quantified gamma exposure across option strikes and maturities.
* Examined the distribution of options-related exposure across the volatility surface.
* Identified concentrations of gamma exposure to support analysis of potential market sensitivity to movements in underlying futures prices.

4. Multi-Leg Transaction Classification

* Classified multi-leg ICE transactions to identify larger options structures.
* Analysed transaction composition and positioning concentrations across strikes and maturities.
* Developed a framework for examining how individual option trades contribute to broader market positioning.

Methodology

The analytical workflow consists of four main stages:

1. Data extraction and preparation — query historical options, futures, and market observations using SQL.
2. Trade reconstruction — match option transactions with associated futures hedges and organise trades into a consistent analytical dataset.
3. Volatility and exposure modelling — invert Black-76 to recover implied volatility and calculate gamma-related exposure metrics.
4. Intraday and positioning analysis — compare reconstructed volatility with desk marks at five-minute intervals and classify multi-leg transactions to investigate positioning concentrations.
