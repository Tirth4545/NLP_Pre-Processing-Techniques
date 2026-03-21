# NLP Preprocessing Techniques

## Project Overview
This project is dedicated to exploring various Natural Language Processing (NLP) preprocessing techniques that transform raw text into a format suitable for analysis. NLP preprocessing is vital for tasks such as sentiment analysis, text classification, and machine translation, as it helps improve model performance by cleaning and structuring data appropriately.

### Key Techniques Explored in This Project:
1. **Tokenization**: Splitting text into individual words or phrases.
2. **Lowercasing**: Converting all text to lowercase to maintain uniformity.
3. **Removing Punctuation**: Eliminating special characters and punctuation marks.
4. **Stop Words Removal**: Filtering out common words that contribute little meaning.
5. **Stemming and Lemmatization**: Reducing words to their root forms.
6. **N-grams Generation**: Creating sequences of N items from the text.
7. **Text Normalization**: Standardizing text representation.

## Code Implementation
The implementation of the above techniques can be found in the `Text_Pre_processing_techniques.ipynb` notebook. Below is a summary of the relevant code snippets:

---

# Assignment 2: Feature Engineering and Word Embeddings

## Overview
Assignment 2 extends the NLP preprocessing techniques with feature engineering and advanced word embedding methods. This assignment focuses on converting preprocessed text into numerical representations suitable for machine learning models.

## Assignment Tasks

### Task 1: Feature Engineering Techniques

#### 1.1 Bag of Words (BoW)
**Bag of Words** is a text representation technique where:
- Each document is converted into a vector of word frequencies
- Grammar and word order are disregarded
- Word multiplicity (frequency) is preserved
- Useful for text classification, sentiment analysis, and document similarity

**Implementation Details:**
- Using `CountVectorizer` from sklearn
- Creates a matrix where each row represents a document and columns represent unique words
- Values represent word frequencies in each document

#### 1.2 TF-IDF (Term Frequency-Inverse Document Frequency)
**TF-IDF** is a numerical statistic that:
- Reflects how important a word is to a document in a collection
- Combines two metrics:
  - **TF (Term Frequency)**: How often a word appears in a document
  - **IDF (Inverse Document Frequency)**: How unique/rare a word is across documents
- Highlights words that are both frequent and discriminative

**Implementation Details:**
- Using `TfidfVectorizer` from sklearn
- Produces normalized vectors with TF-IDF weights
- Better than BoW for highlighting important terms

### Task 2: Word2Vec Implementation

**Word2Vec** is an advanced word embedding technique that:
- Represents words in a continuous vector space
- Captures semantic and contextual relationships between words
- Uses neural networks to learn word representations
- Consists of two architectures:
  - **Continuous Bag of Words (CBOW)**: Predicts target word from context words
  - **Skip-Gram**: Predicts context words from target word

**Implementation Details:**
- Using `Word2Vec` from Gensim library
- Input text must contain 200+ words for meaningful embeddings
- Parameters:
  - `vector_size`: Dimension of word vectors (e.g., 100)
  - `window`: Context window size (e.g., 5 words)
  - `min_count`: Minimum word frequency threshold
  - `workers`: Number of threads for training

**Similarity Analysis:**
- Computes cosine similarity between word vectors
- Identifies semantically similar words
- Range: -1 (opposite) to +1 (identical)

## Notebook Implementation
All implementations can be found in `Text_Pre_processing_techniques.ipynb`:

### Key Outputs:
1. **BoW Feature Matrix**: Word frequency vectors
2. **TF-IDF Matrix**: Weighted importance vectors
3. **Word2Vec Model**: Trained embeddings on 200+ word dataset
4. **Similarity Scores**: Relationships between key terms

### Example Results from Word2Vec:
- Similarity calculations between words like 'technology' and 'learning'
- Most similar words to given terms
- Semantic relationship discovery

## Dependencies
- `nltk`: Natural Language Toolkit
- `scikit-learn`: Machine learning library (CountVectorizer, TfidfVectorizer)
- `gensim`: Word2Vec implementation
- `numpy`: Numerical computations
- `scipy`: Scientific computing

## Assignment Deadline
**Sunday, 10:00 AM**

## Conclusion
Understanding and implementing these preprocessing and feature engineering techniques are crucial steps in preparing text data for any NLP task. This project provides foundational insights into:
- Converting raw text into numerical representations
- Extracting meaningful features from text
- Understanding semantic relationships between words
- Building robust NLP pipelines for machine learning models

These techniques form the foundation for more advanced NLP tasks such as sentiment analysis, machine translation, named entity recognition, and text classification.