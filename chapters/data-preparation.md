# Data Preparation

Data preparation is a critical step in any machine learning pipeline. Before feeding data into a machine learning model, it must be cleaned, transformed, and structured appropriately to ensure high-quality results.

---

## Why Data Preparation Matters

Raw data is often incomplete, inconsistent, or noisy. Data preparation helps:
- Improve model performance
- Reduce biases
- Prevent overfitting or underfitting
- Ensure more accurate predictions

---

## Steps in Data Preparation

### 1. **Data Collection**
Gathering data from various sources:
- Databases
- APIs
- Files (CSV, Excel, JSON)
- Web scraping

### 2. **Data Cleaning**
Fixing or removing incorrect, corrupted, or missing data.

#### Common tasks:
- Handling missing values (impute or remove)
- Correcting data types
- Removing duplicates
- Fixing formatting errors

### 3. **Handling Missing Data**

Techniques include:
- Removing rows or columns with too many missing values
- Filling missing values with:
  - Mean/Median/Mode
  - Constant value
  - Forward/Backward fill

### 4. **Feature Engineering**

Creating new features from existing data to improve model performance.

Examples:
- Converting timestamps into day, month, or hour
- Combining text fields into one
- Creating interaction terms

### 5. **Feature Selection**

Choosing relevant features to reduce noise and overfitting.

Techniques:
- Correlation analysis
- Recursive feature elimination (RFE)
- Feature importance from models

### 6. **Encoding Categorical Variables**

Convert categorical variables into numerical format.

- **Label Encoding**: Each category is assigned a number
- **One-Hot Encoding**: Creates binary columns for each category

### 7. **Data Normalization / Scaling**

Ensures that features are on a similar scale.

- **Min-Max Scaling**: Rescales data to [0, 1]
- **Standardization (Z-score)**: Rescales data to have zero mean and unit variance

### 8. **Splitting the Dataset**

Divide data into:
- **Training Set** (usually 70–80%): For training the model
- **Validation Set** (optional): For tuning hyperparameters
- **Test Set** (usually 20–30%): For final evaluation

Use tools like `train_test_split()` from `sklearn`.

---

## Tools for Data Preparation

- **Pandas**: For data manipulation
- **NumPy**: For numerical operations
- **scikit-learn**: For preprocessing utilities
- **OpenRefine**: For data cleaning
- **SQL**: For querying structured data

---

## Best Practices

- Always visualize the data to understand distributions and relationships
- Maintain a data preparation pipeline for reproducibility
- Handle data leakage by avoiding peeking into test data
- Document all preprocessing steps

---

## Summary

Data preparation is a vital foundation for building successful machine learning models. Well-prepared data leads to better insights, better models, and better outcomes.

> "Garbage in, garbage out" — A machine learning model is only as good as the data it's trained on.
