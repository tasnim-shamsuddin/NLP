# SMS Spam Classification using NLP

## 📌 Project Description
This project implements an **SMS Spam Classification system** using **Natural Language Processing (NLP)** techniques.  
The goal is to classify SMS messages as **Spam** or **Ham (Not Spam)** by converting raw text into meaningful numerical features and applying machine learning algorithms.

---

## 🧹 Data Cleaning & Text Preprocessing
Text preprocessing was performed using the **NLTK** library to improve model performance and reduce noise in the data.  
The following steps were applied:

- Conversion of text to lowercase
- Removal of punctuation and special characters
- Tokenization of text
- **Stopword removal** to eliminate commonly used but non-informative words
- **Stemming using Porter Stemmer** to reduce words to their root form

These steps help in standardizing the text and reducing dimensionality.

---

## 🔢 Feature Engineering

### 📘 Bag of Words (BoW)
Initially, the text data was transformed using the **Bag of Words** model.

- Bag of Words is a **text encoding technique** that converts textual data into numerical vectors
- It represents text based on the **frequency of words**, ignoring grammar and word order
- A vocabulary is created from the corpus, and each message is represented as a vector

This step allowed the conversion of preprocessed text into machine-readable numerical features.

---

### 📗 TF-IDF (Currently Implementing)
The project is now being extended using **TF-IDF (Term Frequency–Inverse Document Frequency)** vectorization.

- TF-IDF improves upon Bag of Words by **reducing the weight of frequently occurring words**
- It assigns higher importance to words that are more meaningful to a particular document
- Helps in handling high-frequency but less informative terms

🚧 **Currently working on implementing TF-IDF vectors and training models using these features**

---

## 🚀 Next Steps
- Train machine learning models (Naive Bayes, Logistic Regression)
- Compare performance between **Bag of Words** and **TF-IDF**
- Evaluate models using:
  - Accuracy
  - Confusion Matrix
  - Precision, Recall, F1-score

---

## 🧰 Tools & Libraries Used
- Python  
- Pandas, NumPy  
- NLTK  
- Scikit-learn  
- Jupyter Notebook  
- VS Code  

---

## ✍️ Author
**Tasnim Shamsuddin**  
Aspiring Data Scientist | NLP & Machine Learning Enthusiast



