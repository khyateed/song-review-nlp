# Classification of Pitchfork Music Reviews
### An Exploration of NLP Methods (Ongoing)<br>By Khyatee Desai

# Introduction
This project explores text preprocessing, stopword removal, lexicon normalization, frequency distribution, part-of-speech analysis, sentiment analysis, vectorization, feature engineering and classification modeling of music reviews published on Pitchfork

# Data
The dataset for this project comes from a Kaggle collection of [song reviews](https://www.kaggle.com/nolanbconaway/pitchfork-data) published on Pitchfork.com. The data is stored as a collection of tables within a Sqlite database.

# Cleaning & Processing 
- join relevant tables
- create the target variable: "good" reviews (scored above 8.0,) and "bad" reviews (scored below 6.0)
- remove stopwords and punctuation
- identify language using langdetect
- stemm and lemmatize

# Exploration
### Frequency Distribution
After creating a frequency distribution, we inspect the most common words used in each class ("good" vs "bad" reviews.)<br>
**Best Reviews:**<br>
`('like', 11948),
 ('album', 8745),
 ('music', 8523),
 ('one', 7614),
 ('band', 6755)`<br><br>
**Worst Reviews:**<br>
`('like', 10444),
 ('album', 7030),
 ('one', 5329),
 ('band', 5123),
 ('music', 4562)`<br>
There does not appear to be a significant difference among the most frequently used words in each review.
### Word Clouds
Word clouds are then generated to visually inspect the most common words in each class.<br>
**Best Reviews:**<br>
![Best Cloud](images/best_cloud.png)<br>
**Worst Reviews:**<br>
![Worst Cloud](images/worst_cloud.png)<br>

# Feature Engineering
The feature engineering process includes length analysis, Part of Speech (POS) analysis, and sentiment analysis.
### Length Analysis
Length analysis uses lambda functions to measure `word_count`,	`char_count`, `sentence_count`,	`avg_word_length`,	and `avg_sentence_length`.<br>
"Best" reviews had an average word count of 910.717931, while "worst" reviews had an average word count of 680.766667.<br>
Along the same vein, Best reviews had an average sentence count of 34.734050, vs 26.614667 for Worst reviews. These statistics indicate that top-scoring reviews contain more words and longer sentences, in general.
### Part of Speech Analysis
### Sentiment Analysis

# Vectorization

# Modeling

# Evaluation

# Next Steps

