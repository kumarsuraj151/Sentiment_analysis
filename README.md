# Sentiment Analysis Project

## Overview
This project focuses on building various models to perform sentiment analysis on textual data. The goal is to classify reviews into positive or negative sentiments using multiple techniques:
- **Word2Vec + Logistic Regression**: Using word embeddings and a simple linear classifier.
- **GRU (Gated Recurrent Unit)**: A deep learning-based approach to capture sequential patterns.
- **DistilBERT Fine-Tuning**: Leveraging a pre-trained transformer model for state-of-the-art sentiment classification.


### Data Resources
The data used for this project can be obtained from the following link:
[Link to Movie Review Dataset](https://www.kaggle.com/competitions/word2vec-nlp-tutorial/data)

## Project Workflow
1. **Data Loading and Preprocessing**:
   - The dataset used is the IMDb movie reviews dataset, containing both text reviews and sentiment labels.
   - Reviews are preprocessed by tokenizing and normalizing the text using libraries like `gensim` and `nltk`.
   
2. **Feature Extraction**:
   - For the logistic regression model, **Word2Vec** embeddings are generated.
   - For GRU and DistilBERT, word tokenization and embedding layers (or pre-trained models) are used to represent the text.

3. **Model Training**:
   - A **Word2Vec + Logistic Regression** pipeline is set up to classify the reviews using traditional machine learning.
   - A **GRU-based deep learning model** is implemented to capture sequential dependencies in the text.
   - **DistilBERT** is fine-tuned for transfer learning, leveraging its pre-trained transformer architecture for improved performance.

## Models Implemented

### 1. Word2Vec + Logistic Regression
- **Word2Vec** is used to generate 300-dimensional word vectors.
- Reviews are converted into sentence-level embeddings by averaging the word vectors.
- **Logistic Regression** is applied to classify the sentiment of the reviews.
  
### 2. GRU (Gated Recurrent Unit)
- A GRU-based neural network is employed to handle the sequential nature of text data.
- The model is built using Keras and trained on tokenized reviews.
- GRU helps in capturing long-term dependencies in the sequence data.

### 3. DistilBERT Fine-Tuning
- DistilBERT, a lightweight version of BERT, is fine-tuned on the IMDb dataset using HuggingFace Transformers.
- The model is adapted for binary classification with the addition of a classification head.



