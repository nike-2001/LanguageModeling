# Language Modeling with N-gram and Neural Networks

**Author**: Venkata Nikhil Chakravarthy Korrapati  
**Project Title**: Exploring Traditional and Neural Language Models  

## 📄 Overview

This project explores building and evaluating language models using both classic n-gram techniques and modern neural networks. The goal was to understand the strengths and limitations of each approach and apply regularization techniques to improve performance on a relatively small dataset.

## 🛠️ What I Built

I implemented and evaluated the following models:

- **Unigram Language Model** – basic word-level generation
- **Bigram Model** – predicts based on previous word
- **Trigram Backoff Model** – uses backoff smoothing for better predictions
- **Neural Trigram Model** – a simple feedforward network with embeddings
- **LSTM Language Model** – recurrent model for sequential data
- **Improved LSTM** – enhanced with multiple regularization techniques and learning rate scheduling

## 🔍 Key Improvements

To enhance the LSTM model's performance and generalization, I applied:

- **Weight Dropout** – applies dropout on LSTM weight matrices  
- **Embedding Dropout** – randomly drops word embeddings during training  
- **Gradient Clipping** – prevents exploding gradients in LSTMs  
- **Learning Rate Scheduler** – automatically reduces learning rate on plateaus

These changes helped reduce overfitting and made the training more stable.

## 📊 Results (Validation Perplexity)

| Model              | Perplexity |
|-------------------|------------|
| Bigram            | 635.62     |
| Trigram Backoff   | 310.73     |
| Neural Trigram    | 237.67     |
| LSTM              | 166.71     |
| **Improved LSTM** | **144.31** |

## 🧪 Highlights

- Learned how to implement backoff smoothing and calculate perplexity
- Applied deep learning best practices (dropout, scheduling, clipping) to improve LSTM training
- Compared model performance using perplexity as the metric
- Built everything in Python using PyTorch and trained models in Google Colab

## 📁 Files Included

- `proj1.ipynb` – the complete notebook with all experiments and code  
- Model predictions (`*.npy` files) for evaluation:
  - `bigram_predictions.npy`
  - `trigram_backoff_predictions.npy`
  - `neural_trigram_predictions.npy`
  - `lstm_predictions.npy`

---

This project was a great hands-on experience with both traditional NLP techniques and modern deep learning models for language modeling.
