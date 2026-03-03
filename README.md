# Book Genre Prediction using Deep Learning
This project explores the application of Natural Language Processing (NLP) and Deep Learning to automatically classify book titles into their respective genres. By comparing various word embedding techniques and neural architectures, the project identifies the most effective pipeline for genre categorization.

## 🚀 Project Overview
Predicting a book's genre based on its title or summary is a challenging NLP task due to the brevity of the text. This project implements a comparative study of three major word embedding methods paired with **CNN** and **LSTM** models to achieve high classification accuracy across 10 distinct genres.

## 🛠️ Technical Workflow

### 1. Data Preprocessing
To handle raw text effectively, we implemented a robust pipeline:

**Cleaning**: Removed punctuation, numbers, HTML tags, and URLs.
**Normalization**: Lowercasing, stopword removal, and stemming (Porter Stemmer).
**Sampling**: Addressed class imbalance in the 4,658-record dataset using oversampling and undersampling techniques.
**Tokenization**: Converted processed text into sequences for model input.

### 2. Word Embeddings
We evaluated three different vectorization strategies:

**CBOW (Word2Vec)**: Predicts a target word from surrounding context.
**Skip-gram (Word2Vec)**: Predicts surrounding context from a target word.
**GloVe (Global Vectors)**: Leverages global word-word co-occurrence statistics.

### 3. Model Architectures

**CNN (Convolutional Neural Networks)**: Used to extract local patterns and features from text sequences.
**LSTM (Long Short-Term Memory)**: Used to capture long-term dependencies and sequential context in book titles.

## 📊 Performance Evaluation
The models were evaluated using:

**Accuracy & Loss Curves**: To monitor learning progress and prevent overfitting.
**Confusion Matrix**: To identify specific genres that were frequently misclassified.
**Classification Report**: Detailed Precision, Recall, and F1-Score for each of the 10 genres.

