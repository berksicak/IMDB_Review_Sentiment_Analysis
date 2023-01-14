# IMDB_Review_Sentiment_Analysis

This project is designed to label the emotions of movie reviews on IMDB as positive or negative.

Data Analysis:


When the dataset is examined, it is observed that it consists of columns named 'text' and 'label'. In the 'text' column, the comments for the movie are given, and in the 'label' column, information about the feeling of the commentary is given. The 'label' column consists of two labels 'negative and 'positive' showing as '0' and '1'. First, the dataset was analyzed according to the 'label' column and its usefulness was determined. It was considered sufficient for the labels to be evenly distributed for usefulness.


Preprocess:


After the usefulness determination, some steps were taken to make the dataset ready for use. First of all, it was checked whether there is a null value in the 'text' column.Reviews are in lowercase. Unnecessary extensions, punctuation, and escape characters have been removed. Then the stopwords were removed. As the last operation of the preprocessing part, the lemmatization process was applied by considering at the position and relations of the word in the sentence.


Training:


Using the pipeline structure, words were vectorized and tokenized with Tfidf vectorizer. Then the model taken as a parameter is trained and evaluation metrics are calculated. Written function returns the pipe which has the most accurate model.

Results:

MultinomialNB:

Accuracy: 0.86

Precision: 0.86

Recall: 0.86

f1 Score: 0.86


BernoulliNB:

Accuracy: 0.85

Precision: 0.85

Recall: 0.85

f1 Score: 0.85


LogisticRegression:

Accuracy: 0.88

Precision: 0.88

Recall: 0.88

f1 Score: 0.88



XGBClassifier:

Accuracy: 0.85

Precision: 0.85

Recall: 0.85

f1 Score: 0.85



RandomForestClassifier:

Accuracy: 0.84

Precision: 0.84

Recall: 0.84

f1 Score: 0.84



Note:

The reason why all metrics are equal is because the dataset is very balanced. So this is not a problem.
