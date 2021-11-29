# CSA - Cryptocurrency Sentiment Analysis


> Machine Learning Project to analyze cryptocurrencies sentiment on twitter 🦤
> The crypto currency chosen were Bitcoin 💰

## 🗂️ Data Acquisition

### 🦤 Select twitter profiles
Was selected 50 twitter profiles that have influence in the crypto market.

### 🦤 Extraction with Octoparse
The data extracted was tweets, this tweets was collected via octoparse a web data extraction software and the simplified extraction process can be seen below:
![](https://i.imgur.com/U7bfWPY.png)

### 💰 Bitcoin 
The bitcoin price was extracted from this site in a csv file: 
| Features          | Tutorials               |
| ----------------- |:----------------------- |
| Yahoo Finance       | [:link:][Yahoo-Finance] |


[Yahoo-Finance]:  https://finance.yahoo.com/quote/BTC-USD/history?period1=1410825600&period2=1631577600&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true

## 🗄️ Data Organization

### 🦤 Twitter Datasets
Was necessary to clean all the datasets and check with the columns were in the same order. 

![](https://i.imgur.com/aM8DiOj.png)

After that all datasets were grouped.

![](https://i.imgur.com/aj8BEAo.png)

### 💰 Bitcoin Dataset
In the bitcoin dataset, only the Date, Open and Close columns were selected. Futhemore, another column called raise was created, which showed whether the was a positive or negative day in the market, based on the Open and Close balance.

![](https://i.imgur.com/usNIOkM.png)



## 📊 Sentiment analysis of collected tweets
Sentiment analysis was developed via NLP and an optimization pipeline was made, where each optimization has a visual analysis of a word cloud or Pareto.

![](https://i.imgur.com/X3b3Lqh.png)

![](https://i.imgur.com/UKjiKOK.png)


## 🧠 Neural network

A neural network was developed for the classification of tweets that obtained its best result with 57.3973% accuracy.

Some of the low precision hypotheses are:
- Voltatility of the chosen currency.
- Data quality, considering that some influential profiles in the market do not speak exclusively about bitcoin.
- Other currencies do not influence bitcoin, so some profile may have talked about the fall or rise of some currency but this was not reflected in the price of the cryptocurrency.
