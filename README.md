# social-media-stock-sentiment
This objective of this project is to develop analytics on stocks using social media and news feeds. The backend is developed using Databricks notebook that is deployed in Azure. Stock posts are accessed from r/wallstreetbets using pushshift.io Reddit API. Stock tickers are captured using Alpaca API. Sentiment analysis was performed on stock news feeds using FINVIZ.com news feeds. VADER (Valence Aware Dictionary and sentiment Reasoner - is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media) and NLTK's SentimentIntensityAnalyzer is used for this analysis. All outputs are stored in Azure SQL database with the timestamps of post date or news reporting date.

Data pipeline is shown below:


![social-data-pipeline](https://user-images.githubusercontent.com/37245809/207219558-90ea6f3a-a258-48d8-bf5b-c28f684b8168.png)

Data visualization is shown below:

![stock_sentiment](https://user-images.githubusercontent.com/37245809/205722603-07150595-5f2a-45ab-87da-e41b34aa9f95.png)

The frontend is developed using R. App is developed in R-shiny and hosted in https://snowflectanalytics.shinyapps.io/socialNet/. Backend is refreshed using Databricks jobs once everyday. 
