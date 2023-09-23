# Fake-News-Detection


This repository focuses on the detection of fake news using the [Source-Based News Classification Dataset](https://www.kaggle.com/datasets/ruchi798/source-based-news-classification). The dataset includes various features, such as author, published date, title, text, language, site URL, main image URL, type, and a label indicating whether the news is real or fake. We utilize natural language processing (NLP) techniques and machine learning algorithms to classify news articles as real or fake.

## Dataset

The dataset contains the following columns:

- **author**: The author of the news article.
- **published**: The publication date of the article.
- **title**: The title of the news article.
- **text**: The textual content of the news article.
- **language**: The language in which the article is written.
- **site_url**: The URL of the news site.
- **main_img_url**: The URL of the main image in the article.
- **type**: The type or category of the article.
- **label**: The target variable indicating whether the news is real (1) or fake (0).

## Preprocessing

The code includes text preprocessing steps to prepare the data for machine learning:

1. **Stemming**: The `stemming` function reduces words to their root form to simplify text analysis. It removes non-alphabetical characters, converts text to lowercase, tokenizes the text, and applies stemming using the Porter stemmer. Additionally, it removes common English stopwords.

2. **Text Vectorization**: To convert textual data into numerical form, the code uses the TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer. It transforms the text data into a numerical format suitable for machine learning.

## Machine Learning

The code utilizes the following machine learning steps:

- **Data Splitting**: The dataset is split into training and testing sets (80% training, 20% testing) using stratified sampling to maintain class distribution balance. The random seed is set to ensure reproducibility.

- **Model Training**: Machine learning algorithms, such as logistic regression, decision trees, or others, can be used to train the model on the preprocessed data.

- **Model Evaluation**: The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. This helps assess the model's effectiveness in distinguishing real news from fake news.

