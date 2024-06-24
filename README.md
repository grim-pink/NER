# Named Entity Recognition

## Overview

This project involves two main tasks in Natural Language Processing (NLP): Legal Named Entities Recognition from Indian court judgment texts and Aspect Term Extraction from laptop review texts. The tasks are divided into multiple parts including data preparation, baseline model implementation, and advanced model implementation.

### Task 1: Legal Named Entities Recognition
The goal is to identify and classify named entities in Indian court judgment texts. Entities include key subjects such as statutes, precedents, judges, etc. 

### Task 2: Aspect Term Extraction
The objective is to extract relevant terms from laptop reviews that are essential for opinion mining and sentiment analysis.

## Part 1: Data Preparation

### Task 1 Dataset
1. **Splitting Data**: The dataset is split into training and validation sets in an 85:15 ratio.
2. **BIO Chunking**: The data is tokenized, and each token is assigned a BIO (Beginning-Intermediate-Outside) label corresponding to the 13 legal entities.

### Task 2 Dataset
1. **BIO Chunking**: The data is tokenized, and each token is assigned a BIO label for aspect terms.

## Part 2: Baseline Models Implementation

### RNN-based Sequence Tagging Models
Three models are implemented for sequence tagging:
1. Vanilla RNN
2. LSTM Network
3. GRU Network

Each model uses three different pre-trained word embeddings: Word2Vec, GloVe, and FastText. Additionally, a contextualized embedding like BERT or LegalBERT can be used. 

### Evaluation
- Models are evaluated based on Macro-F1 and Accuracy.
- Plots are generated for training and validation loss, and Macro-F1 scores against epochs.

## Part 3: BiLSTM-CRF Model Implementation

### BiLSTM-CRF Model
A BiLSTM-CRF model is implemented for token classification, using three different pre-trained word embeddings and one contextualized embedding. 

### Evaluation
- The same metrics and plotting as in Part 2 are used.
- Label-wise F1 scores are calculated and visualized.

This project provides a comprehensive approach to handling named entity recognition and aspect term extraction using various NLP models and embeddings.
