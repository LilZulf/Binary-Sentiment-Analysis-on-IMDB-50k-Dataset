# Binary-Sentiment-Analysis-on-IMDB-50k-Dataset

This project performs **binary sentiment classification** (positive or negative) on the **IMDB 50K Movie Reviews Dataset** using a deep learning model based on **LSTM (Long Short-Term Memory)** neural networks.

## 🔍 Objective

To build a neural network model that can predict the sentiment of a movie review based on its text content using sequence modeling techniques.

---

## 📁 Dataset

- **Source**: [IMDB 50k Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)
- **Format**: CSV file with two columns:
  - `review`: The text of the review.
  - `sentiment`: Either `positive` or `negative`.

---

## 🧪 Methodology

### 1. Course of Action

- Load and inspect the dataset from Google Drive.
- Preprocess text using tokenization and padding.
- Build and train an LSTM model.
- Evaluate performance using accuracy, F1-score, and learning curves.
- Optionally: experiment with other models (GRU, CNN) and hyperparameters.

### 2. Preprocessing

- **Label Encoding**: Sentiments mapped to binary labels (positive = 1, negative = 0).
- **Tokenization**: Using Keras `Tokenizer`, vocabulary limited to top 10,000 words.
- **Padding**: All reviews padded or truncated to 500 tokens.

### 3. Model Architecture

```text
Embedding Layer (10000 vocab, 128 dim)
↓
LSTM Layer (64 units)
↓
Dense Output (Sigmoid)
↓
Lost Funtion (Binary Crossentropy)
↓
Optimizer (Adam)
↓
Metrics (Accuracy)
```

