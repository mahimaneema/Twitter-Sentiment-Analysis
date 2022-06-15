# Twitter-Sentiment-Analysis
Descriptive and Predictive (classification) analysis on the sentiments of people from all over the world regarding the the conflict between Russia and Ukraine

Russia began a full-scale invasion of Ukraine on 24 February 2022, in an escalation of the Russo-Ukrainian War that began in 2014. The invasion is the largest conventional military attack on a sovereign state in Europe since World War II

The conflict between Russia and Ukraine has been causing knock-on effects globally. Distribution and cost
of oil has been great impacted, commodities such as Wheat and Aluminum prices increased, European
banks stocks fell affecting global stock markets. 

Data Source: Extract data from Twitter. Expected size of the data collected 30,000 observations.[team_twitter_data.csv](https://github.com/mahimaneema/Twitter-Sentiment-Analysis/files/8904975/team_twitter_data.csv)

Prerequisite
A developer account in twitter is required to use twitter API. Limited Access provides us with monthly
tweet cap of 500,000.
API: Twitter API v2[Twitter_Keys.csv](https://github.com/mahimaneema/Twitter-Sentiment-Analysis/files/8904976/Twitter_Keys.csv)

Library: Tweepy, TextBlob, WordCloud, Scikit-Learn
Tools: Jupyter Notebook
Twitter Query: Biden (US President), Putin (Russian President) and Zelenskyy (Ukraine President)
Twitter fields: username, location, date, text, verified, and tweet source
Predictive models: Logistic and KNN

The war began on Feb 22 officially, we will be mining data periodically on dates Mar 06, 2022 (15,000
observations), and Mar 13, 2022 (15,000 observations). The recent search method of API helps us retrieve
tweets of max period, last 7 days. 5,000 tweets from users on three presidents are mined for the abovementioned dates.
Once data is mined, sentiment analysis is run on the texts of each tweet using TextBlob library to classify
tweets as Negative, Neutral and Positive.
New sentiment attribute will be used for Predictive analysis using Logistic and KNN using scikit library with
independent attribute text (only 1 independent).[final_data_twitter.csv](https://github.com/mahimaneema/Twitter-Sentiment-Analysis/files/8904977/final_data_twitter.csv)

Descriptive Questions:
• Who gets the most negative sentiment among three presidents?
• Which locations do have highest/lowest, positive, and negative sentiments?
• Are the negative sentiments most by unverified users?
• What type of sources are most used by users for tweets?
• What are the most common words used for each president (Word Cloud)
