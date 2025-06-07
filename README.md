# fake_news_detection

Project goal is detecting the fake news by analysing the whole news dataset. For this task and data I trained Multinominal Naive Bayes model.
For feature extraction I used : TF-IDF Vectorization
Model Accuracy: ~93%

## DATASET
You can use the dataset I used by downloading it from: "https://onlineacademiccommunity.uvic.ca/isot/2022/11/27/fake-news-detection-datasets/"
Also you can check the dataset from kaggle.com
This dataset includes 2 csv files one of them for true one of them for fake news.
Columns in this dataset are: 'title', 'text', 'subject', 'date'

## Methodology
Data Preprocessing
- Merged real and fake news into one dataset and this dataset is shuffled to avoid overfitting.
- For Cleaning lowercased all the texts, removed punctuation using regex, tokenized texts using NLTK word tokenize
- Lemmatization applied wordnetlemmatizer with POS tagging

For feature extraction
- Used TF-IDF vectorization applied on the news text

For model training
-used train/test split .2 for test .8 for training
-My model selection was: Multinomial Naive Bayes Classifier


Evaluation
- Accuracy Score
- Classification Report (Precision, Recall, F1-score)
