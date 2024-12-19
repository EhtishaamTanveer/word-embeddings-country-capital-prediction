# Word Embedding Analysis and Country-Capital Prediction

This repository contains a Jupyter Notebook exploring word embeddings and their applications, specifically focusing on predicting countries from their capitals. The project delves into the properties of word vectors, demonstrating how they capture semantic relationships between words.

## Overview

This project explores the fascinating world of word embeddings (word vectors) and demonstrates their ability to capture semantic relationships between words. Using a single Jupyter Notebook, I perform several key analyses:

*   **Analogy Prediction:** I use word vectors to solve analogy problems (e.g., "king is to man as queen is to ?"). This showcases the vector arithmetic properties of word embeddings.
*   **Dimensionality Reduction and Visualization:** I apply Principal Component Analysis (PCA) to reduce the dimensionality of the word embeddings, allowing me to visualize them in a two-dimensional space. This provides insights into the clustering and relationships between words.
*   **Similarity Measurement:** I calculate the cosine similarity between word vectors to quantify the semantic relatedness of words.
*   **Country-Capital Prediction:** I leverage the learned relationships to predict countries based on their capitals, demonstrating a practical application of word embeddings.

## Project Structure

This repo contains the following files:

*   `word_embedding_analysis.ipynb`: This notebook contains all the code for word embedding analysis, PCA visualization, similarity calculations, and country-capital prediction.
*   `utils.py`: All the helper functions used in the main file are stored here
*   `w3_unittest.py` Test cases are stored here to verify the correctness of the functions created in main file.

## Steps in the Project

* Importing the Data
* Implementation of Cosine Similarity and Euclidean Distance methods
* Using these methods to find country of each capital
* Evaluate our predictions using *accuracy* metric
* Peforming Dimensionality Reduction using PCA to visualize the results

## Results Accuracy

- Through a 300-dimension word embedding vector, I was able to accurately predict relationships among words.
- By feeding 2 related words and 1 unknown word, I predicted a 4th word that was related to the unknown word e.g. "Athens is to Greece as Bangkok is to ____" ?
- The similarity between words was calculated through Cosine Similarity function.
- True predictions were filtered out and their ratio with total number of predictions to get the accuracy.
- I received 92% Accuracy with this approach.

## Dependencies

The following Python libraries are required to run the notebook:

*   `numpy` - for vectorized calculations
*   `matplotlib` - for plotting
*   `pandas` - for better representation of tabulated data
*   `pickle` - for loading files
*   `nltk` - for tokenization
*   `gensim` - for loading word embeddings

You can install these dependencies using pip:

```bash
pip install numpy matplotlib pandas pickle nltk gensim
```
## Acknowledgements

* Dataset Sources:
  * [Google News](https://code.google.com/archive/p/word2vec/)
  * [Coursera](https://www.coursera.org/)
