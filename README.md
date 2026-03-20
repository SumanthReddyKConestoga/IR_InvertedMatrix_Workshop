# IR Inverted Matrix Workshop

## PROG8245 – Active Learning Workshop  
### Implementing an Inverted Matrix (Jupyter + GitHub Edition)

This repository contains our team submission for the **Inverted Matrix / Inverted Index Workshop**.  
The notebook demonstrates how a small information retrieval pipeline is built step by step using Python, Jupyter Notebook, and GitHub collaboration.

---

## Project Overview

The purpose of this workshop is to build a mini **Information Retrieval (IR)** system that can:

- collect and load text documents
- tokenize raw text into words
- normalize text using stop-word removal and stemming
- build an **inverted index**
- extend it into a **positional index**
- support **phrase queries**
- explain **TF, IDF, and TF-IDF**
- compare **positional indexing** with a **term-document count matrix**

In simple terms, this notebook shows how a search engine can organize text documents so that keyword and phrase searches become fast and accurate.

---

## Repository Contents

- `IR_InvertedMatrix_Workshop.ipynb` → Main workshop notebook
- `README.md` → Project explanation and submission details
- `requirements.txt` → Python libraries required to run the notebook
- `sample_docs_exec/` → Folder containing downloaded or fallback text documents used in the corpus

---

## Workshop Tasks Covered

The notebook includes the following major steps:

### 1. Document Collection
- Loads at least 20 text documents
- Builds a corpus for indexing
- Verifies vocabulary diversity

### 2. Tokenizer Implementation
- Converts text into lowercase tokens
- Removes punctuation using regex-based tokenization

### 3. Normalization Pipeline
- Removes stop words
- Applies stemming using `PorterStemmer`
- Produces cleaner and more consistent searchable terms

### 4. Inverted Index
- Maps each term to the list of document IDs where it appears

### 5. Positional Index
- Stores exact term positions in documents
- Supports phrase query matching

### 6. Phrase Query Testing
- Tests at least 2 phrase queries
- Verifies exact word order and adjacency

### 7. TF, IDF, and TF-IDF Discussion
- Explains local and global term importance
- Shows how search relevance can be improved

---

## Dataset Description

The notebook uses a corpus of text documents collected from:

- **Python Software Foundation RSS feed**, or
- a **fallback local corpus** generated from Python standard-library documentation when RSS is unavailable

This fallback design ensures the notebook can still run in offline or restricted lab environments.

### Corpus Characteristics
- 20+ documents
- 2000+ unique words
- text-based content suitable for indexing and phrase search

---

## Why This Project Matters

This assignment represents a complete mini search pipeline.

It helps us understand:

- how raw text is transformed into searchable data
- why preprocessing matters in NLP
- how an inverted index improves search efficiency
- why a positional index is needed for phrase search
- how TF-IDF helps in ranking and relevance

These same ideas are used in:

- search engines
- enterprise search systems
- document retrieval platforms
- legal and academic search
- AI assistants and RAG pipelines

---

## Key Concepts Used

- Information Retrieval (IR)
- Inverted Index
- Positional Index
- Tokenization
- Normalization
- Stop Word Removal
- Stemming
- Phrase Queries
- Term Frequency (TF)
- Inverse Document Frequency (IDF)
- TF-IDF

---

## Tools and Technologies

- Python
- Jupyter Notebook
- GitHub
- `feedparser`
- `nltk`
- `pandas`
- `matplotlib`

---

## Installation

Install the required packages using:

```bash
pip install -r requirements.txt
````

---

## How to Run

1. Clone this repository
2. Open the project folder
3. Install dependencies from `requirements.txt`
4. Launch Jupyter Notebook
5. Open `IR_InvertedMatrix_Workshop.ipynb`
6. Run the notebook cells in order

---

## Team Members

Add your actual team member names below:

* Sumanth Reddy
* Muthuraj
* Lohith Reddy

---

## GitHub Repository Link

Add your final public GitHub repository link here:

`[Paste your GitHub repo link here]`

---

## Talking Points Included

This notebook includes discussion-ready talking points on:

* why document collection matters
* how tokenization converts text into machine-readable units
* why normalization improves search quality
* why inverted indexes are faster than naive search
* why positional indexes are better for bigram and phrase search
* how TF and IDF contribute to search relevance

---

## Main Conclusion

For searching **bigrams** or **exact phrases**, a **positional index** is the better choice because it stores the exact positions of terms in each document.

A term-document count matrix can tell us how often a term appears, but it cannot confirm whether two words appear **next to each other and in the correct order**.

That is why positional indexing is more suitable for phrase-based retrieval.

---


### Data Source

* Python Software Foundation Blog RSS Feed
* Python Standard Library Documentation (fallback corpus)


## Submission Note

This repository was created as part of the **PROG8245 Inverted Matrix Workshop** submission.
The notebook includes markdown explanations, code implementation, phrase query demonstrations, and retrieval analysis as required in the workshop instructions.

````

