# Simulated Stock Portfolio: Enhancing Investment Success through Fundamental Analysis and Portfolio Optimization

## Abstract:

This report aims to provide a comprehensive analysis of a simulated stock portfolio, highlighting the systematic approach of fundamental analysis, stock selection, and portfolio optimization. By leveraging financial statements, industry trends, and key financial metrics, investors identify stocks with growth potential. The selected stocks are then held for a designated period, to maximize returns.

## Objective:

**The objective of this report is to present a comprehensive analysis of a simulated stock portfolio, focusing on the process of selecting stocks at the end of 2022 or the beginning of 2023.** By adopting a "buy and hold" strategy for one year, we aim to evaluate the performance and returns of the chosen stocks at the end of 2023.

## Note: 
**It is crucial to note that the outcomes and conclusions presented in this report are based on simulated data and do not constitute financial advice.**

## 1. Stock Data Collection 

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


## 2. Fundamental Analysis

In our analysis, we collected financial statements and ratios for each selected company, creating a data frame with columns including Symbol, Release Date, Total Revenue, Market Price, Net Income, Total Stockholder Equity, EPS, P/E Ratio, ROE, and ROCE. We focused on key financial metrics such as the P/E ratio, ROE, and ROCE.

<img src='./image/dfHead.png' width='800'>


### 2.1 Selection Criteria on Fundamental Analysis: 

- **P/E ratio** provides insights into the valuation of a stock, with a higher ratio indicating a higher price relative to earnings. A lower P/E ratio may indicate an attractive investment opportunity, assuming other fundamentals are strong.


- **ROE** measures a company's profitability conversion capability, with a higher ROE indicating better profitability. 


- **ROCE** reflects the company's ability to generate returns for both equity and debt holders. If the ROCE is higher than the ROE, it suggests efficient utilization of debt to reduce the cost of capital.


Filtering stocks based on criteria such as ROE > 20%, P/E < 40%, and a similarity between ROCE and ROE, we aimed to identify stocks with favorable fundamentals for potential inclusion in the portfolio.


## 2.2 Comparison of P/E, ROE, and ROCE for each selected Stock

<img src='./image/SelectedStockComparsion.png' width='800'>

## Stock Selection

1. ON Semiconductor Corporation (ON):
   - Sector(s): Technology
   - Industry: Semiconductors
   - Description: ON Semiconductor is an American semiconductor supplier, formerly the semiconductor component division of Motorola Group. It has an industry-leading position in the fields of automotive, industrial and cloud power semiconductor components.
    
     
2. Arista Networks, Inc. (ANET):
   - Sector(s): Technology
   - Industry: Computer Hardware
   - Description: Arista Networks was founded to pioneer and deliver software-driven cloud networking solutions for large data center storage and computing environments.

   
3. Super Micro Computer, Inc. (SMCI):
   - Sector(s): Technology
   - Industry: Computer Hardware
   - Description: Supermicro Computer Co., Ltd., mainly engaged in computer host solutions.

     
4. Alphabet Inc. (GOOG):
   - Sector(s): Communication Services
   - Industry: Internet Content & Information
   - Description: Alphabet, Inc is a holding company engaged in the business of acquiring and operating different companies. It operates through its Google and Other Bets divisions. The Google segment includes its major Internet products.

5. Netflix, Inc. (NFLX):
    - Sector(s): Communication Services
    - Industry: Entertainment
    - Description: Netflix is ​​an OTT service company that provides online on-demand streaming of videos around the world.

      
6. Adobe Inc. (ADBE):
    - Sector(s): Technology
    - Industry: Software - Infrastructure
    - Description: Adobe is mainly engaged in the development of multimedia production software. In recent years, it has also begun to develop software such as rich Internet applications, marketing applications, and financial analysis applications.

7. Lithia Motors, Inc. (LAD)
    - Sector(s): Consumer Cyclical
    - Industry: Auto & Truck Dealerships
    - Description: Lithia Motors is an American nationwide automotive dealership group headquartered.

8. Mueller Industries, Inc. (MLI)
    - Sector(s): Industrials
    - Industry: Metal Fabrication
    - Description: Mueller Industries, Inc. is an industrial manufacturer that specializes in copper and copper alloy manufacturing while also producing goods made from aluminum, steel, and plastics. 

9. Devon Energy Corporation (DVN)
    - Sector(s): Energy
    - Industry: Oil & Gas E&P
    - Description: Devon's targets focus on reducing the carbon intensity of our operations, minimizing freshwater use, and engaging constructively with our value chain.

10. Texas Pacific Land Corporation (TPL)
    - Sector(s): Energy
    - Industry: Oil & Gas E&P
    - Description: Texas Pacific Land Trust is one of the largest landowners in the State of Texas with approximately 900000 acres of land in West Texas.

11. Exxon Mobil Corporation (XOM):
    - Sector(s): Energy
    - Industry: Oil & Gas Integrated
    - Description: ExxonMobil is one of the world's largest publicly traded international oil and gas companies.

12. Chevron Corporation (CVX): 
    - Sector(s): Energy
    - Industry: Oil & Gas Integrated
    - Description: Chevron Corporation is one of the world's largest multinational energy companies. Its business scope penetrates all aspects of the oil and natural gas industry: exploration, production, refining, marketing, transportation, petrochemicals, power generation, etc.

13. Deckers Outdoor Corporation (DECK):
    - Sector(s): Consumer Cyclical
    - Industry: Footwear & Accessories
    - Description: Deckers Outdoor Corporation, doing business as Deckers Brands, is a footwear designer and distributor based in Goleta, California, United States. 

14. Matador Resources Company (MTDR):
    - Sector(s): Energy
    - Industry: Oil & Gas E&P
    - Description: Matador is an independent energy company engaged in the exploration, development, production and acquisition of oil and natural gas resources in the US.
   
## 5. Capital Asset Pricing Model

**CAPM**, a widely-used financial model, estimates the expected return on an investment based on its systematic risk, commonly known as beta. In this analysis, we utilized the S&P 500 as a benchmark for our portfolio. The CAPM helped us determine the appropriate required rate of return for our investments.

### 5.1 Normalized Prices for all stocks from 2018 to 2022

<img src='./image/NormalizedPrices.png' width='800'>

### 5.2 Correlation matrix between all stocks

<img src='./image/Coff.png' width='800'>

**Correlation coefficient (r)** quantifies the degree to which the prices of two different stocks or financial assets, move in relation to each other. It is represented by the symbol "r" and can take values between -1 and 1.

Interpretation:

*r > 0*: If one stock goes up, the other tends to go up too. +1 means a perfect match.

*r < 0*: If one stock goes up, the other often goes down. -1 means a perfect opposite match.

*r = 0*: They move independently, no clear connection.

### 5.3 Beta  (β)

**Beta  (β)** is a measure of a stock's or portfolio's sensitivity to market movements. It quantifies the systematic risk of an investment.

Interpretation:

β = 1: the stock tends to move in sync with the market.

β > 1: the stock is more volatile (riskier) than the market.

0 < β < 1: the stock is less volatile (less risky) than the market.

β < 0 (negative): the stock moves inversely to the market.

```
{'ADBE': 1.2758267091281452,
 'ANET': 1.2098311411357998,
 'CVX': 1.0407618439616375,
 'DECK': 1.1468512568533273,
 'DVN': 1.45314887705542,
 'GOOG': 1.1390856199886885,
 'GOOGL': 1.144984613869538,
 'LAD': 1.1088461946826724,
 'MLI': 1.2038564544078376,
 'MTDR': 1.8404605252445647,
 'NFLX': 1.1186574614371128,
 'ON': 1.7326100663937736,
 'SMCI': 1.1633970369366942,
 'TPL': 1.0991219811035702,
 'XOM': 0.9061008361245484}
```

### 5.4 Alpha (α) 

**Alpha (α)** is a measure of the difference between actual return and expected return. (Optional)

Interpretation:

If the actual return is higher than the expected return, then α > 0, which means the portfolio performed better than expected, otherwise it is α < 0.

```
{'ADBE': 0.03071627629715536,
 'ANET': 0.0517591172575335,
 'CVX': 0.030742645632524504,
 'DECK': 0.12178458121271682,
 'DVN': 0.06687200105280273,
 'GOOG': 0.017206934769539085,
 'GOOGL': 0.0159860260959632,
 'LAD': 0.04869279801055145,
 'MLI': 0.038890011167942176,
 'MTDR': 0.12308940151906302,
 'NFLX': 0.03513060327350933,
 'ON': 0.07868448779733836,
 'SMCI': 0.1281382829591363,
 'TPL': 0.14743780394985403,
 'XOM': 0.030165381100497903}
```

### 5.5 Expected Return Based on CAPM

We constructed a portfolio with uniform weighting.

```
Annual Expected Return Based on CAPM for ADBE is 12.095133121357907g%
Annual Expected Return Based on CAPM for ANET is 11.469479829593446g%
Annual Expected Return Based on CAPM for CVX is 9.866663677975696g%
Annual Expected Return Based on CAPM for DECK is 10.872415918864712g%
Annual Expected Return Based on CAPM for DVN is 13.77618840190914g%
Annual Expected Return Based on CAPM for GOOG is 10.798795880204354g%
Annual Expected Return Based on CAPM for GOOGL is 10.854719710423984g%
Annual Expected Return Based on CAPM for LAD is 10.512119114486255g%
Annual Expected Return Based on CAPM for MLI is 11.412838413626778g%
Annual Expected Return Based on CAPM for MTDR is 17.447992660891558g%
Annual Expected Return Based on CAPM for NFLX is 10.605132198971061g%
Annual Expected Return Based on CAPM for ON is 16.425545295848323g%
Annual Expected Return Based on CAPM for SMCI is 11.02927375172964g%
Annual Expected Return Based on CAPM for TPL is 10.419931314295011g%
Annual Expected Return Based on CAPM for XOM is 8.590046090028475g%

Annual Expected Return Based on CAPM for the Portfolio is 11.75%
```

### 5.6 BackTesting from 2023

<img src='./image/UniformPoftfolio.png' width='800'>

We constructed a portfolio with uniform weighting and evaluated its performance. The portfolio's total return was calculated to be 50.95%, indicating the cumulative return achieved throughout the designated holding period.

#### Cumulative Return for all stocks from 2023

<img src='./image/Cumulative Return.png' width='800'>

