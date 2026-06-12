# 🎬 IMDB Movie Review Sentiment Analysis

An end-to-end Natural Language Processing (NLP) project that classifies IMDB movie reviews as **Positive** or **Negative** using both **Machine Learning** and **Deep Learning** approaches.

The project demonstrates the complete NLP workflow, from text preprocessing and feature engineering to model training, evaluation, and comparison.

---

## 📌 Project Overview

Sentiment Analysis is a fundamental NLP task used to determine the emotional tone of textual data.

In this project, IMDB movie reviews are analyzed and classified into:

* Positive Sentiment (1)
* Negative Sentiment (0)

The notebook implements and compares multiple approaches:

* Logistic Regression
* Multinomial Naive Bayes
* LSTM (Long Short-Term Memory)
* Improved Bidirectional LSTM

---

## 🚀 Features

* Comprehensive text preprocessing pipeline
* TF-IDF based feature extraction
* Traditional Machine Learning models
* Deep Learning models using TensorFlow/Keras
* Model performance comparison
* Visualization of training metrics
* Confusion Matrix and Classification Reports
* ROC-AUC evaluation

---

## 📂 Dataset

The project uses the **IMDB Movie Review Dataset**, which contains movie reviews labeled as positive or negative.

### Dataset Columns

| Column    | Description               |
| --------- | ------------------------- |
| review    | Movie review text         |
| sentiment | Positive / Negative label |

Example:

| Review                  | Sentiment |
| ----------------------- | --------- |
| This movie was amazing! | Positive  |
| Waste of time.          | Negative  |

---

## 🛠️ Tech Stack

### Programming Language

* Python 3.x

### Libraries

#### Data Processing

* Pandas
* NumPy

#### NLP

* NLTK
* WordNet Lemmatizer
* Stopwords

#### Machine Learning

* Scikit-Learn

  * Logistic Regression
  * Multinomial Naive Bayes
  * TF-IDF Vectorizer

#### Deep Learning

* TensorFlow
* Keras

  * Embedding Layer
  * LSTM
  * Bidirectional LSTM
  * Dropout
  * EarlyStopping

#### Visualization

* Matplotlib
* Seaborn

---

## 📊 Workflow

### 1. Data Loading

Load the IMDB dataset into a Pandas DataFrame.

### 2. Text Preprocessing

The reviews undergo several preprocessing steps:

* Lowercasing
* HTML tag removal
* Punctuation removal
* Number removal
* Tokenization
* Stopword removal
* Lemmatization

Example:

Input:

I absolutely loved this movie!!! <br />

Output:

absolutely loved movie

---

### 3. Label Encoding

Convert sentiments into numerical values:

| Sentiment | Value |
| --------- | ----- |
| Positive  | 1     |
| Negative  | 0     |

---

### 4. Train-Test Split

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

---

## 🤖 Models Used

### Logistic Regression

* TF-IDF Features
* Fast and efficient
* Strong baseline model

### Multinomial Naive Bayes

* Probability-based classifier
* Excellent performance on text data
* Computationally lightweight

### LSTM Network

Architecture:

Embedding Layer
↓
Spatial Dropout
↓
LSTM Layer
↓
Dropout
↓
Dense Output Layer

Key Parameters:

* Vocabulary Size: 20,000
* Sequence Length: 200
* Embedding Dimension: 128
* LSTM Units: 128

### Improved Bidirectional LSTM

Architecture:

Embedding Layer
↓
Spatial Dropout
↓
Bidirectional LSTM (128)
↓
Dropout
↓
Bidirectional LSTM (64)
↓
Dropout
↓
Dense (ReLU)
↓
Dropout
↓
Sigmoid Output

Key Improvements:

* Larger vocabulary
* Longer sequence length
* Bidirectional context learning
* Better generalization
* Reduced overfitting

---

## 📈 Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

---

## 📊 Visualizations

The notebook generates:

### Dataset Analysis

* Sentiment Distribution Plot

### Model Evaluation

* Confusion Matrix
* Classification Report

### Deep Learning Analysis

* Accuracy Curves
* Loss Curves

### Performance Comparison

* Accuracy Comparison
* Precision Comparison
* Recall Comparison
* F1 Score Comparison
* ROC-AUC Comparison

---

## 📁 Project Structure

```text
IMDB-Sentiment-Analysis/
│
├── IMDB_Sentiment_analysis.ipynb
├── IMDB Dataset.csv
├── README.md
└── requirements.txt
```

---

## ▶️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/IMDB-Sentiment-Analysis.git
cd IMDB-Sentiment-Analysis
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

1. Open the notebook:

```bash
jupyter notebook
```

or

```bash
jupyter lab
```

2. Open:

```text
IMDB_Sentiment_analysis.ipynb
```

3. Upload the IMDB Dataset when prompted.

4. Run all cells sequentially.

---

## 📋 Expected Results

The project will produce:

* Cleaned review dataset
* TF-IDF feature matrix
* Trained ML models
* Trained Deep Learning models
* Evaluation reports
* Performance visualizations
* Best model identification

---

## 🏆 Results

The Improved Bidirectional LSTM model generally achieves the highest performance due to its ability to learn contextual information from both directions of a sequence.

Typical performance:

* Accuracy: 95%+
* F1 Score: 95%+
* ROC-AUC: 95%+

*(Results may vary depending on train-test split and training environment.)*

---

## 🔮 Future Enhancements

* BERT-based Sentiment Analysis
* RoBERTa Fine-Tuning
* Transformer Architectures
* Hyperparameter Optimization
* Flask/FastAPI Deployment
* Streamlit Web Application
* Real-Time Sentiment Prediction API

---

## 🎓 Learning Outcomes

This project provides practical experience in:

* Natural Language Processing (NLP)
* Text Cleaning & Preprocessing
* Feature Engineering
* Machine Learning Classification
* Deep Learning with LSTM Networks
* Model Evaluation Techniques
* Data Visualization
* End-to-End AI Workflow

---

## 👩‍💻 Author

**Shreya Saha**

B.Tech Student | Artificial Intelligence & Machine Learning Enthusiast

---

## ⭐ Support

If you found this project useful, consider starring the repository and sharing it with others.

```bash
⭐ Star this repository if it helped you!
```
