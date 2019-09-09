
<img src="images/wordcloud.png">

---

# [Medium Files](https://github.com/dc-aichara/DS-ML-Public/tree/master/Medium_Files)

## 1. [hyp_tune.ipynb](https://github.com/dc-aichara/DS-ML-Public/blob/master/Medium_Files/hyp_tune.ipynb)

- A notebook to guide hyperparameters optimization using Bayesian model based optimization. 

Example hyperparameters optimization results table for LightGBM Regressor on Boston Housing data. 

<img src="images/hyp_lgbm.png">

Read complete article on [Medium](https://medium.com/analytics-vidhya/hyperparameters-optimization-for-lightgbm-catboost-and-xgboost-regressors-using-bayesian-6e7c495947a9). 

## 2. [Bar_Plot_Animation.py ](https://github.com/dc-aichara/DS-ML-Public/blob/master/Medium_Files/Bar_Plot_Animation.py)
- Creates animation of bar plots using matplotlib python package <br>
[Read complete tutorial on Medium](https://medium.com/@dc.aichara/making-animated-bar-plots-of-top-16-cryptocurrencies-market-capitalization-price-and-volume-7889788af264)<br>
[Watch animation on YouTube](https://www.youtube.com/watch?v=jqSuaRpCnro) <br>
[![YouTube Video](http://img.youtube.com/vi/jqSuaRpCnro/0.jpg)](http://www.youtube.com/watch?v=jqSuaRpCnro)

## 3. [telegram.py](https://github.com/dc-aichara/DS-ML-Public/blob/master/Medium_Files/telegram.py)
- Telegram chat data extraction and data processing <br>
[Medium Tutorial](https://medium.com/@dc.aichara/telegram-channel-data-extraction-users-information-chats-and-specific-messages-and-data-21bb54710fd3)  <br>

> An example of telegram chats which contain keyword 'bitcoin' or 'btc'

<img src='images/Bitcoin_text_ts.png'>


## 4. [Bitcoin_messages_telegram.py](https://github.com/dc-aichara/DS-ML-Public/blob/master/Medium_Files/Bitcoin_messages_telegram.py)
- Get text messages from telegram groups and channels which contain word 'bitcoin' or 'btc'. <br>

Example: 

```python
>>> tele_btc_messages.head()

```
<img src='images/tele_text.png'>

## 5. [telegram_user_status.py](https://github.com/dc-aichara/DS-ML-Public/blob/master/Medium_Files/telegram_user_status.py)
- Use to get users who were online in last 24 hours.

Example: 
```
$ cd DS-ML-Public
$ python telegram_user_status.py 12345 fe3922d77g6wgwgwyu35g46c9 bitgrit
Number of active users in last 24 hours is 1530.
          User               status
0  Dayal Chand               online
1       Sameer             recently
2  Dikesh Shah  2019-07-02 01:13:19
3       Crypto  2019-07-02 00:47:50
4        Billy  2019-07-02 01:32:49

```
*** 

## Others 

## 1. [lok_sabha_results.py](https://github.com/dc-aichara/DS-ML-Public/blob/master/Others/lok_sabha_results.py)
- Get [Lok Sabha elections 2019 results](https://results.eci.gov.in/pc/en/partywise/index.htm) using web scraping technique with requests and BeautifulSoup python packages. 

## 2. [crypto_news_scraper.py]()
- Python script to extracted cryptocurries related news from [CoinDesk](https://www.coindesk.com), [Cointelegraph](https://cointelegraph.com) and [cryptonewsz](https://www.cryptonewsz.com). 

### Usages
$ git clone https://github.com/dc-aichara/DS-ML-Public.git
$ cd DS-ML-Public/Others
$ python3 

```python
>>> from crypto_news_scraper import NewsScrap
>>> news = NewsScrap()
>>> df_coindesk = news.CoinDesk_News()
>>> df_coindesk.head()
  category                                            heading  ...                time    source
0     news  Dapp.com Closes $1 Million Investment Round Le...  ... 2019-09-06 22:00:00  CoinDesk
1     news  Telegram Finally Releases Code for Its $1.7 Bi...  ... 2019-09-06 21:46:00  CoinDesk
2     news  Massive $1 Billion Bitcoin Whale Transaction M...  ... 2019-09-06 19:00:00  CoinDesk
3     news  Ethereum Picks Early October for Testnet Activ...  ... 2019-09-06 18:00:00  CoinDesk
4     news  Dapp Data Site DappRadar Raises $2.33 Million ...  ... 2019-09-06 17:00:00  CoinDesk

[5 rows x 6 columns]
>>> df_cointelegraph = news.Cointelegraph_News()
>>> df_cointelegraph.head()
  category                                            heading  ...                 time         source
0     News  Crypto and Blockchain Adoption Grows: 5 Import...  ...  2019-09-09 11:15:03  CoinTelegraph
1     News  World’s ‘First’ Blockchain Smartphone to Becom...  ...  2019-09-09 08:15:03  CoinTelegraph
2     News  Ethereum's Istanbul Hard Fork Implementation D...  ...  2019-09-09 08:15:03  CoinTelegraph
3     News  Blockchain Startup DappRadar Raises $2.33M Fro...  ...  2019-09-09 08:15:03  CoinTelegraph
4     News  Huobi’s Research Arm to Partner with the Unive...  ...  2019-09-09 07:15:03  CoinTelegraph

[5 rows x 6 columns]
>>> df_all = news.get_all_news()
Getting news from CoinDesk!!
Getting news from Cointelegraph!!
Getting news from cryptonewsz!! This will take 1-2 mintues. 😉
>>> df_all.head()
  category                                            heading  ...                 time    source
0     news  Dapp.com Closes $1 Million Investment Round Le...  ...  2019-09-06 22:00:00  CoinDesk
1     news  Telegram Finally Releases Code for Its $1.7 Bi...  ...  2019-09-06 21:46:00  CoinDesk
2     news  Massive $1 Billion Bitcoin Whale Transaction M...  ...  2019-09-06 19:00:00  CoinDesk
3     news  Ethereum Picks Early October for Testnet Activ...  ...  2019-09-06 18:00:00  CoinDesk
4     news  Dapp Data Site DappRadar Raises $2.33 Million ...  ...  2019-09-06 17:00:00  CoinDesk

[5 rows x 6 columns]


```

## [My Medium Articles](https://medium.com/@dcaichara)
-  [Hyperparameters Optimization for LightGBM, CatBoost and XGBoost Regressors using Bayesian Optimization.](https://medium.com/game-of-data/hyperparameters-optimization-for-lightgbm-catboost-and-xgboost-regressors-using-bayesian-6e7c495947a9)
-  [Google Spreadsheets Automation with Python](https://medium.com/@dcaichara/play-with-google-spreadsheets-with-python-301dd4ee36eb)
-  [Telegram Group/Channel Data Extraction (User’s information, chats, and specific messages), and Data Processing](https://medium.com/@dcaichara/telegram-channel-data-extraction-users-information-chats-and-specific-messages-and-data-21bb54710fd3)
-  [12 Things to know about Jupyter Notebook Markdown](https://medium.com/@dcaichara/12-things-to-know-about-jupyter-notebook-markdown-3f6cef811707)
-  [Making Animated Bar Plots of Top 16 CryptoCurrencies (Market Capitalization, Price and Volume)](https://medium.com/@dcaichara/telegram-channel-data-extraction-users-information-chats-and-specific-messages-and-data-21bb54710fd3)
-  [Coin Hopping Attack : How did c0ban (First ICO from Japan) deal with it using LWMA ?](https://medium.com/@dcaichara/coin-hopping-attack-how-did-c0ban-first-ico-from-japan-deal-with-it-using-lwma-9facda2f02b6)
