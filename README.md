# Sentiment Analysis on Amazon Product Reviews

## Project Overview
This project applies **Sentiment Analysis** on Amazon product reviews using **Natural Language Processing (NLP)** and **Machine Learning** techniques.  
The goal is to classify reviews into three categories:
- **Positive**
- **Neutral**
- **Negative**

We address **class imbalance** using **SMOTE** and compare two modeling approaches:
1. Logistic Regression with SMOTE  
2. Logistic Regression with GridSearchCV + SMOTE (pipeline)

---

## ⚙Workflow
1. **Data Preprocessing**
   - Text cleaning (removing punctuation, stopwords, lemmatization).
   - Tokenization and vectorization with `TfidfVectorizer`.

2. **Handling Imbalanced Data**
   - Applied **SMOTE** to balance minority classes.

3. **Model Training**
   - Logistic Regression (baseline model).
   - GridSearchCV + SMOTE within pipeline for hyperparameter tuning.

4. **Evaluation**
   - Classification report (precision, recall, F1-score).
   - Confusion matrix visualization.
  

---

##  Results

- **Logistic Regression + SMOTE**  
  Accuracy: ~90%  
  Macro Avg F1: ~0.72  

- **GridSearchCV + SMOTE (Pipeline)**  
  Accuracy: ~88%  
  Macro Avg F1: ~0.69  

 Logistic Regression + SMOTE performed slightly better overall (especially for minority classes).

---


