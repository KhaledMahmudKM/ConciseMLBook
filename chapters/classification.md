# Classification

Classification is a type of supervised learning used when the output variable is a **category** or **label**, such as "spam or not spam", "disease or no disease", or "cat or dog". The goal is to learn a function that maps input features to discrete output classes.

---

## What is Classification?

In classification, the model learns from a labeled dataset to identify which class an input belongs to. It differs from regression in that the output is categorical instead of continuous.

Examples:
- Email → Spam or Not Spam
- Image → Cat or Dog
- Transaction → Fraud or Legitimate

---

## Types of Classification

### 1. **Binary Classification**
Two possible outcomes (e.g., yes/no, 0/1)

### 2. **Multiclass Classification**
More than two classes (e.g., classifying digits 0–9)

### 3. **Multilabel Classification**
Each input can be assigned multiple labels (e.g., a news article tagged as both "sports" and "politics")

---

## Common Algorithms

- **Logistic Regression**
- **Decision Trees**
- **Random Forests**
- **Support Vector Machines (SVM)**
- **Naive Bayes**
- **K-Nearest Neighbors (KNN)**
- **Neural Networks**

---

## How It Works

1. The model is trained on input features and their corresponding labels.
2. It learns patterns in the data that distinguish one class from another.
3. When given new data, it assigns the most likely class label.

---

## Evaluation Metrics

Classification models are evaluated using metrics such as:

- **Accuracy**: Proportion of correct predictions
- **Precision**: Proportion of positive identifications that were actually correct
- **Recall (Sensitivity)**: Proportion of actual positives that were identified correctly
- **F1 Score**: Harmonic mean of precision and recall
- **Confusion Matrix**: A table showing correct vs. incorrect classifications

For imbalanced datasets, precision, recall, and F1 score are more informative than accuracy.

---

## Example: Email Spam Detection

| Features                | Label     |
|-------------------------|-----------|
| Contains "lottery"      | Spam      |
| Contains "meeting"      | Not Spam  |
| From unknown sender     | Spam      |
| Has unsubscribe link    | Not Spam  |

The model learns from labeled emails to predict whether a new email is spam.

---

## Challenges in Classification

- **Class Imbalance**: One class significantly outnumbers the other(s)
- **Overfitting**: Model memorizes training data but performs poorly on new data
- **Underfitting**: Model is too simple to capture patterns
- **Noise**: Incorrect or ambiguous labels

---

## Use Cases

- Spam filtering
- Medical diagnosis
- Image recognition
- Sentiment analysis
- Fraud detection
- Customer segmentation

---

## Summary

Classification is a core task in supervised learning, used to predict categories or labels based on input data. With a variety of models and evaluation metrics available, classification is widely applicable across industries and domains.

> Next step: Try building a simple binary classifier in Python using `scikit-learn`.
