# Sentiment-Analysis

# Sentiment Analysis using SVM and TF-IDF  

## 📖 Project Overview  
This project classifies **customer reviews into Positive and Negative sentiments** using machine learning. Text data was preprocessed, converted into numerical vectors using **TF-IDF**, and modeled with **Support Vector Machines (SVM)**. The model achieved strong performance across multiple metrics.  

---

## 📂 Dataset  
- **Size:** 1,000+ customer reviews  
- **Columns:**  
  - `Id` → unique identifier  
  - `Text` → review content  
  - `Sentiment` → Positive / Negative  
  - `Platform` → review source  
- **Preprocessing Steps:**  
  - Removed irrelevant columns (`Unnamed: 0`, `Unnamed: 0.1`)  
  - Renamed identifiers  
  - Cleaned sentiment labels (removed whitespaces)  
  - Filtered binary classes (Positive, Negative)  

---

## ⚙Methodology  

### 🔹 Data Preprocessing  
- Cleaned and filtered dataset  
- Stratified **train-test split (80/20)**  

### 🔹 Feature Engineering  
- Applied **TF-IDF Vectorizer** with `max_features=5000`  
- Each review transformed into a **5,000-dimensional vector**  

### 🔹 Modeling  
- Trained **SVM Classifier** with:  
  - Linear Kernel  
  - RBF Kernel  

### 🔹 Evaluation Metrics  
- **Accuracy:** ~88%  
- **Precision:** 86%  
- **Recall:** 87%  
- **ROC-AUC:** 0.90  
- Visualized with **Confusion Matrix & ROC Curve**  

---

## Results  
- **Linear SVM** outperformed RBF Kernel  
- TF-IDF effectively captured word importance  
- Achieved strong classification results on unseen reviews  

---

## Key Learnings  
- Importance of **data cleaning** in NLP tasks  
- TF-IDF’s role in converting text into numerical features  
- Effectiveness of **SVM** in high-dimensional spaces  
- Evaluating models with multiple metrics beyond accuracy  

---

## Future Improvements  
- Increase dataset size for better generalization  
- Try other ML models (**Logistic Regression, Random Forest, XGBoost**)  
- Explore **deep learning approaches (LSTM, BERT)**  
- Extend to **multiclass sentiment analysis** (Neutral, Mixed)  

---

## Tech Stack  
- **Python**  
- **Pandas, NumPy**  
- **Scikit-learn**  
- **Matplotlib, Seaborn**  

---

- This project demonstrates how machine learning can analyze real-world text data to understand customer sentiment effectively.
