# E-Commerce Sentiment Engine

<div align="center">

# 🧠 E-Commerce Sentiment Engine

Machine Learning-based sentiment analysis system for Indonesian e-commerce reviews using TF-IDF and Linear Support Vector Machine (SVM).

</div>

---

## 📖 Overview

E-Commerce Sentiment Engine is a Natural Language Processing (NLP) project developed to classify Indonesian e-commerce product reviews into:

- Positive
- Neutral
- Negative

The project focuses on building and evaluating multiple machine learning models to determine the most effective approach for sentiment classification.

---

## 🎯 Objectives

The objectives of this project are:

- Analyze customer sentiment from e-commerce reviews
- Compare multiple machine learning algorithms
- Evaluate classification performance
- Build a reusable sentiment classification engine

---

## 📊 Dataset

Source:

- Kaggle E-Commerce Review Dataset

Characteristics:

| Feature | Value |
|----------|----------|
| Total Reviews | ~40,000 |
| Language | Indonesian |
| Product Categories | Multiple |
| Missing Values | None |

---

## 🏷 Labeling Method

### Lexicon Combine Labeling

This project uses a Lexicon Combine Labeling approach.

Instead of manually labeling every review, sentiment labels are generated through lexicon-based sentiment scoring and rule-based aggregation.

Final classes:

- Negative (0)
- Neutral (1)
- Positive (2)

---

## 🧹 Text Preprocessing

The preprocessing pipeline consists of:

- Lowercasing
- URL Removal
- Symbol Removal
- Special Character Removal
- Regex Cleaning
- Whitespace Normalization

Example:

Input:

```text
Barang BAGUS!!! 🤩
```

Output:

```text
barang bagus
```

---

## 🔠 Feature Extraction

### TF-IDF Vectorizer

The project uses TF-IDF (Term Frequency – Inverse Document Frequency) to convert text into numerical vectors.

Advantages:

- Highlights important terms
- Reduces influence of common words
- Effective for text classification

---

## 🤖 Models Evaluated

Four machine learning models were evaluated.

| Model | Accuracy |
|---------|---------|
| Naive Bayes | 75.70% |
| Random Forest | 93.62% |
| Logistic Regression | 94.06% |
| Linear SVM | 94.92% |

---

## 🏆 Best Model

### Linear Support Vector Machine (SVM)

Final selected model:

```text
LinearSVC
```

Performance:

```text
Accuracy: 94.92%
```

Reasons:

- Highest accuracy
- Excellent performance on sparse text data
- Fast inference time
- Strong generalization capability

---

## 📈 Evaluation Metrics

The following metrics were used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📂 Repository Structure

```text
.
├── training.ipynb
├── svm_model.pkl
├── tfidf_vectorizer.pkl
├── dataset/
├── notebooks/
└── README.md
```

---

## 🛠 Technologies

- Python
- Pandas
- NumPy
- Scikit-Learn
- TF-IDF
- Linear SVM
- Matplotlib
- Seaborn

---

## 🔮 Future Work

Potential improvements:

- IndoBERT
- Transformer Models
- Aspect-Based Sentiment Analysis
- Sarcasm Detection
- Larger Dataset

---

## 👨‍💻 Authors

- Alif Agil
- Ahmad Rizki Wardana
- Muadz

---

## 📄 Academic Purpose

This project was developed as part of a Natural Language Processing (NLP) coursework project.
