# Abstractive-Text-Summarization-using-Transformers-BART-Model
Deep Learning Project to implement an Abstractive Text Summarizer using Google's Transformers-BART Model to generate news article headlines.

# Project Description

## Introduction to Text Summarization using Transformers

Summarization has closely been and continues to be a hot research topic in the data science arena. Summarization is a technique that reduces the size of a document while preserving its meaning. It is one of the most researched areas among the Natural Language Processing (NLP) community.

Summarization techniques are categorized into two classes based on whether the exact sentences are considered as they appear in the original text. New sentences are generated using NLP techniques, extractive, and abstractive summarization. 

### Extractive Text Summarization

The most meaningful sentences in an article are selected and arranged comprehensively in extractive summarization. In other words, the summarized sentences are extracted from the article without any modifications.

### Abstractive Text Summarization

An NLP task aims to generate a concise summary of a source text. Abstractive summarization does not simply copy essential phrases from the source text but also potentially develops new relevant phrases, which can be seen as paraphrasing.

 

### Abstractive summarization has several applications in different domains such as,

* Science and R&D
* Books and literature. 
* Financial research and legal documents analysis
* Meetings and video conferencing 
* Programming languages, etc

## BART for Summarization of Text Data

BART stands for Bidirectional and Auto-Regressive Transformer. Its primary features are a bidirectional encoder from BERT and an autoregressive decoder from GPT. The encoder and decoder are united using the seq2seq model to form the BART algorithm. Let us look at it in more detail.

## BART Model Architecture
To understand the BART transformer, one needs to closely look at BERT and GPT. BERT performs the Masked Language Modelling with the help of its bidirectional transformer and predicts the missing values. On the other hand, GPT uses its autoregressive decoder to predict the next token in a sentence. Merging both of these results in the BART model, as depicted in the image below.

## BART Pre-training

There are five primary methods for training BART with noisy text:


1. Token Masking: Randomly, a small number of input points are masked.
2. Token Deletion: Certain tokens from the document are deleted.
3. Text Infilling: Multiple tokens are replaced with a single mask token.
4. Sentence Permutation: Sentences are identified with the help of ‘.’ and are then shuffled for training.
5. Document Rotation: A token is randomly selected, and the sequence is rotated so that the document begins with the chosen token.

These strategies augment the dataset and make the BART model better understand the natural language.