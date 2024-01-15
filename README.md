# Sentiment_Analysis_in_NLP

## Overview
This is a team project to analyze sentiment inclination of editorial articles across 6 big media, including Reuters, The Sun, Daily Mail, The Washington Post, New York Times, The Boston Globe, in the period of Russia-Ukraine War.  

We would like to visualize their sentiment score, which is the polarity (0 for negative, 1 for positive) in the end, and also present the time trend of the sentiment change.  

## Dataset
We utilize Beautiful Soup to web-crawl all editorial articles around the beginning of the war until 2022-06-01.   

## Solution Steps
We use Word2Vec to construct models to predict polarity (0 for negative, 1 for positive).  

The followings are solution steps:  
1. Load in web-crawled articles that we had done in advance, presenting in Sentiment_analysis_web_crawling.ipynb (only partial in this notebook)  
2. Data preprocessing: remove unnecessary elements like punctuations and combine the web-crawled articles into a dataframe   
3. Use VADER(Valence Aware Dictionary and sEntiment Reasoner) to calculate the polarity score for each article  (VADER: a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media)
4. Mannually label the target variable: by setting our threshold, we mannually label each article as 0(negative) or 1(positive)
5. Build models to predict the sentiment score of each article: we construct Gradient Boosting Classifier, SVM Classifier, and RandomForest Classifier to conduct the prediction, and do some experiments for parameter adjusting  
6. Train GRU (Gated Recurrent Units) model to predict the polarity score in time serise for each medium, and report model performance  
7. Visualization for polarity scores for media separately and in time serise  

### Credit to other team members: Megan Kuo, Pola Lee
