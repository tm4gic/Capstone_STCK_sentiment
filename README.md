# Stock Sentiment Capstone Project
In this project, NLP is used to attempt to predict Tesla Stock movement based on sentiment from articles about the stock from the New York Times. 

## Overview
We have all heard at some point about the magic of the Stock market, transforming investments into fortunes for those that dare take the risk. Many investors and institutions study, observe and gather data on stock to gain any edge that they can in order to provide a strong and reliable stock trading strategy. Similar to a casino, gaining any edge over 50% could lead to great rewards. 

Lately, given the volatility of the stock market, especially during the COVID-19, many oppurtunities have presented themselves in the market. The stock market experienced an influx from the stimulus packages as well a influx of retail traders. According to a study, more than 10MM new brokerage accounts were opened in 2020 - more than ever in a year. We have seen stocks such as GameStop, Moderna, Wayfair, Peloton and many more gain enormous amounts of market cap. For this project, I decided to pick one of people's favorites and as well as a large winner from Covid-19- Tesla. Tesla has increased its price from its Covid low of around $72 to its current price of $753 as of Tuesday, September 9 close.

Tesla remains one of retail traders favorites (currently sits as the second most traded stock on Robinhood, a favorite trading platform for retail traders.) Because of the gap of information between large institutional traders and the retail traders. I have formed a hypothesis that the average retail trader would be more likely to react to both positive and negative sentiments regarding the stock itself.

To try and prove this, this project attemps to use NLP's Sentiment analysis tools to solve a classification problem. Given an article released about Tesla, my classifier model will attempt to predict wether the sotck would close up or below the open price for that day. 

## Data
Articles URLs were obtained from the New York Times API and then paired with beautiful soup to scrape the body of the articles. 
