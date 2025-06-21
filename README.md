# Sentiment Analysis with LSTM on Movie Reviews

This project performs **sentiment analysis** on movie reviews using a **custom NLP pipeline** and a **Keras LSTM** model.

---

## 📁 Dataset

- File: `movie_reviews.csv`
- Columns:
  - `review` – Raw movie review text
  - `sentiment` – Binary label (`positive` or `negative`)



---

## 🧠 Model Architecture

- Embedding Layer
- SpatialDropout1D
- LSTM Layer
- Dense Output Layer (Sigmoid activation)

---

## 🧹 Preprocessing

1. **Text Cleaning**
   - Remove HTML tags
   - Remove non-alphabetic characters
   - Lowercasing
   - Stopword removal (`nltk.stopwords`)
2. **Tokenization**
   - Custom tokenization (splitting on space)
3. **Vocabulary Mapping**
   - Built from training data using `collections.Counter`
4. **Sequence Padding**
   - Manual `pad_sequences` from Keras

---

## 🔧 Model Details

- Embedding dimension: `128`
- LSTM units: `64`
- Dropout: `0.2`
- Batch size: `100`
- Epochs: `5`
- Loss: `binary_crossentropy`
- Optimizer: `adam`

---

## 🧪 Evaluation Metrics

After training, the model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---


