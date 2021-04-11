# VPIN
Volume Synchronized Probability of Informed Trading
##Introduction
-  The VPIN method intends to measure the probability of market informed transaction; as a predictive sign of the market liquidity risk.

## Basic info
- Version - Written in Python 3.7.3
- Keywords
  - VPIN
  - Random control
  - Market micro-structure
  
## Prerequisite
- pandas
- numpy 
- matplotlib.pyplot
- time
- train_test_split
- LinearRegression
- SGDRegressor

## Usage
dataset
- sise3.csv
- Sampling time: 2021-March-17

## Methodology
- For transactions in the sampling date, the entile volume is divided into 1000 buckets.

- Filling Procedure: Filling of bucket starts when transaction starts. When volume of transaction exceeds the upper bound, calculate vol_bucket, which indicates the rest of transaction amount Loop of aforementioned process generate a series of baskets.

## Sample Output
