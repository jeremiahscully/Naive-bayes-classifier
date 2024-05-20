# Naive-bayes-classifier

# Tweepy Sentiment Analysis
This project explores sentiment analysis on Twitter data using the Tweepy library and compares the performance of the Multinomial Naive Bayes (MultinomialNB) classifier with the Vader sentiment analysis tool.

# Introduction
The objective of this project was to find a topic with a clear polarity division (positive, negative, neutral) that could be used to train and evaluate a sentiment analysis model. Initially, the GameStop short squeeze was considered, but the data was predominantly positive. Therefore, the topic of "flatearthers" was chosen for its controversy and distinct opposing views.

# Dataset
# Data Collection

* Twitter Developer Account: Created to obtain access tokens and keys for data mining.
* Tweepy API: Used to gather tweets based on specific hashtags.
* Rate Limiting: Limited to 200 tweets per day to avoid account suspension.
* Data Volume: Collected just under 1000 tweets for both topics.

# Data Annotation
* Polarity Metrics: Tweets were labeled as positive, negative, or neutral.
* Emotion Metrics: Tweets were categorized into emotions: unknown, joy, fear, anger, sadness, surprise, disgust.
* Cleaning: Removed white spaces, duplicate tweets, and applied stemming and stopping to preprocess the dataset.
# Model
# Multinomial Naive Bayes (MultinomialNB)
* Selection: Chosen for its efficiency in text classification with small datasets.
* Dataset: Comprised of 881 tweets and emotion entries.
# Performance:
* Emotions: Achieved 79% accuracy.
* Polarity: Achieved 78% accuracy.
* GameStop Dataset: Achieved 86% accuracy despite limited negative data.
# Improvements

* Dataset Size: Increasing the number of tweets could provide more meaningful annotations.
* Emotion Categories: Reducing the number of emotions to avoid overlap (e.g., sadness vs. anger).
* Comparison: MultinomialNB vs. Vader
* Vader Tool Setup: Classified tweets from the dataset using Vader.

# Performance:

* Neutral: Achieved 87% accuracy.
* Positive/Negative: Scored less than 0% accuracy.
* Conclusion: MultinomialNB significantly outperforms Vader in all aspects of text classification, likely due to Vader's limitations in understanding tweet complexity and slang.

# Conclusion
* Dataset Variety: Starting with a dataset offering a variety of outcomes improves model training.
* Controversial Topics: Topics with two clear opposing sides provide richer data for sentiment analysis.
* Model Performance: MultinomialNB is highly effective for classifying emotions and polarities in tweets, outperforming the Vader sentiment analysis tool.
