# Sentiment-Analysis-IMDB
Sentiment Analysis of IMDB dataset 

Sentiments: positive or negative review

Dataset:
2 columns (Text, sentiments) --- IMDB Dataset taken from kaggle containing 50k review
url-https://www.kaggle.com/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews#


Method-1: Linear Regression
Method-2: Linear svm
Method-3: multinomial naive bayes

For each method we have applied:
1. bag of words vectorizer method

2. tfidf matrix vectorizer method


Accuracy:

Method-1: Logistic regression model
 Regression
lr_bow_score : 0.7605
lr_tfidf_score : 0.7576

        classification report Logistic Regression
              precision    recall  f1-score   support

    Positive       0.76      0.76      0.76      4993
    Negative       0.76      0.76      0.76      5007

    accuracy                           0.76     10000
   macro avg       0.76      0.76      0.76     10000
weighted avg       0.76      0.76      0.76     10000

              precision    recall  f1-score   support

    Positive       0.75      0.78      0.76      4993
    Negative       0.77      0.74      0.75      5007

    accuracy                           0.76     10000
   macro avg       0.76      0.76      0.76     10000
weighted avg       0.76      0.76      0.76     10000

Method-2: svm
svm_bow_score : 0.6227
svm_tfidf_score : 0.5111

                classification report svm
              precision    recall  f1-score   support

    Positive       0.93      0.27      0.41      4993
    Negative       0.57      0.98      0.72      5007

    accuracy                           0.62     10000
   macro avg       0.75      0.62      0.57     10000
weighted avg       0.75      0.62      0.57     10000

              precision    recall  f1-score   support

    Positive       1.00      0.02      0.04      4993
    Negative       0.51      1.00      0.67      5007

    accuracy                           0.51     10000
   macro avg       0.75      0.51      0.36     10000
weighted avg       0.75      0.51      0.36     10000


Method-3: multinomial naive bayes
mnb_bow_score : 0.7576
mnb_tfidf_score : 0.7572

     classification report multinomial naive bayes
              precision    recall  f1-score   support

    Positive       0.75      0.76      0.76      4993
    Negative       0.76      0.75      0.76      5007

    accuracy                           0.76     10000
   macro avg       0.76      0.76      0.76     10000
weighted avg       0.76      0.76      0.76     10000

              precision    recall  f1-score   support

    Positive       0.75      0.77      0.76      4993
    Negative       0.76      0.75      0.76      5007

    accuracy                           0.76     10000
   macro avg       0.76      0.76      0.76     10000
weighted avg       0.76      0.76      0.76     10000


Word cloud for positive review words

Word cloud for negative review words

"""**Conclusion:**
* We can observed that both logistic regression and multinomial naive bayes model performing well compared to linear support vector  machines.
* Still we can improve the accuracy of the models by preprocessing data and by using lexicon models like Textblob, 
the only downside is it takes lot of time to normalize the text.


***Dataset taken from kaggle**
"""

Additional:  apply method in python
url for stock dataset https://drive.google.com/drive/folders/1jiJNeODlO76f6I0j5CNPzjCU1lOguWJ-
