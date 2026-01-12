🧠 Problem Statement

Spam messages are unsolicited and often harmful. Automatically detecting spam helps improve user experience and protects users from fraud. This project applies NLP techniques to efficiently identify spam messages from SMS data.

📂 Dataset

The dataset consists of labeled SMS messages classified as Spam or Ham.

Each message is processed and transformed into numerical features suitable for machine learning models.

🔧 Data Cleaning & Preprocessing

The following preprocessing steps were applied to the text data:

✅ Conversion of text to lowercase

✅ Removal of punctuation and special characters

✅ Tokenization (splitting text into individual words)

✅ Lemmatization to reduce words to their base form

✅ Removal of unnecessary symbols and noise

⚠️ Important Note on Data Leakage
Before applying Bag of Words or TF-IDF, the dataset was first split into training and testing sets. Feature extraction was performed only on the training data, and then applied to the test data. This approach prevents data leakage, ensuring that the model does not gain prior information from the test set during training.

⚙️ Feature Engineering

To convert textual data into numerical form, the following techniques were used:

1️⃣ Bag of Words (BoW)

Represents text by counting word occurrences

Simple and effective for baseline models

2️⃣ TF-IDF (Term Frequency–Inverse Document Frequency)

Measures word importance across documents

Reduces the impact of commonly used words

Improves model performance compared to BoW

🤖 Model Used

Naive Bayes Classifier

Chosen for its simplicity, speed, and strong performance in text classification tasks such as spam detection

📊 Model Evaluation

The model performance was evaluated using the following metrics:

📈 Accuracy – Overall correctness of the model

🎯 Precision – Accuracy of spam predictions

🔄 Confusion Matrix – Detailed classification results

Evaluation was performed for both:

Bag of Words features

TF-IDF features

TF-IDF provided improved and more reliable performance compared to Bag of Words.

🚀 Results

The model successfully classifies SMS messages into Spam and Ham.

TF-IDF with Naive Bayes achieved better precision and accuracy.

Demonstrates the effectiveness of NLP preprocessing and feature engineering techniques.

🛠️ Technologies Used

Python

Natural Language Processing (NLP)

Scikit-learn

Pandas & NumPy

Naive Bayes Algorithm

📌 Conclusion

This project showcases a complete NLP-based machine learning workflow for SMS spam detection. It highlights the importance of text preprocessing and feature extraction methods like TF-IDF in improving classification performance.

📎 Future Enhancements

Try advanced models like Logistic Regression, SVM, or Deep Learning

Hyperparameter tuning

Deployment as a web application or API

