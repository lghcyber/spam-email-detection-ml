# Spam Email Detection Using Naive Bayes

A machine learning project that classifies email messages as spam or legitimate (ham) using Natural Language Processing (NLP), TF-IDF feature extraction, and a Multinomial Naive Bayes classifier.

## 🔍 Project Overview

The goal of this project is to build a binary classification model capable of identifying spam emails.

Email text is cleaned and transformed into numerical features using TF-IDF before being passed to a Multinomial Naive Bayes classifier.

## 🛠️ Technologies Used

- Python
- Pandas
- NLTK
- Scikit-learn
- TF-IDF
- Multinomial Naive Bayes
- Matplotlib
- Jupyter Notebook

## ⚙️ Methodology

### 1. Text Preprocessing

The email text was prepared by:

- Converting text to lowercase
- Removing punctuation, numbers, and special characters
- Removing English stopwords using NLTK
- Applying stemming to reduce words to their base forms

### 2. Feature Extraction

TF-IDF was used to transform the cleaned email text into numerical features.

TF-IDF assigns greater importance to informative words while reducing the influence of commonly occurring terms.

### 3. Model Training

The dataset was split into:

- **80% training data**
- **20% testing data**

A Multinomial Naive Bayes classifier was trained on the resulting TF-IDF features.

### 4. Model Evaluation

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- AUROC
- AUPRC
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve

## 📊 Results

| Metric | Score |
|---|---:|
| Accuracy | 88.82% |
| Precision | 100.00% |
| Recall | 53.45% |
| F1-Score | 69.66% |
| AUROC | 76.72% |
| AUPRC | 65.23% |

## 📈 Results Analysis

The classifier achieved **88.82% accuracy and 100% precision**.

The perfect precision indicates that the model did not incorrectly classify legitimate emails as spam in the evaluated test set.

However, recall was **53.45%**, meaning the classifier missed a substantial portion of the actual spam messages.

This highlights an important security tradeoff: minimizing false positives while still detecting as many unwanted or potentially malicious messages as possible.

### Potential Improvements

- Use lemmatization instead of stemming
- Test n-grams to capture additional context between words
- Experiment with alternative classification algorithms
- Perform additional feature engineering
- Tune model and feature-extraction parameters
- Explore techniques for improving recall while maintaining strong precision

## 📁 Repository Structure

```text
spam-email-detection-ml/
│
├── spam_email_detection_naive_bayes.ipynb
└── README.md
```

## ▶️ Running the Project

Open the Jupyter Notebook:

```text
spam_email_detection_naive_bayes.ipynb
```

The notebook contains the text preprocessing, TF-IDF feature extraction, model training, predictions, evaluation metrics, and performance visualizations used in the experiment.

## 🔐 Cybersecurity Relevance

Spam and phishing emails are common delivery mechanisms for social engineering and other cybersecurity threats.

Automated email classification can help identify suspicious or unwanted messages and support email security workflows.

This project demonstrates experience with:

- Email classification
- Natural Language Processing
- Machine learning for security applications
- Text preprocessing
- TF-IDF feature extraction
- Binary classification
- Model evaluation
- Precision and recall analysis

## 🎓 Project Context

This project was completed as part of my cybersecurity coursework at the University of South Carolina Upstate.

## 👤 Author

**Alani Hodge**  
Cybersecurity Student | Security Operations | Threat Detection

[LinkedIn](https://www.linkedin.com/in/alani-hodge) | [GitHub](https://github.com/lghcyber)
