# Foundations of CCNLP

## About Cognitive Computing and NLP

Cognitive Computing and Natural Language Processing (NLP) is a field of AI focused on enabling machines to understand, interpret, and generate human language. It combines linguistics, machine learning, and computational techniques to power applications like chatbots, sentiment analysis, translation, and speech recognition.

## What This Repo Contains

This repository is a collection of foundational NLP implementations, covering core text processing techniques — from tokenization, stemming, and POS tagging to word embeddings, named entity recognition, text summarization, sentiment analysis, and speech-based NLP — built as part of my coursework and AI research journey.

## Tech Stack

- Python 3.10
- NLTK
- Gensim
- Sumy
- gTTS, SpeechRecognition, IBM Watson SDK

## Datasets & Corpora

This repo mostly uses built-in corpora and pretrained resources rather than external datasets — NLTK corpora (e.g. Gutenberg, stopwords, VADER lexicon) and Gensim's `text8` dataset are downloaded automatically within the notebooks via `nltk.download()` and `gensim.downloader`. No manual dataset download is required unless a notebook specifies otherwise.

## Notebooks

- **NLP_Tokenization_Basics.ipynb** — Covers word and sentence tokenization, stopword removal, and exploring the Gutenberg corpus using NLTK, with edge cases like abbreviations and punctuation handling.

- **NLP_Stemming_Lemmatization_POS.ipynb** — Demonstrates stemming and lemmatization to reduce words to root forms, along with Part-of-Speech tagging to identify grammatical roles of words in a sentence.

- **NLP_WordEmbeddings_Gensim.ipynb** — Explores Gensim for building Bag-of-Words and TF-IDF models, generating bigrams/trigrams, and training Word2Vec and Doc2Vec models for word/document embeddings.

- **NLP_BoW_Ngrams.ipynb** — Implements stopword removal, Bag-of-Words representation using frequency distribution, and generates unigrams, bigrams, and trigrams from sample text.

- **NLP_NamedEntityRecognition.ipynb** — Uses NLTK's POS tagging and chunking to perform Named Entity Recognition, identifying entities like persons and locations in text.

- **NLP_TextToSpeech_SpeechRecognition.ipynb** — Converts text to speech in multiple languages (English, Hindi, Marathi) using gTTS, and performs speech-to-text recognition using the SpeechRecognition library.

- **NLP_IBMWatson_SpeechServices.ipynb** — Uses IBM Watson's Speech-to-Text and Text-to-Speech APIs for voice processing tasks.

- **NLP_RuleBased_Translation.ipynb** — A simple rule-based English-to-German translator using a predefined dictionary mapping and word tokenization.

- **NLP_TextSummarization.ipynb** — Implements both extractive summarization (TF-IDF sentence scoring) and abstractive-style summarization using the Sumy library's LSA summarizer.

- **NLP_SentimentAnalysis.ipynb** — Performs sentiment analysis on text samples using NLTK's VADER sentiment intensity analyzer, classifying text as positive, negative, or neutral.

## Requirements

```bash
pip install nltk gensim sumy gtts SpeechRecognition pyaudio ibm-watson ibm-cloud-sdk-core
```
