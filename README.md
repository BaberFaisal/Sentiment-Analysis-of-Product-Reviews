#  Sentiment Analysis of Product Reviews

This project performs a complete sentiment analysis pipeline on a dataset of synthetic product reviews. It includes text preprocessing, sentiment scoring, exploratory data analysis, and topic modeling using NLP and machine learning techniques.

---

##  Project Structure

- **Data Source**: Synthetic dataset of 1000 reviews across 5 products.
- **Fields**:
  - `ReviewID`: Unique identifier
  - `ProductID`: Product (e.g., Product_A, Product_B)
  - `UserID`: User identifier
  - `Rating`: Integer (1–5)
  - `ReviewText`: Text of the review
  - `ReviewDate`: Submission date
- **Processed Fields**:
  - `CleanedReviewText`: Preprocessed review text
  - `SentimentScore`: Polarity score (via TextBlob)
  - `SentimentLabel`: Positive / Negative / Neutral

---

##   Key Features

###  Text Preprocessing
- Lowercasing
- Removal of punctuation, numbers, and special characters
- Tokenization
- Stopword removal
- Lemmatization using NLTK

###  Sentiment Analysis
- Sentiment polarity computed using **TextBlob**
- Reviews categorized:
  - `Positive`: score > 0.1
  - `Negative`: score < -0.1
  - `Neutral`: otherwise

###  Exploratory Data Analysis (EDA)
- Distribution of sentiments
- Word clouds for positive and negative reviews
- Sentiment trends over time
- Sentiment distribution by product
- Correlation between `Rating` and `SentimentScore`

###  Topic Modeling
- **NMF** applied to negative reviews using TF-IDF
- **LDA** applied to all reviews using CountVectorizer
- Top keywords extracted per topic to understand recurring themes

---

##  Insights & Recommendations

### Key Findings
- **Most Positive Product**: `Product_A`
- **Most Negative Product**: `Product_D`
- **Common Praise**: `recommend`, `excellent`, `perfectly`
- **Pain Points**: `broke`, `missing features`, `poor quality`

### Actionable Recommendations
- Investigate quality issues in `Product_D`
- Leverage positive feedback in marketing `Product_A`
- Improve feature delivery and customer service
- Use sentiment keywords in advertising strategy






