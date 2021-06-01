# Sentiment-Aalysis
#NLP #Random Forest
## Context:

Twitter posses 330 million monthly active users, which allows businesses to reach a broad population and connect with customers without intermediaries. On the other side, there’s so much information that it’s difficult for brands to quickly detect negative social mentions that could harm their business.

That's why sentiment analysis/classification, which involves monitoring emotions in conversations on social media platforms, has become a key strategy in social media marketing.

Listening to how customers feel about the product/services on Twitter allows companies to understand their audience, keep on top of what’s being said about their brand, and their competitors, and discover new trends in the industry.

## Data Description:

A sentiment analysis job about the problems of each major U.S. airline. Twitter data was scraped from February of 2015 and contributors were asked to first classify positive, negative, and neutral tweets, followed by categorizing negative reasons (such as "late flight" or "rude service").

## Objective

The purpose of this analysis is to make up a prediction model where we will be able to predict whether a tweet is positive, negative or neutral

## Code
    (project_8.py)
## Conclusion
### Summary:

- We used dataset which has tweets in text format and their sentiment scores as positive, negative and neutral
- The goal was to build a model for text-classification.
- We Pre-processed the data using variuos techniques and libraries.
  - Used beautiful soup for removing html
  - We have also removed url and emojis
  - Removed numbers,puctuations, special characters which acts as noise to the text
  - We have used NLTK library to tokenize words , remove stopwords and lemmatize the remaining words
  - Removing stopwords is great as it lowers the dimensionality while using vectorization
  - Converted all to lowercase, that also helps in dimensionality reduction as python is case sensitive
  - As the data is less ,we used lemmatizing as it is more meaningful than stemming
- The pre-precessed data is converted to numbers, so that we can feed the data in the model.
- It can be converted using countvectorizer or TF-IDF
- TF-IDF value for every word and in some cases it may consider different meaning reviews as similar after stopwords removal. so to over come we can use BI-Gram or NGram.
- We build the classification model for countvectorized data and TF-IDF data , we predicted the result for the test data.
- Only a slight variation of accuracy for TF-IDF vectorized data has been observed
- After that we saw that using the above techniques, our model performed good in perspective of how the text classification models perform.
- We have used weighted loss as data is imbalanced. Used random forest clasiifier
- One more way to increase accuracy is to use different variations of Pre-processing techniques.
- Also for increasing accuracy, we can increase the data collection we have.
