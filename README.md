# hbc-wise
## Code Repository for Honors By Contract Project
### Author: Michael Wise
### Advisor: Eitel Lauria
### Marist College, Spring 2022

---

This project focuses on the topic of sentiment analysis, a subset of natural language processing. The goal of sentiment analysis is to extract meaning and polarity from various lines of text. We explore the practicality of using Twitter as a mode of identifying sentiment of the general population during a specific time period. In this case study, we examined the polarity of over 20,000 tweets relating to the current war between Russia and Ukraine. Twitter sentiment analysis comes with many problems, including procedures for collecting/scraping the data, preprocessing tweets to clean text and turn it into something understandable by a computer, and the dilemma of dealing with unlabeled text. 
As a solution, we use a tool called [VADER](https://github.com/cjhutto/vaderSentiment), a rule-based lexicon, to derive sentiment scores for our Ukraine tweets (polarity was broken up into tweets of “positive”, “negative” and “neutral” sentiment). The validity of the model was tested by comparing its predictions with the pre-labeled [Sentiment140 dataset](https://www.kaggle.com/datasets/kazanova/sentiment140), in which VADER predicted the same labels as the pre-labeled data with 77% accuracy. We also explore classification models for predicting polarity using machine learning.
As a baseline, a multinomial Naive Bayes classifier in combination with a bag of words approach was trained to predict unseen tweets with 80% accuracy. Future avenues for sentiment analysis are also discussed, including the use of deep learning and transformers (like BERT) that have been the state-of-the-art techniques for natural language processing.

The repo contains the Juptyer notebook for all of the analysis. The `.csv` that was scraped and used to train the classifer is also provided.
