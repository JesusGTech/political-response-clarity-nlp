# 📊 Political Response Clarity Classification

NLP model that classifies political question-answer pairs by response clarity using TF-IDF and machine learning models.

---

## 🧠 Overview

This project focuses on analyzing political language and classifying how clearly a response answers a question.

Given a question and its answer, the model predicts one of three labels:

- Clear Reply  
- Ambivalent  
- Clear Non-Reply  

Political responses are often indirect or vague, making this a challenging Natural Language Processing (NLP) task.

---

## 🎯 Goal

Build a machine learning model that can detect whether a political answer:

- Directly answers the question  
- Is unclear or ambiguous  
- Does not answer the question  

---

## ⚙️ Methods

### 🔹 Method 1: TF-IDF + Logistic Regression

- Combined question and answer into one text input  
- Converted text into numerical features using TF-IDF  
- Trained a Logistic Regression classifier  

This method serves as a simple baseline using word frequency patterns.

---

### 🔹 Method 2: TF-IDF + Linear SVM

- Used same TF-IDF features  
- Added n-grams (1–3 words) for more context  
- Trained a Linear Support Vector Machine (SVM)  

This model performs better at separating classes in high-dimensional text data.

---

## 📊 Results

Evaluation metric: **Macro F1-score**

| Model | Score |
|------|------|
| Logistic Regression | 0.48 |
| Linear SVM | 0.55 |

The SVM model performed better overall, especially in distinguishing clearer response types.

---

## 🔍 Key Insights

- Ambivalent responses are easier to detect due to language patterns  
- Clear Reply vs Clear Non-Reply is more difficult  
- Traditional models struggle with understanding intent and context  

---

## 🛠️ Tech Stack

- Python  
- pandas  
- scikit-learn  
- TF-IDF Vectorization  
- Logistic Regression  
- Linear SVM  

---

## 📁 Project Structure
