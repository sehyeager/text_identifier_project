# Using Logistic Regression to discern what country a text message originated in.

In this project, I use international text-message data provided by Codecademy Pro to build a logistic regression model that predicts the country of origin for text messages.  

## Pre-processing
The first step in my data preprocessing step is to apply code I built in a previous Codecademy lesson, using a WordNet lemmatizer to remove stop words and make the messages more amenable to tokenization, and then tokenizing the messages.  I import this script into my Pre-processing notebook, where I then apply a tfidf vectorizer to the words as well, giving me the dataset I will ultimately use to build my model.

## Modeling
Due to the enormous size of the dataset, I chose to use a simple Logistic Regression model for this first run.  I may try different ones in the future, but for now, simplicity is the best policy.  Additionally, to run this model on my own computer, it is necessary to take a random sample half the size of the dataset, as building off the entire dataset takes too long and will stall out before finishing.  Your own computer may differ, or you may be able to use cloud computing to get better results.

## Conclusions and Future Opportunities
In the end, my model is significantly over-fit, but not useless.  It far outperforms randomly predicting targets, and with more time spent in the future, I can close the gap between the training and testing accuracy scores. 