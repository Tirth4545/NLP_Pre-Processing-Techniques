# Assignment 2: Feature Engineering

## Feature Engineering Techniques

1. **Bag of Words (BoW)**: An approach to text representation where each document is represented as a vector of word counts. It disregards grammar and word order but retains multiplicity. This model can be used for various tasks like text classification and sentiment analysis.

2. **TF-IDF**: Stands for Term Frequency-Inverse Document Frequency. It's a numerical statistic that reflects how important a word is to a document in a collection. TF-IDF is often used in text mining and information retrieval.

## Word2Vec Implementation

**Word2Vec** is a popular word embedding technique that allows words to be represented in continuous vector space, capturing contextual relations between words. It consists of two main architectures:
- Continuous Bag of Words (CBOW)
- Skip-Gram

Using libraries such as Gensim, we can easily implement Word2Vec to create word embeddings that improve model performance in natural language processing tasks.