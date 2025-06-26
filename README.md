# Spam-Filter-using-ML-Algorithms
Trained several classifiers (Naive Bayes, KNN, logistic regression) to build a spam classifier. Analysed dataset to find words that are indicative of an email being a spam.

Problem Statement:
A spam filter is a computer program that classifies e-mail messages as either spam (unwanted) or ham (wanted). The spam filter maintains a set of features. A feature is a characteristic of messages that the spam filter can use to distinguish ham from spam. A feature could be simply the presence of a word in the message, for example, ”the message contains the word ’lottery’”, and it could be much more complex/powerful, for example, ”the subject line is all capitals” or ”the message body mentions many Internet domains”. Given (1) a set of features, (2) a set of messages known to be ham, and (3) a set of messages known to be spam, the spam filter learns how to classify incoming messages as ham
or spam.

In this exercise we are going to train a spam filter using the Apache SpamAssassin public mail corpus.
1. Download the files 20030228_easy_ham.tar.bz2 and 20030228_spam.tar.bz2 from
https://spamassassin.apache.org/old/publiccorpus/. The first file contains 2500
ham messages, and the second one contains 500 spam messages.
2. Unzip the datasets and familiarize yourself with the data format.
3. Use Python’s email module to parse the email messages (see code example at the end).
4. Apply text preprocessing techniques to convert each email into a feature vector. These
may include tokenization of the text into words, removing stop words, replacing all
URLs with ”URL”, TF-IDF vectorization, etc.
5. Split the emails into training and test sets.
6. Try out several classifiers (e.g., Naive Bayes, KNN, logistic regression) and see if you
can build a great spam classifier, with both high recall and high precision.
7. Show the confusion matrix and the classification report of your best classifier on both
the training and the test set.
8. How does the size of the training set affect the classifier’s performance? Train your
classifier with different training set sizes, and show the learning curve (test set error vs.
training set size).
9. Intuitively, some tokens may be particularly indicative of an email being in a particular
class. We can get an informal sense of how indicative token i is for the spam class by
looking at:
<img width="305" alt="image" src="https://github.com/user-attachments/assets/5dce9cd9-d35d-48c4-a2b3-3c5a900745d9" />
Using this measure, find the 10 tokens that are most indicative of the spam class (i.e.,
have the highest positive value on the measure above).
