# Movie Review Classification with Word Embeddings (Feb 2018)
Classified movie reviews into positive and negative with GloVe embeddings and machine learning techniques.

## Description
The large movie view dataset (http://ai.stanford.edu/~amaas/data/sentiment/) contains a collection of 50,000 reviews from IMDB. The dataset contains an even number of positive and negative reviews and is divided into training and test sets. The training set is the same 25,000 labeled reviews. The sentiment classification task consists of predicting the polarity (positive or negative) of a given text.

## Steps
1. Use the libary spacy to tokenize data. 
2. Download embedding vectors from https://nlp.stanford.edu/projects/glove/.
3. Read the 300 dimensional GloVe embeddings into a dictionary.
4. Create average feature embedding for each sentence (ignore stopwords).
5. Fit an XGBoost classifier to this data. Report test and training errors.
6. Compare previous results to fitting XGBoost to a one-hot encoding representation of the data with bag of words. Report test and training errors.
