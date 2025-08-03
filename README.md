# 🧠 Arabic Sentiment Analysis with Machine Learning (No Transformers)

This project performs sentiment analysis on Arabic text using classic machine learning techniques (TF-IDF + Naive Bayes) without relying on deep learning or transformer models like AraBERT. It includes full Arabic preprocessing, model training, evaluation, and word cloud visualizations.

---

## 📌 Features

- Arabic text normalization (diacritics, elongation, unwanted characters)
- Arabic stopword removal
- TF-IDF vectorization
- Naive Bayes classifier
- Evaluation: accuracy, classification report, confusion matrix
- WordClouds for both positive and negative sentiment

---

## 🗃️ Dataset

Replace the sample data with your own CSV or dataset containing:

| text                              | label     |
|-----------------------------------|-----------|
| البرنامج ممتاز وسهل الاستخدام     | positive  |
| تطبيق فاشل جدا ولا يستحق التحميل | negative  |

---

## ⚙️ Preprocessing Techniques

- Normalize Arabic letters (e.g. "أ" → "ا")
- Remove diacritics and tashkeel
- Handle repeated character elongation (e.g. "جمييييل" → "جمييل")
- Remove non-Arabic characters and digits
- Remove common Arabic stopwords

---

## 📊 Model Used

- **TF-IDF Vectorizer** from `scikit-learn`
- **Multinomial Naive Bayes (MNB)** for classification

---

## 📈 Visualizations

- **Confusion Matrix**
- **Word Cloud** for:
  - Positive Sentiment
  - Negative Sentiment

---

## 🛠️ Requirements

Install required libraries using pip:

```bash
pip install pyarabic wordcloud arabic_reshaper python-bidi scikit-learn matplotlib seaborn
