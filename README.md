# VPIN
Volume Synchronized Probability of Informed Trading

## Introduction
-  The VPIN method intends to measure the probability of market informed transaction.
-  Although VPIN method is viewed for the HFT environment. But the result suggests that certain VPIN model with Linear Regression provides proxies for adverse selection risk 
- 주식시장에서의 매수, 매도는 50:50으로 이루어진다는 가정하에 거래량의 불균형을 계산하는 방법입니다.
- 보고자 하는 주식 종목의 일일 평균 거래량을 잘 파악해서 버켓의 크기와 VPIN 계산하기 위한 버캣개수 개수를 잘 설정 해줘야합니다.

## Info
- Version - Written in Python 3.7.3
- Keywords
  - VPIN
  - Market micro structure
  
## Prerequisite
- pandas
- numpy 
- matplotlib.pyplot
- time
- train_test_split
- LinearRegression
- 
## Correspondence
Please do not hesitate to submit an issue or contact via ichuzupikachu@gmail.com.

## Usage
dataset
- kakaostock.csv
- Sampling time: 2021-March-17
- Data sample in time period between 1000 and 1400.

## Methodology
- For transactions in the sampling date, the entile volume is divided into 1000 buckets.

- Filling Procedure: Filling of bucket starts when transaction starts. When volume of transaction exceeds the upper bound, calculate vol_bucket, which indicates the rest of transaction amount Loop of aforementioned process generate a series of baskets.

## Sample Output
<img width="901" alt="스크린샷 2021-04-11 오후 9 13 13" src="https://user-images.githubusercontent.com/42399580/114303916-69fbfe80-9b0b-11eb-9045-138efcd0de1d.png">
