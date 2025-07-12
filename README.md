# Reddit-Based Analysis of Financial Anxiety During Economic Uncertainty

This project explores how Reddit users express financial anxiety during economically uncertain times. By analyzing over 1,000 comments from the subreddits r/personalfinance and r/unemployment, the project uncovers key themes, sentiment patterns, and linguistic insights using a combination of natural language processing (NLP), topic modeling, and machine learning techniques.

You can read the full paper here:  
**[Medium Article: Reddit-Based Analysis of Financial Anxiety During Economic Uncertainty](https://medium.com/@ytakte/reddit-based-analysis-of-financial-anxiety-during-economic-uncertainty-1493-words-711eda091274)**

## Project Goals
- Understand dominant topics related to financial stress on Reddit.
- Classify user sentiment as Coping or Anxious using supervised learning.
- Visualize linguistic patterns and emotional tone in online financial discourse.

## Tools & Technologies
- Python  
- Scikit-learn  
- PRAW (Python Reddit API Wrapper)  
- TextBlob  
- pyLDAvis  
- Pandas, NumPy, Matplotlib, Seaborn

## Methodology

### 1. Data Collection
- Scraped 1,000+ first-level Reddit comments using PRAW.
- Focused on the post-pandemic economic period to capture real-world anxiety.

### 2. Data Preprocessing
- Applied lemmatization, tokenization, and stopword removal.
- Built a custom NLP pipeline to prepare data for modeling.

### 3. Topic Modeling (Unsupervised)
- Performed coherence-optimized LDA using Scikit-learn to uncover 7 major themes, including:
  - Housing and Rent Stress  
  - Inflation and Salary Concerns  
  - Insurance, Taxes, and Life Expenses  
- Visualized topics using pyLDAvis and supporting bar charts.

### 4. Sentiment Classification (Supervised)
- Labeled sentiment using TextBlob polarity scores into two classes: Coping and Anxious.
- Used TF-IDF vectorization and trained a Logistic Regression model.
- Achieved:
  - Accuracy: 90%
  - AUC: 0.95  
- Visualized key predictive terms for both sentiment classes.

## Key Results
- Topic 7 (Housing/Rent) and Topic 4 (Inflation/Salary) appeared most frequently in Anxious comments.
- Words like "expensive", "debt", and "past" were strongly associated with anxiety.
- Coping users used terms like "wedding", "good", and "learning" more frequently.
