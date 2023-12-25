# Simulated Stock Portfolio: Enhancing Investment Success through Fundamental Analysis and Portfolio Optimization

## Abstract:

This report aims to provide a comprehensive analysis of a simulated stock portfolio, highlighting the systematic approach of fundamental analysis, stock selection, and portfolio optimization. By leveraging financial statements, industry trends, and key financial metrics, investors identify stocks with growth potential. The selected stocks are then held for a designated period, to maximize returns.

## Objective:

**The objective of this report is to present a comprehensive analysis of a simulated stock portfolio, focusing on the process of selecting stocks at the end of 2022 or the beginning of 2023.** By adopting a "buy and hold" strategy for one year, we aim to evaluate the performance and returns of the chosen stocks at the end of 2023.

## Note: 
**It is crucial to note that the outcomes and conclusions presented in this report are based on simulated data and do not constitute financial advice.**

## Stock Data Collection 

To ensure the integrity and impartiality of our analysis, **we have deliberately limited our stock selection process to recommendations and information available in the news during 2022**. By constraining our choices to this period, we aim to eliminate any potential bias or future factors that may arise from being aware of 2023 news and trends.

```
stocks_list = ['AMD','NVDA','INTC','ON','ANET','SMCI','GOOG','META','AMZN','BABA','NIO','AMC','NFLX','ADBE','TSLA','UBER','PINS','AAPL',
              'LAD','TNL','MLI','HRI','DVN','MRO','QCOM','MU','AGYS','CECO','TPL','NOV','MRC','ELF','ATI','XOM','CVX','CRM',
              'AMD','GOOGL','DECK','HAL','TMUS','WDAY','LULU','MTDR','AMGN','ADM']
```
> Reference:
> 
> 1. https://www.nasdaq.com/articles/10-top-stocks-to-buy-for-2022
>    
> 2. https://finance.yahoo.com/news/12-best-performing-growth-stocks-185041601.html
>    
> 3. ... ...


## Fundamental Analysis

In our analysis, we collected financial statements and ratios for each selected company, creating a data frame with columns including Symbol, Release Date, Total Revenue, Market Price, Net Income, Total Stockholder Equity, EPS, P/E Ratio, ROE, and ROCE. We focused on key financial metrics such as the P/E ratio, ROE, and ROCE.

<img src='./image/dfHead.png' width='800'>

