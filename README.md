# Sentiment-Analysis

Project Overview

This project focuses on classifying customer reviews into Positive and Negative sentiments using machine learning techniques. Text data was preprocessed, converted into numerical vectors using TF-IDF, and modeled with Support Vector Machines (SVM). The model was evaluated using multiple metrics, achieving strong performance.

📂 Dataset

Size: 1,000+ customer reviews

Columns:

Id → unique identifier

Text → review content

Sentiment → Positive or Negative label

Platform → source of the review

Preprocessing:

Removed unnecessary columns (Unnamed: 0, Unnamed: 0.1)

Renamed identifiers

Stripped whitespaces in labels

Filtered binary sentiments (Positive/Negative)

⚙️ Methodology
1. Data Preprocessing

Handled irrelevant columns and reformatted column names

Cleaned and filtered sentiment classes

Created train-test split (80/20 stratified)

2. Feature Engineering

Used TF-IDF Vectorizer with max_features=5000 to represent text data numerically

Each review was transformed into a 5,000-dimensional vector capturing word importance

3. Modeling

Implemented Support Vector Machine (SVM) with:

Linear Kernel

RBF Kernel

Trained models on the transformed dataset

4. Evaluation Metrics

Accuracy: ~88%

Precision: 86%

Recall: 87%

ROC-AUC: 0.90

Confusion Matrix & ROC Curve plotted for visualization

📊 Results

Linear SVM performed better than RBF Kernel

TF-IDF with top 5,000 features captured the most important words for sentiment classification

The model achieved strong performance in predicting unseen reviews

🚀 Key Learnings

Importance of data cleaning in text-based datasets

How TF-IDF effectively transforms unstructured text into numerical features

SVM’s effectiveness in high-dimensional text classification problems

Using multiple evaluation metrics (Accuracy, Precision, Recall, ROC-AUC) to judge model performance

🔮 Future Improvements

Expand dataset size to improve model generalization

Experiment with advanced models such as Logistic Regression, Random Forest, or XGBoost

Try deep learning approaches (LSTMs, BERT) for better performance

Add support for multiclass sentiment classification (Neutral, Mixed)

🛠️ Tech Stack

Python

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn
