# Quora_question_pair

Description:
Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect
with people who contribute unique insights and quality answers. This empowers people to learn from each
other and to better understand the world.Over 100 million people visit Quora every month, so it's no 
surprise that many people ask similarly worded questions. Multiple questions with the same intent can
cause seekers to spend more time finding the best answer to their question, and make writers feel they
need to answer multiple versions of the same question. Quora values canonical questions because they provide
a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

Problem Statement:
Identify which questions asked on Quora are duplicates of questions that have already been asked.
This could be useful to instantly provide answers to questions that have already been answered.
We are tasked with predicting whether a pair of questions are duplicates or not.

Data overview:
Dataset contains 5 columns : qid1, qid2, question1, question2, is_duplicate

Our task:
We have to predict whether 2 questions are duplicate or not.

Performance Matric:
We use logloss for evaluating the performance of our models.

Step by Step Procedure to solve this problem:
Firstly I took 50k datapoints from train_data and did Data Visualisation of Quora duplicate and non_duplicate questions. 
I add some classical NLP features like word_common_shar,no_of_words, no_of_characters etc.
I did Text Preprocessing and cleaning I add some complex NLP distance based features.
I did Analysis of the Extracted features. I plot the TSNE with 15 advanced features which i got.
I split the data and apply various featurizations like tfidf weighted word2vec and tf-idf vectorizer.
I save all features into the files and then read the data from file and then store the data in sql database.
I made the Baseline model I apply Logistic regression, Linear SVM and XGBOOST with Tf-idf_Weighted_word2vec featurizer 
Last,I apply Logistic regression, Linear SVM and XGBOOST with Tf-idf vectorizer







