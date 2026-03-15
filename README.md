# 🧠 Natural Language Processing (NLP)

> 🚧 **Work in Progress** — This repository is actively being developed. New notebooks, datasets, and topics will be added as learning progresses. Stay tuned for updates!

A structured, beginner-to-intermediate collection of Jupyter Notebooks covering the core concepts and techniques of **Natural Language Processing (NLP)** using Python. Each notebook is hands-on and progressively builds up knowledge from raw text processing to feature extraction for machine learning.

---

## 📁 Repository Structure

```
Natural-Language-Processing-NLP-/
│
├── Data/
│   ├── IMDB Dataset.csv          # Movie reviews dataset for sentiment analysis
│   ├── train.csv                 # Training dataset
│   └── nlp_pipeline_notes.pdf   # Reference notes on NLP pipelines
│
├── tokenization.ipynb            # Word & sentence tokenization techniques
├── stemming and lemmatization.ipynb  # Stemming & lemmatization methods
├── Stopwords.ipynb               # Removing stopwords from text
├── Parts of Speech Tagging.ipynb # POS tagging using NLTK
├── Text Preprocessing.ipynb      # Full text preprocessing pipeline
├── Text Representation.ipynb     # Feature extraction (BoW, TF-IDF, Embeddings)
│
└── requirements.txt              # Python dependencies
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
- Named Entity Recognition (NER) with `ne_chunk`
- Applied on Dr. APJ Abdul Kalam's speech as sample text
- Using the `averaged_perceptron_tagger` model from NLTK

### 5. 🧹 Text Preprocessing (`Text Preprocessing.ipynb`)
A full preprocessing pipeline applied on the **IMDB Movie Reviews Dataset**:
- Lowercasing text
- Removing special characters, HTML tags, URLs
- Handling contractions and punctuation
- Combining tokenization, stopword removal, and stemming

### 6. 🔢 Text Representation (`Text Representation.ipynb`)
Feature extraction techniques to convert text into numerical vectors:
- **Bag of Words (BoW)** using `CountVectorizer`
- **TF-IDF** (Term Frequency–Inverse Document Frequency)
- **Word Embeddings** (Word2Vec, GloVe conceptual overview)
- **N-grams** for capturing word sequences
- Why feature extraction matters for ML models (Logistic Regression, SVM, etc.)

---

## 🗂️ Datasets

| File | Description |
|------|-------------|
| `IMDB Dataset.csv` | 50,000 movie reviews labeled as positive/negative for sentiment analysis |
| `train.csv` | Additional training data used in preprocessing exercises |
| `nlp_pipeline_notes.pdf` | Supplementary reference notes on the NLP pipeline |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `nltk` | Core NLP tasks — tokenization, stemming, POS tagging, stopwords |
| `spacy` | Advanced NLP processing |
| `scikit-learn` | Feature extraction (CountVectorizer, TfidfVectorizer) |
| `textblob` | Simple NLP API for text processing |
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

For the best learning experience, follow the notebooks in this order:

```
1. tokenization.ipynb
2. stemming and lemmatization.ipynb
3. Stopwords.ipynb
4. Parts of Speech Tagging.ipynb
5. Text Preprocessing.ipynb
6. Text Representation.ipynb
```

---

## 🗺️ Upcoming Topics

The following topics are planned for future notebooks:

- [ ] Named Entity Recognition (NER)
- [ ] Text Classification
- [ ] Sentiment Analysis (end-to-end)
- [ ] Word Embeddings (Word2Vec, GloVe, FastText)
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
