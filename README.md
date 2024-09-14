# AI Text Detection Model
## Introduction
This project aims to develop a robust solution for detecting whether a piece of text was written by an AI or a human. It leverages machine learning classifiers such as RandomForest, LightGBM, Naive Bayes, and Logistic Regression, using TF-IDF vectorization for feature extraction. Two separate models (bigram and unigram) are built, allowing flexible choices based on feature representation.

## Model Architecture
### Unigram Model
The unigram model extracts unigram (single-word) features using TF-IDF. It employs two classifiers:<br>

1. Naive Bayes<br>
2. Logistic Regression<br>

The final prediction is based on an ensemble approach where the probabilities from both models are averaged to give a combined prediction.

### Bigram Model
The bigram model extracts bigram (word-pair) features from the text using TF-IDF. It utilizes two classifiers:<br>

1. RandomForest<br>
2. LightGBM<br>

Like the unigram model, the final prediction is based on the average of probabilities from both classifiers.

## Dataset
The model was trained on a dataset consisting of over 450,000 text samples, both AI-generated and human-written. The features for the model are extracted using TF-IDF with unigrams and bigrams.
find the dataset on [Kaggle](https://www.kaggle.com/datasets/shanegerami/ai-vs-human-text).
