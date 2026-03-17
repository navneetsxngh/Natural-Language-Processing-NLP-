# 🧠 Natural Language Processing (NLP)

> 🚧 **Work in Progress** — This repository is actively being developed. New notebooks, datasets, and topics will be added as learning progresses. Stay tuned for updates!

A structured, beginner-to-intermediate collection of Jupyter Notebooks covering the core concepts and techniques of **Natural Language Processing (NLP)** using Python. Each notebook is hands-on and progressively builds knowledge — from raw text processing and feature extraction to real-world classification projects.

---

## 📁 Repository Structure

```
Natural-Language-Processing-NLP-/
│
├── Data/
│   ├── IMDB Dataset.csv            # 50K movie reviews for sentiment analysis
│   ├── SMSSpamCollection.txt       # Labelled SMS spam/ham messages
│   ├── all_kindle_review.csv       # Kindle product reviews for sentiment analysis
│   ├── train.csv                   # General training dataset
│   └── nlp_pipeline_notes.pdf      # Reference notes on NLP pipelines
│
├── tokenization.ipynb              # Word & sentence tokenization
├── stemming and lemmatization.ipynb # Stemming & lemmatization methods
├── Stopwords.ipynb                 # Removing stopwords from text
├── Parts of Speech Tagging.ipynb   # POS tagging using NLTK
├── Named Entity Recognition.ipynb  # NER with NLTK
├── Text Preprocessing.ipynb        # Full text preprocessing pipeline
├── Text Representation.ipynb       # Conceptual overview of text features
├── Bag of Words.ipynb              # BoW with CountVectorizer
├── TF-IDF.ipynb                    # TF-IDF with TfidfVectorizer
├── N-Grams.ipynb                   # N-gram language models
├── Word2Vec.ipynb                  # Word embeddings with Gensim
│
├── Projects/
│   ├── Kindle Review Sentiment Analysis.ipynb
│   ├── Spam Ham Classification Project Using BOW.ipynb
│   ├── Spam Ham Classification Project Using TF-IDF.ipynb
│   └── Spam Ham Projects Using Word2vec,AvgWord2vec.ipynb
│
└── requirements.txt                # Python dependencies
```

---

## 📓 Notebooks Overview

### 1. 🔤 Tokenization (`tokenization.ipynb`)
Covers the process of breaking text into smaller units (tokens):
- Word tokenization using Python's `split()` function
- Sentence tokenization
- Limitations of basic tokenization
- Advanced tokenization using **NLTK** (`word_tokenize`, `sent_tokenize`)

### 2. 🌱 Stemming & Lemmatization (`stemming and lemmatization.ipynb`)
Explores techniques to reduce words to their base or root forms:
- **PorterStemmer** — aggressive but fast stemming
- **SnowballStemmer** — improved multilingual stemmer
- **WordNetLemmatizer** — context-aware lemmatization
- Comparison between stemming and lemmatization with practical examples

### 3. 🚫 Stopwords (`Stopwords.ipynb`)
Demonstrates how to remove common, low-information words from text:
- Using `nltk.corpus.stopwords` for English and other languages
- Applied on a real-world text (APJ Abdul Kalam's speech)
- Integration with stemming for a combined preprocessing step

### 4. 🏷️ Parts of Speech Tagging (`Parts of Speech Tagging.ipynb`)
Covers grammatical tagging of words in a sentence:
- POS tagging using `nltk.pos_tag`
- Applied on Dr. APJ Abdul Kalam's speech as sample text
- Using the `averaged_perceptron_tagger` model from NLTK

### 5. 🔍 Named Entity Recognition (`Named Entity Recognition.ipynb`)
Identifies and classifies named entities (persons, places, organizations) in text:
- NER using NLTK's `ne_chunk`
- Extracting persons, GPE, and organizations from sample text

### 6. 🧹 Text Preprocessing (`Text Preprocessing.ipynb`)
A full preprocessing pipeline applied on the **IMDB Movie Reviews Dataset**:
- Lowercasing, removing special characters, HTML tags, URLs
- Handling contractions and punctuation
- Combining tokenization, stopword removal, and stemming

### 7. 🔢 Text Representation (`Text Representation.ipynb`)
Conceptual overview of techniques to convert text into numerical vectors:
- Bag of Words (BoW), TF-IDF, Word Embeddings, and N-grams
- Why feature extraction matters for ML models (Logistic Regression, SVM, etc.)

### 8. 🛍️ Bag of Words (`Bag of Words.ipynb`)
Hands-on implementation of the BoW model:
- `CountVectorizer` from scikit-learn
- Building and interpreting a document-term matrix
- Applied on real review data

### 9. 📊 TF-IDF (`TF-IDF.ipynb`)
In-depth implementation of TF-IDF vectorization:
- `TfidfVectorizer` from scikit-learn
- Understanding term frequency vs. inverse document frequency
- Comparison with BoW

### 10. 🔗 N-Grams (`N-Grams.ipynb`)
Explores n-gram language models:
- Unigrams, bigrams, trigrams
- Generating n-grams with NLTK
- Applications in text prediction and feature engineering

### 11. 🧬 Word2Vec (`Word2Vec.ipynb`)
Word embedding models using neural networks:
- Training Word2Vec using **Gensim**
- CBOW and Skip-gram model architectures
- Finding similar words and exploring word relationships

---

## 🗂️ Projects

End-to-end classification projects applying all the NLP techniques learned above.

### 📧 Spam/Ham Classification — BOW (`Spam Ham Classification Project Using BOW.ipynb`)
Binary text classification using the **SMS Spam Collection** dataset:
- Preprocessing pipeline (cleaning, tokenization, stopword removal)
- Feature extraction using **Bag of Words** (CountVectorizer)
- Model training and evaluation (Naive Bayes, Logistic Regression)

### 📧 Spam/Ham Classification — TF-IDF (`Spam Ham Classification Project Using TF-IDF.ipynb`)
Same classification task with a different feature extraction strategy:
- Feature extraction using **TF-IDF**
- Comparison of model performance vs. BoW approach

### 📧 Spam/Ham Classification — Word2Vec (`Spam Ham Projects Using Word2vec,AvgWord2vec.ipynb`)
Classification using dense word vector representations:
- Using pre-trained **Word2Vec** and **Average Word2Vec** features
- Demonstrates the advantage of semantic word embeddings over sparse features

### 📚 Kindle Review Sentiment Analysis (`Kindle Review Sentiment Analysis.ipynb`)
End-to-end sentiment classification on the **Kindle Reviews** dataset:
- Full NLP pipeline from raw text to trained classifier
- Explores multiple vectorization strategies
- Multi-model comparison and evaluation

---

## 🗂️ Datasets

| File | Description |
|------|-------------|
| `IMDB Dataset.csv` | 50,000 movie reviews labelled positive/negative |
| `SMSSpamCollection.txt` | Labelled SMS messages for spam/ham classification |
| `all_kindle_review.csv` | Kindle product reviews for sentiment analysis |
| `train.csv` | Additional training data used in preprocessing exercises |
| `nlp_pipeline_notes.pdf` | Supplementary reference notes on the NLP pipeline |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `nltk` | Core NLP — tokenization, stemming, POS tagging, NER, stopwords |
| `spacy` | Advanced NLP processing |
| `scikit-learn` | Feature extraction (`CountVectorizer`, `TfidfVectorizer`) and ML models |
| `gensim` | Word2Vec and word embedding models |
| `textblob` | Simple NLP API for text processing |
| `beautifulsoup4` | HTML parsing and cleaning |
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` & `seaborn` | Visualization |
| `emoji` | Handling emoji characters in text |

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/navneetsxngh/Natural-Language-Processing-NLP-.git
   cd Natural-Language-Processing-NLP-
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download required NLTK data**
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('maxent_ne_chunker')
   nltk.download('words')
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

5. Open any `.ipynb` file and run the cells sequentially.

---

## 🚀 Recommended Learning Order

For the best learning experience, follow this order:

```
Core Concepts
1. tokenization.ipynb
2. stemming and lemmatization.ipynb
3. Stopwords.ipynb
4. Parts of Speech Tagging.ipynb
5. Named Entity Recognition.ipynb
6. Text Preprocessing.ipynb

Feature Extraction
7. Text Representation.ipynb        ← conceptual overview
8. Bag of Words.ipynb
9. TF-IDF.ipynb
10. N-Grams.ipynb
11. Word2Vec.ipynb

Projects (apply everything)
12. Spam Ham Classification Project Using BOW.ipynb
13. Spam Ham Classification Project Using TF-IDF.ipynb
14. Spam Ham Projects Using Word2vec,AvgWord2vec.ipynb
15. Kindle Review Sentiment Analysis.ipynb
```

---

## 🗺️ Upcoming Topics

- [ ] Text Classification (multi-class)
- [ ] Sequence Models (RNN, LSTM)
- [ ] Transformers & BERT
- [ ] Topic Modelling (LDA)
- [ ] Text Summarization
- [ ] Question Answering

> 💡 Have a suggestion? Feel free to open an issue!

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve existing notebooks or add new NLP topics:

1. Fork this repository
2. Create a new branch (`git checkout -b feature/your-topic`)
3. Commit your changes (`git commit -m 'Add: your topic'`)
4. Push to the branch (`git push origin feature/your-topic`)
5. Open a Pull Request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Navneet Singh**
- GitHub: [@navneetsxngh](https://github.com/navneetsxngh)

---

> ⭐ If you found this repository helpful, consider giving it a star!
