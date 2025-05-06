# 📱 SMS Spam Classifier

A machine learning project that classifies SMS text messages as either **spam** or **ham** (not spam) using natural language processing (NLP) and a linear support vector machine (SVM). The app includes an interactive Gradio interface to test the classifier in real time.

---

## 🎯 Goal

The goal of this project is to accurately identify spam messages using machine learning by:

- Preprocessing and vectorizing text data using **TF-IDF**.
- Training a **LinearSVC** model to classify SMS messages.
- Creating an easy-to-use **Gradio interface** for interactive predictions.

---

## 🧪 Implementation Details

- **Data Source**: SMS Spam Collection from UCI Machine Learning Repository.
- **Preprocessing**:
  - Removed stop words.
  - Converted raw text into TF-IDF vectors.
- **Model**:
  - `LinearSVC` classifier from `scikit-learn`.
  - Trained using a pipeline for efficient transformation and modeling.
- **Evaluation**:
  - Train/Test Split: 67/33 ratio.
  - Accuracy Score: **98.9%** on the test set.
- **Interface**:
  - Built with [Gradio](https://gradio.app) to allow real-time spam prediction via text input.

 ---
 
## 📂 Dataset Overview

The dataset contains 5,572 SMS messages labeled as either **spam** or **ham**.

| Label | Count |
|-------|-------|
| Ham   | 4825  |
| Spam  | 747   |

Each message is stored in two columns:  
- **label** — the classification (`ham` or `spam`)  
- **text_message** — the raw SMS content  

---

## 🧠 Key Findings

- The TF-IDF + LinearSVC pipeline achieved **high accuracy (0.989)** with minimal tuning.
- Stopword removal and vectorization were crucial in reducing noise and improving classification.
- Short promotional texts with keywords like "win", "free", "cash", and "claim" had the highest probability of being classified as **spam**.
- The classifier was robust against slight variations in spam phrasing, showing good generalization.

---

## 🌟 Example Predictions

Input SMS | Predicted Label
--------- | ---------------
"Congrats! You’ve won a free iPhone. Click here to claim now!" | `spam`
"Are we still meeting for lunch tomorrow?" | `ham`
"URGENT! Your account is suspended. Verify now to avoid closure." | `spam`
"Hey, just checking in—how did your interview go?" | `ham`

---

## ✅ Conclusion

This project demonstrates how traditional machine learning methods, combined with simple NLP preprocessing, can be highly effective for spam detection. The pipeline achieved a **98.9% accuracy**, proving its reliability and effectiveness. By integrating the model with Gradio, the project becomes an engaging and practical tool for real-world use.

---

## 🔗 Citation & References

- 📊 **Dataset**  
  Almeida, T. & Hidalgo, J. (2011). *SMS Spam Collection* [UCI Repository].  
  [https://doi.org/10.24432/C5CC84](https://doi.org/10.24432/C5CC84)

- 📚 **Scikit-learn Documentation**  
  [https://scikit-learn.org/stable/documentation.html](https://scikit-learn.org/stable/documentation.html)

- 🛠️ **Gradio Library**  
  [https://gradio.app](https://gradio.app)

- 📄 **Google**  
   [https://google.com](https://google.com)


---
