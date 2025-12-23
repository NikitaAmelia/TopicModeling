# 📚 NLP Topic Modeling Project

This repository contains a **Natural Language Processing (NLP) Topic Modeling project** aimed at discovering hidden thematic structures in large text corpora. The project explores and compares multiple **classical and modern topic modeling techniques** to extract meaningful insights from textual data.

---

## 🚀 Project Overview

Topic modeling is an **unsupervised machine learning technique** used to identify latent topics within a collection of documents.
In this project, several topic modeling approaches are implemented and evaluated to analyze their effectiveness in extracting interpretable topics from **news articles**.

---

## 🧠 Models Implemented

The following topic modeling methods are implemented and compared:

* **Latent Semantic Analysis (LSA)**
* **Latent Dirichlet Allocation (LDA)**
* **Non-negative Matrix Factorization (NMF)**
* **BERTopic** (Transformer-based topic modeling)

Each model is evaluated using **topic coherence scores** and **qualitative topic interpretation**.

---

## 📂 Project Structure

```
├── NLP_TopicModeling_Final.ipynb   # Main notebook: preprocessing, modeling, evaluation
├── dataset/                        # Dataset directory (not included in repository)
└── README.md                       # Project documentation
```

> ⚠️ **Note:** The dataset is not included in this repository due to GitHub size limitations.

---

## 📊 Dataset

The dataset used in this project is publicly available on Kaggle:

🔗 [https://www.kaggle.com/datasets/sh1zuka/indonesia-news-dataset-2024](https://www.kaggle.com/datasets/sh1zuka/indonesia-news-dataset-2024)

Please download the dataset and place it inside the `dataset/` directory before running the notebook.

---

## 🔍 Workflow

### 1. Data Loading

* Load the news article dataset

### 2. Text Preprocessing

* Case folding
* Tokenization
* Stopword removal (Indonesian & English)
* Lemmatization
* Bigram & Trigram modeling

### 3. Feature Extraction

* Bag of Words (BoW)
* TF-IDF

### 4. Topic Modeling

* LSA using TF-IDF
* LDA using Bag of Words
* NMF using TF-IDF
* BERTopic using transformer-based embeddings

### 5. Evaluation

* Topic coherence score
* Topic interpretability analysis

### 6. Visualization

* Topic-word distributions
* Coherence score comparison across models

---

## 📈 Evaluation Metric

### Topic Coherence Score

Measures the semantic similarity between words within a topic and helps assess the **quality and interpretability** of generated topics.

---

## 🛠️ Technologies & Libraries

* **Python 3.x**
* Pandas
* NumPy
* Gensim
* Scikit-learn
* NLTK
* BERTopic
* Sentence-Transformers
* Matplotlib

---

## ▶️ How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/nlp-topic-modeling.git
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open and run the notebook:

   ```bash
   jupyter notebook NLP_TopicModeling_Final.ipynb
   ```

---

## 📌 Key Findings

* **LSA** is computationally efficient but may produce less interpretable topics.
* **LDA** generates probabilistic topics with good interpretability when properly tuned.
* **NMF** produces more coherent and distinct topics when applied to TF-IDF features.
* **BERTopic** achieves higher-quality topics by leveraging contextual embeddings from transformer models.

---

## 🎯 Future Improvements

* Hyperparameter tuning for LDA, NMF, and BERTopic
* Interactive topic visualization
* Model comparison dashboard (Streamlit / Power BI)
* Multi-language topic modeling support

