# classification-challenge

# Spam Email Detection

## Project Overview
This project focuses on building a supervised machine learning model to classify emails as spam or not spam. The goal is to help an Internet Service Provider (ISP) improve its email filtering system for customers. Two machine learning models, Logistic Regression and Random Forest, are created, evaluated, and compared for performance.

---

## Dataset
The dataset contains information about emails, with labels indicating whether the email is:
- **Spam (1)**
- **Not Spam (0)**

### Data Source
The dataset is loaded from: [Spam Data CSV](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)

### Features and Labels
- **Features (X):** All columns except `spam`
- **Label (y):** `spam`

---

## Project Steps

### 1. Data Preparation
- **Data Loading:** The dataset is loaded into a Pandas DataFrame.
- **Feature and Label Selection:** Labels are extracted from the `spam` column, and the remaining columns are used as features.
- **Train-Test Split:** The data is split into training (75%) and testing (25%) sets using `train_test_split`.

### 2. Feature Scaling
- **StandardScaler:** The features are standardized to ensure optimal performance of machine learning models.

### 3. Model Training and Evaluation
Two models are trained and evaluated:
1. **Logistic Regression:**
   - A linear classification model is trained on the scaled training data.
   - The model predicts on the test data, and its accuracy is calculated.

2. **Random Forest Classifier:**
   - A non-linear classification model is trained on the scaled training data.
   - The model predicts on the test data, and its accuracy is calculated.

### 4. Model Comparison
The performance of both models is compared based on their accuracy scores.

---

## Results
- **Logistic Regression Accuracy:** `0.92`
- **Random Forest Accuracy:** `0.95`

### Model Performance
The model with the higher accuracy score is considered better for spam detection. The analysis includes justifications for the performance difference between the models.

---

## Dependencies
This project uses the following Python libraries:
- `pandas`
- `scikit-learn`
- `numpy`

To install all dependencies, use:
```bash
pip install pandas scikit-learn numpy