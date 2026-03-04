# Amazon Review Sentiment Analysis (NLP)

## Overview
This project analyzes customer reviews of a pharmaceutical supplement to classify sentiment as positive or negative.

The goal is to extract insights from textual data to support product improvement and decision-making.

## Dataset
- Source: Harvard Dataverse
- Records: ~5,000 reviews
- Features: Review text, ratings, metadata

## Methods

### Data Preprocessing
- Removed punctuation, URLs, numbers
- Tokenization and stopword removal
- Lemmatization
- TF-IDF vectorization (max_features=5000)

### Models Used
- Logistic Regression
- Multinomial Naive Bayes

### Handling Imbalance
- Used class_weight='balanced' for Logistic Regression


## Results
- Logistic Regression outperformed Naive Bayes
- Accuracy reduced after balancing but improved minority detection
- Negative sentiment detection improved significantly


## Key Insights
- Majority of reviews are positive (~88%)
- Model can detect dissatisfaction trends
- Useful for real-time customer feedback monitoring


## Tools & Libraries
- Python
- Scikit-learn
- NLTK / NLP preprocessing
- Matplotlib, Seaborn

## Business Impact
- Helps identify product issues early
- Supports customer satisfaction tracking
- Enables data-driven product improvements
