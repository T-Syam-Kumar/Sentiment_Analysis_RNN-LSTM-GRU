# IMDB Movie Review Sentiment Analysis using RNN, LSTM, and GRU

This project implements **Sentiment Analysis on the IMDB Movie Review dataset** using three different **Recurrent Neural Network architectures**:

* Simple RNN
* LSTM (Long Short-Term Memory)
* GRU (Gated Recurrent Unit)

The models are built using **TensorFlow and Keras** to classify movie reviews as **positive or negative**.

---

# Project Overview

Sentiment analysis is a Natural Language Processing (NLP) task used to determine whether a piece of text expresses a **positive or negative opinion**.

In this project:

1. The **IMDB dataset** is loaded from TensorFlow.
2. Reviews are converted into **integer sequences**.
3. Sequences are padded to a fixed length.
4. Three deep learning models are trained:

   * **Simple RNN**
   * **LSTM**
   * **GRU**
5. Each model predicts whether a review is **positive or negative**.

---

# Models Implemented

## Simple RNN Model

Architecture:

Input Review
    ↓
Embedding Layer
    ↓
SimpleRNN Layer
    ↓
Dense Output Layer (Sigmoid)

Simple RNN captures **basic sequential patterns** in text.

However, it may struggle with **long-term dependencies**.

---

## LSTM Model

Architecture:

Input Review
    ↓
Embedding Layer
    ↓
LSTM Layer
    ↓
Dense Output Layer

LSTM solves the **vanishing gradient problem** of RNN and remembers **long-term dependencies in sequences**.

This makes it more effective for **text and language tasks**.

---

## GRU Model

Architecture:

Input Review
    ↓
Embedding Layer
    ↓
GRU Layer
    ↓
Dense Output Layer

GRU is a **simplified version of LSTM** with fewer parameters.

Advantages:

* Faster training
* Comparable performance to LSTM
* Efficient memory usage

---

# Dataset

This project uses the **IMDB Movie Review Dataset** from TensorFlow.

Dataset details:

| Feature           | Value                   |
| ----------------- | ----------------------- |
| Total Reviews     | 50,000                  |
| Training Reviews  | 25,000                  |
| Testing Reviews   | 25,000                  |
| Sentiment Classes | 2 (Positive / Negative) |

Labels:

| Label | Meaning         |
| ----- | --------------- |
| 0     | Negative Review |
| 1     | Positive Review |

Only the **10,000 most frequent words** are used to reduce model complexity.

---

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Natural Language Processing (NLP)

---

# Model Training Configuration

| Parameter           | Value               |
| ------------------- | ------------------- |
| Vocabulary Size     | 10,000              |
| Sequence Length     | 200                 |
| Embedding Dimension | 32 / 64             |
| Batch Size          | 64                  |
| Epochs              | 5                   |
| Loss Function       | Binary Crossentropy |
| Optimizer           | Adam                |

---

# Expected Performance

Typical accuracy values:

| Model      | Accuracy |
| ---------- | -------- |
| Simple RNN | ~82%     |
| LSTM       | ~86–88%  |
| GRU        | ~86–88%  |

LSTM and GRU generally perform **better than Simple RNN**.

---

# Learning Outcomes

This project demonstrates:

* Text preprocessing
* Sequence padding
* Word embeddings
* Recurrent Neural Networks
* LSTM architecture
* GRU architecture
* Binary text classification using deep learning

---

# Future Improvements

Possible improvements include:

* Using **Bidirectional LSTM**
* Adding **Dropout layers**
* Using **pretrained embeddings (GloVe / Word2Vec)**
* Implementing **Attention mechanisms**
* Deploying the model using **Streamlit**

---

# Author

**Syam Kumar**

If you found this project useful, consider **starring ⭐ the repository**.

---

# 📄 License

This project is licensed under the **MIT License**.
