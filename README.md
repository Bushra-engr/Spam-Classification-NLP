# 📧 Spam Mail Classifier: BoW vs TF-IDF Comparison

This project implements a robust NLP pipeline to classify emails as **Spam** or **Ham**. The focus is on comparing two major vectorization techniques and evaluating them using multiple performance metrics.

## 🚀 Features
- **Text Preprocessing**: Full pipeline including Regex cleaning, tokenization, and Lemmatization.
- **Vectorization**: Implementation of **Bag of Words (CountVectorizer)** and **TF-IDF**.
- **Class Imbalance Handling**: Integrated **SMOTE** to balance the spam/ham distribution.
- **Model Comparison**: Evaluated Multinomial Naïve Bayes and Logistic Regression.
- **Advanced Visualization**: Custom dark-themed dashboard featuring:
  - **Accuracy Bars**: Direct model comparison.
  - **Grouped Metrics**: Precision, Recall, and F1-Score for the Spam class.
  - **Radar Chart**: Holistic performance view.

## 🛠️ Tech Stack
- **Language**: Python 3.x
- **NLP Libraries**: `spaCy`, `NLTK`, `re`
- **Machine Learning**: `Scikit-Learn`, `Imbalanced-Learn (SMOTE)`
- **Visualization**: `Matplotlib`, `Seaborn`

## 📊 Performance Summary
The models are evaluated on the following metrics:
- **Accuracy**: Overall correctness.
- **Precision**: How many predicted "Spam" were actually spam? (Crucial to avoid filtering important emails).
- **Recall**: How many actual "Spam" emails did we catch?
- **F1-Score**: The harmonic mean of Precision and Recall.

### Visual Results
The pipeline generates a `spam_results.png` dashboard:
1. **Accuracy Bar**: Shows which vectorizer yields higher overall hits.
2. **Spam Class Metrics**: Deep dive into how the models handle the minority class.
3. **Radar Chart**: Displays the balance between all four metrics simultaneously.

## 📝 How to Use
1. Ensure `spaCy`'s English model is installed: `python -m spacy download en_core_web_sm`.
2. Run the preprocessing script to clean and lemmatize text.
3. Execute the training script to generate the model and performance plots.

---
*Created by an Aspiring AIML Intern 🚀*
