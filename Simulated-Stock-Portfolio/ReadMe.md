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
