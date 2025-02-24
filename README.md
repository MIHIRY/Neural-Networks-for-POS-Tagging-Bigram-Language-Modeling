# 📌 Neural Networks for POS Tagging & Bigram Language Modeling

## 📖 Overview
This project implements **Part-of-Speech (POS) tagging using neural networks** and **Bigram Language Models** to explore natural language processing techniques. The project consists of:
- Training **feed-forward neural networks** for **POS tagging on English tweets**
- Using **feature engineering, pretrained word embeddings**, and **architectural variations** to improve accuracy
- Implementing **Bidirectional RNNs (LSTM/GRU/BiLSTM)** for sequence modeling
- Developing **Bigram Language Models** with and without smoothing to analyze their probabilistic behavior

---

---

## 🛠 Methodology
### 1️⃣ POS Tagging Using Neural Networks
- **Baseline Model:** A **feed-forward neural network** trained on annotated Twitter data
- **Feature Engineering:** Additional **syntactic and lexical features** to improve performance
- **Pretrained Embeddings:** Incorporating **word2vec-based Twitter embeddings**
- **Architecture Engineering:** Comparing **hidden layers, activation functions, and wider layers**
- **Bidirectional RNNs:** Implementing **RNN, LSTM, GRU, and BiLSTM** for sequence modeling

### 2️⃣ Bigram Language Modeling
- **Unsmoothed Bigram Model (Model U):** Estimates probabilities based on raw frequency counts
- **Smoothed Bigram Model (Model S):** Uses **add-one smoothing** to handle unseen bigrams
- **Comparison:** Demonstrates **cases where smoothing improves probability estimation**

---

## 📊 Experimental Results
- **POS Tagging Performance:**
  - **Baseline accuracy:** 79.2% (w=0) → 82.4% (w=1)
  - **Feature Engineering:** Improved accuracy by **~2%**
  - **Pretrained Embeddings:** Further improvement to **88.88%**
  - **Deep Architectures:** **Two hidden layers (512 units each) with Tanh** achieved **89.31% accuracy**
  - **Bidirectional RNNs:** **BiLSTM achieved the best performance at 78.62%**

- **Bigram Language Model:**
  - **Model U (Unsmoothed):** Assigns zero probability to unseen bigrams
  - **Model S (Smoothed):** Assigns higher probability to rare sequences
  - **Comparison:** Identifies cases where **Model S > Model U**

---


