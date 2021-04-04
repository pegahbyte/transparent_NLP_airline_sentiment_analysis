# US airline tweets - Sentiment Analysis

This notebook contains a sentiment analysis for [this Kaggle challenge](https://www.kaggle.com/crowdflower/twitter-airline-sentiment) with an emphasis on making the NLP transparent. The "Behind the Code" sections show examples to create an understanding for the underlying transformations. This way, an intuition for the feature engineering process can be obtained.


## Content

0. Data and Libraries Load
1. Text Preprocessing  
    * Behind the Code: Translating Emoticons to Text
    * Behind the Code: Pre-Processing (Cleaning, Removal of Stop Words, Lemmatisation)
    * Behind the Code: Rule-Based Sentiment Analyser VADER  
        * Examples of most positive and most negative read tweets
        * Examples of misjudgement
    * Behind the Code: What top "(2-3)-grams" are the most common in the data?
    * Behind the Code: Getting an Intuition for fastText's Word Embedding
        * Most similar words
        * Similarity of words to "happy" and "sad" as proxies for positive and negative sentiment
2. Classification Model
      * Creating Test and Train Set with Various Feature Sets
      * Optimizing Hyperparameters for most Promising Classification Models
      * Evaluation

## Prerequisites

```
All libraries imported at the beginning must be installed to be able to run the code.
```
For the pre-trained word embeddings download the [fastText word vectors](https://fasttext.cc/docs/en/english-vectors.html) - 2 million word vectors trained on Common Crawl
