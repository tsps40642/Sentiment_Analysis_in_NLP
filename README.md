# Sentiment_Analysis_in_NLP

## Overview
As the Reuters, The Sun, Daily Mail, The Washington Post, New York Times, The Boston Globe.

use Word2Vec to construct model

The following is the processing steps:
1. Feature Engineering: Label the polarity score and
2. Spliting Data: Split data into train, test set, and fit the data into label encoder.
3. Label Encoder: Fit the training data into label encoder, that is, turn target variable 
(negative, positive) into 0,1.
4. TFIDF: Convert TFIDF vector, and compute TFIDF from training set.
5. Classification: Using decision tree algorithm as classifier. Fit training set on the 
classifier and predict labels on testing dataset.
6. Precision & Recall: Print out the accuracy and recall score of test data set for both 
negative and positive polarity

## Dataset

### Credit to other team members: Megan Kuo, Pola Lee
