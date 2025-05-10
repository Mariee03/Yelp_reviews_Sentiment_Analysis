# Yelp Reviews Sentiment Analysis – NLP for Review Classification 📢🍴

This project uses natural language processing (NLP) to classify Yelp reviews as **positive** or **negative**. It focuses on cleaning and vectorizing review text and evaluating several machine learning models for sentiment classification.

> Project by: Marie Elyse Bassil

---

## 🎯 Objective

Automatically classify user-written Yelp reviews into positive or negative sentiment, using the associated text and a supervised machine learning pipeline.

---

## 🗂️ Dataset Overview

- `yelp.csv` contains:
  - `text`: Full written review
  - `stars`: Rating from 1 to 5 stars

### 📌 Labeling Rule
- Reviews with **4 or 5 stars** → labeled **positive**
- Reviews with **1 or 2 stars** → labeled **negative**
- **3-star reviews are excluded** to remove ambiguity

---

## 🔍 Pipeline Summary

### 1. Preprocessing
- Lowercasing
- Punctuation removal
- Tokenization
- Stopword removal using NLTK

### 2. Feature Engineering
- **TF-IDF vectorization** to transform reviews into numerical vectors

### 3. Model Training
Tested multiple classifiers:
- Logistic Regression ✅ best performing
- Multinomial Naive Bayes
- Random Forest
- Support Vector Machine (SVM)

### 4. Evaluation Metrics
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

---

## 📈 Results

- **Logistic Regression** outperformed all other models
- Achieved accuracy of **~92%** on validation set
- TF-IDF provided strong signal for separating sentiment classes

---

## 🚀 How to Run

1. Clone this repository:
```bash
git clone https://github.com/Mariee03/Yelp_reviews_Sentiment_Analysis.git
cd Yelp_reviews_Sentiment_Analysis
```
2. Install requirements:
```bash
pip install -r requirements.txt
```
3. Open the notebook:
```bash
jupyter notebook SAYR_yelp_reviews.ipynb
```

## 📬 Author

Created by Marie Elyse Bassil
Feel free to explore, fork, or connect!
