# 📝 Automated Essay Scoring using Machine Learning

## 📌 Project Overview
This project implements an **Automated Essay Scoring (AES)** system using Natural Language Processing (NLP) and Machine Learning techniques.  
The goal is to automatically predict human-like scores for essays based on content quality, structure, and linguistic features.

The system is designed as a **regression problem**, where the model predicts a continuous essay score rather than discrete classes.

---

## 🎯 Objectives
- Automatically score essays based on:
  - Content relevance
  - Coherence and structure
  - Vocabulary richness
  - Linguistic quality
- Compare baseline and advanced machine learning models
- Demonstrate real-world inference by predicting scores for unseen essays

---

## 📂 Dataset
- **Source:** Hugging Face  
- **Dataset:** `jatinmehra/Automated-Essay-Scoring-2.0`
- **Size:** 17,307 essays
- **Score Range:** 1 to 6 (human-graded)

Each essay contains:
- Essay text
- Corresponding human-assigned score

---

## 🧠 Methodology

### 1️⃣ Text Preprocessing
- Lowercasing
- Punctuation and digit removal
- Tokenization
- Stopword removal

### 2️⃣ Feature Engineering
In addition to textual features, structural features were engineered:
- Word count
- Sentence count
- Average word length

These features help capture essay depth, structure, and vocabulary richness.

### 3️⃣ Text Vectorization
- **TF-IDF Vectorization**
  - Unigrams and bigrams
  - Top 5,000 features

### 4️⃣ Model Training
Two regression models were trained and compared:
- **Random Forest Regressor** (baseline)
- **XGBoost Regressor** (final model)

---

## 📊 Model Evaluation


The following regression metrics were used:
- **RMSE (Root Mean Squared Error)**
- **R² Score (Coefficient of Determination)**

### 🔍 Results

| Model | RMSE | R² |
|-----|-----|-----|
| Random Forest Regressor | ~0.42 | ~0.62 |
| **XGBoost Regressor** | **~0.37** | **~0.66** |

**XGBoost outperformed Random Forest**, demonstrating better alignment with human essay scores.

---

## ✍️ Inference on New Essays
The trained model can predict scores for unseen essays by applying:
- The same preprocessing pipeline
- The same TF-IDF vectorizer
- The same engineered features

Predicted scores are **clipped to the valid range [1, 6]** to ensure realistic and interpretable outputs.

Example:
- Short, underdeveloped essay → Lower score
- Structured, content-rich essay → Higher score

This confirms that the model generalizes well and behaves logically.

---

## 🧪 Sanity Check (Human vs Model)
As a qualitative validation step, essays with known human scores were passed through the model.

Example:
- **Human Score:** 4  
- **Model Prediction:** 4.11  

This close alignment demonstrates that the model effectively captures relative essay quality.

---

## 🏁 Conclusion
This project demonstrates a complete end-to-end Automated Essay Scoring pipeline using NLP and machine learning.  
The results show that engineered linguistic features combined with gradient boosting models can effectively approximate human essay scoring behavior.

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- NLTK
- Scikit-learn
- XGBoost
- Hugging Face Datasets

---

## 👤 Author
**[Debaswini-M]**  

