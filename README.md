# Basic Text Analytics 

Data Set Description: Amazon Reviews dataset for cell phones and accessories
Data Link: https://jmcauley.ucsd.edu/data/amazon/ 

### Project Overview: 

In this project we are exploring different techniques to analyse the text. Major concepts covered are Lemmatization, Stemming, Tokenization, Stop wort removal, parts of speech tagging. We also create an LDA model and identify top words. We identify the TFIDF features by dividing the data into train and test.  


### Steps 
1.	Extracted the reviewText and overall fields from the file. We are working with only two files.
2.	Performed these steps as part of pre-processing: lowercasing and removing punctuation. Computed IDF of all words in these reviews. Reported the top 20 words and bottom 20 words, based on IDF, with their IDF scores for the top 10000 reviws. 
3.  Used Spacy to perform sentence detection. Each line has a review ID (i.e., line number from the file) and the sentence itself, this was done on top 10 reviews
4.	Performed word tokenization, lemmatization, part-of-speech tagging using Spacy by giving a review ID (i.e., line number from the file), token (i.e. word), lemma, and POS tag for each Line.
5.	Took the first 1000 review texts and created an LDA model with 10 topics by using gensim. Identified the top 50 words. 
6.	Took the first 80% dataset for train and remaining 20% for test. On the train set, I obtained TFIDF(Term Frequency- Inverse Document Frequency) features (with 50K vocabulary) and learnt a multinomial Naïve Bayes model. Reported the accuracy on the test set for this five-class classification problem. 
