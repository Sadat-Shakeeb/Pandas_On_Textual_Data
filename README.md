# Pandas_On_NLP_Data
# Sentiment Analysis of IMDB Reviews

This project focuses on performing sentiment analysis on IMDB reviews using various data processing and analysis techniques. The dataset contains two columns: reviews and their corresponding sentiment (negative or positive). The steps performed in this project are described below.

## Table of Contents
- [Introduction](#introduction)
- [Data Gathering](#data-gathering)
- [Data Cleaning](#data-cleaning)
- [Preprocessing](#preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Vectorization](#vectorization)
- [Libraries Used](#libraries-used)

## Introduction
The goal of this project is to analyze the sentiment of movie reviews from IMDB. Sentiment analysis is a natural language processing (NLP) technique used to determine whether the sentiment expressed in a text is positive, negative, or neutral. This project involves various steps including data cleaning, preprocessing, exploratory data analysis (EDA), and vectorization to prepare the data for modeling.

## Data Gathering
The dataset for this project was obtained from Kaggle and consists of IMDB reviews and their sentiment labels. The dataset includes two columns:
1. **Reviews**: Textual reviews of movies.
2. **Sentiment**: Sentiment label indicating whether the review is positive or negative.

## Data Cleaning
The following data cleaning steps were performed on the dataset to ensure the data is in a usable format:
1. **Lowercasing**: Converting all text to lowercase to maintain consistency.
2. **Removing trailing and leading spaces**: Trimming unnecessary spaces from the beginning and end of each review.
3. **Removing URLs**: Using Regular Expressions (RegEx) to remove any URLs present in the reviews.
4. **Removing HTML tags**: Using RegEx to remove any HTML tags present in the reviews.
5. **Spelling correction**: Correcting spelling errors in the reviews using the TextBlob library.
6. **Removing punctuation**: Eliminating punctuation marks from the reviews.
7. **Removing special characters**: Removing any special characters that might interfere with text analysis.

## Preprocessing
The following preprocessing steps were performed to prepare the text data for analysis:
1. **Tokenization**: Converting sentences into lists of words using `nltk.tokenize.word_tokenize`.
2. **Stop word removal**: Removing common stop words (e.g., "the", "and", "is") using `nltk.corpus.stopwords` to focus on meaningful words.
3. **Stemming**: Reducing words to their root form to group similar words together (e.g., "running" to "run").

## Exploratory Data Analysis (EDA)
The following EDA steps were performed to gain insights into the dataset:
1. **Distribution of text length/word count**: Analyzing the distribution of the number of words in each review.
2. **Common unigrams, bigrams, and trigrams**: Identifying the most frequently occurring single words (unigrams), pairs of words (bigrams), and triplets of words (trigrams) in the reviews.
3. **Word cloud**: Creating a visual representation of the most frequent words in the reviews using a word cloud.

## Vectorization
The text data was converted into numerical format using vectorization techniques to prepare it for modeling:
1. **Bag of Words (BoW)**: Converting text into a matrix of token counts, which represents the frequency of words in each review.

## Ready for Modeling
After completing the above steps, the dataset is ready for building a sentiment analysis model. Various machine learning algorithms can be applied to classify the sentiment of the reviews as positive or negative.

## Libraries Used
The following libraries were used in this project:
- pandas
- numpy
- nltk
- regex
- textblob
- wordcloud

