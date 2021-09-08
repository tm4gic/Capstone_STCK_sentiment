# Stock Sentiment Capstone Project

![image](https://user-images.githubusercontent.com/83128139/132532985-3c91c648-c9e5-401d-a895-0d66ea83b990.png)

In this project, NLP is used to attempt to predict Tesla Stock movement based on sentiment from articles about the stock from the New York Times. 

## Overview
We have all heard at some point about the magic of the Stock market, transforming investments into fortunes for those that dare take the risk. Many investors and institutions study, observe and gather data on stock to gain any edge that they can in order to provide a strong and reliable stock trading strategy. Similar to a casino, gaining any edge over 50% could lead to great rewards. 

Lately, given the volatility of the stock market, especially during the COVID-19, many oppurtunities have presented themselves in the market. The stock market experienced an influx from the stimulus packages as well a influx of retail traders. According to a study, more than 10MM new brokerage accounts were opened in 2020 - more than ever in a year. We have seen stocks such as GameStop, Moderna, Wayfair, Peloton and many more gain enormous amounts of market cap. For this project, I decided to pick one of people's favorites and as well as a large winner from Covid-19- Tesla. Tesla has increased its price from its Covid low of around $72 to its current price of $753 as of Tuesday, September 9 close.

Tesla remains one of retail traders favorites (currently sits as the second most traded stock on Robinhood, a favorite trading platform for retail traders.) Because of the gap of information between large institutional traders and the retail traders. I have formed a hypothesis that the average retail trader would be more likely to react to both positive and negative sentiments regarding the stock itself.

To try and prove this, this project attemps to use NLP's Sentiment analysis tools to solve a classification problem. Given an article released about Tesla, my classifier model will attempt to predict wether the sotck would close up or below the open price for that day. 

## Data

### API
Articles URLs were obtained from the New York Times API and then paired with beautiful soup to scrape the body of the articles. 
https://developer.nytimes.com/docs/articlesearch-product/1/overview

The Article Search API of The New York Time was queried for articles containing the term 'tesla' 2010 (Tesla IPO year) and 2021. The search term returned a total of 3,220 article hits.

The API returned the following information for each article:
* URL
* Snippet (Headline)
* Publication Date
* Identifier
* Lead Paragraph

### Web Scraping

The body of artciles were obtained from webscraping using beautiful soup.

### Data Processing

insert EDA graphs and analysis

## Natural Language Processing
Natural Language Processing (NLP) was applied to each article snippet (headline), lead paragraph and article body. Two sentiment analysis toolsets were applied to the article texts.

Two NLP tools were used in this analysis: 

### TextBlob Sentiment Analysis https://textblob.readthedocs.io/en/dev/

TextBlob Sentiment Analysis tool was applied to the snippet (headline), lead paragraph and article body of each article. Form there, Polarity and subjectivity scores were recorded for each article.

* Polarity: a float which lies in the range of [-1,1] where 1 means positive statement and -1 means a negative statement.
* Subjectivity : a float between [0,1] where 0 refer to factuaql information and 1 indicates that it is total public opinion


