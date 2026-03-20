# 🚀 Supplier Ticket Classification using NLP & Deep Learning

---

## 📌 Overview
This project focuses on **classifying supplier support tickets** into:

- ✅ ACTIONABLE  
- ❌ NON-ACTIONABLE  

It uses a hybrid NLP approach combining:
- 🧠 BERT Embeddings  
- 🏷️ Named Entity Recognition (NER)  
- 📄 TF-IDF Features  
- 🤖 MLP Classifier with Optuna tuning  

---

## 🧠 Tech Stack

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-orange?logo=scikit-learn)
![SpaCy](https://img.shields.io/badge/SpaCy-green)
![PyTorch](https://img.shields.io/badge/PyTorch-red?logo=pytorch)
![Optuna](https://img.shields.io/badge/Optuna-Hyperparameter%20Tuning-blueviolet)

---

## ⚙️ Features

✨ Advanced text preprocessing  
✨ Hybrid feature engineering (BERT + TF-IDF + NER)  
✨ Data balancing using Random Oversampling  
✨ Hyperparameter tuning using Optuna  
✨ Stratified K-Fold Cross Validation  
✨ Multi-metric evaluation  

---

## 🏗️ Workflow

```mermaid
graph TD
A[Raw Ticket Data] --> B[Text Cleaning]
B --> C[NER Features]
B --> D[BERT Embeddings]
B --> E[TF-IDF]
C --> F[Feature Combination]
D --> F
E --> F
F --> G[Data Balancing]
G --> H[Optuna Tuning]
H --> I[MLP Classifier]
I --> J[Cross Validation]
J --> K[Evaluation]
