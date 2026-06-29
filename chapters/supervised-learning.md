# Supervised Learning

Supervised learning is one of the most widely used and well-understood types of machine learning. In this approach, the model is trained on **labeled data**, which means each input example is paired with the correct output.

---

## What is Supervised Learning?

In supervised learning, the goal is to **learn a mapping** from inputs (features) to outputs (labels) based on example input-output pairs.

Given:
- A dataset of feature vectors `X` (e.g., age, salary, education)
- Corresponding labels `y` (e.g., approved/rejected)

The model tries to find a function `f(X) = y` that best approximates the true relationship.

---

## Two Main Tasks

### 1. **Regression**
Predicts **continuous** numeric values.

**Examples:**
- Predicting house prices
- Estimating temperature
- Forecasting sales

**Common Algorithms:**
- Linear Regression
- Decision Trees for Regression
- Support Vector Regression (SVR)

---

### 2. **Classification**
Predicts **discrete** labels or categories.

**Examples:**
- Email: spam or not spam
- Image: cat, dog, or bird
- Medical: disease present or not

**Common Algorithms:**
- Logistic Regression
- Decision Trees
- Random Forest
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Support Vector Machines (SVM)

---

## Supervised Learning Workflow

1. **Data Collection**
   - Gather a dataset with input-output pairs.

2. **Data Preprocessing**
   - Clean, normalize, and transform the data.

3. **Split the Dataset**
   - Training set (usually 70–80%)
   - Test set (usually 20–30%)
   - Optional: Validation set (for tuning)

4. **Train the Model**
   - Use the training data to learn patterns.

5. **Evaluate the Model**
   - Use test data and metrics like accuracy, MSE, etc.

6. **Improve the Model**
   - Tune hyperparameters, try different algorithms, feature engineering, etc.

---

## Example: Predicting House Prices

| Feature         | Value         |
|-----------------|---------------|
| Size (sqft)     | 1800          |
| Bedrooms        | 3             |
| Location        | Suburban      |
| Price (label)   | $350,000      |

Using many such rows, a regression model can learn how house characteristics affect price and predict the price of a new house.

---

## Evaluation Metrics

### For Classification:
- **Accuracy**: % of correct predictions
- **Precision**: True positives / Predicted positives
- **Recall**: True positives / Actual positives
- **F1 Score**: Harmonic mean of precision and recall
- **Confusion Matrix**: Table showing TP, FP, FN, TN

### For Regression:
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **R² Score** (coefficient of determination)

---

## Benefits of Supervised Learning

✅ Straightforward to understand and implement  
✅ Effective when you have labeled data  
✅ Broad range of powerful algorithms available  
✅ Used in many practical applications

---

## Limitations

❌ Requires large amounts of labeled data  
❌ Labeling can be expensive or time-consuming  
❌ May not work well if data is noisy or biased  
❌ Susceptible to overfitting without proper validation

---

## Common Use Cases

- Sentiment analysis (positive/negative reviews)
- Email spam detection
- Credit risk assessment
- Medical diagnosis
- Stock price prediction

---

## Summary

Supervised learning is a powerful and flexible approach where learning is guided by examples. Whether you're building a spam filter or predicting housing prices, supervised learning is often the best place to start.

It’s like learning with a teacher — you know the correct answers during training, which allows the model to learn efficiently.

> Next up: Try building a small supervised learning project using tools like **scikit-learn**, and experiment with classification and regression tasks!

