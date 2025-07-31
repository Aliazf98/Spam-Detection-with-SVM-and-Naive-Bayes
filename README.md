# Spam Detection with SVM and Naive Bayes

This project presents a comparative study of two popular machine learning algorithms — **Support Vector Machine (SVM)** and **Gaussian Naive Bayes (GNB)** — for the task of spam email classification. The analysis focuses on preprocessing, training, evaluation, and optimization using the Spambase dataset from the UCI Machine Learning Repository.

---

## Project Motivation

In the digital communication era, spam emails compromise security and productivity. This project addresses this challenge by:
- Applying and comparing two supervised ML algorithms.
- Evaluating their performance on a real-world dataset.
- Recommending an effective model for spam detection tasks.

---

## Dataset

I used the [Spambase dataset](https://archive.ics.uci.edu/dataset/94/spambase) from the UCI Repository.  
It includes **57 numerical features** extracted from emails, with a binary label:  
- `1` = spam  
- `0` = not spam

---

## Preprocessing Steps

- **Cleaning**: Removed missing/erroneous values
- **Feature Scaling**: Standardized features using `StandardScaler`
- **Handling Imbalance**: Applied `RandomOverSampler` to address class imbalance
- **Train-Test Split**: 80/20 ratio for model evaluation

---

## Models Implemented

### 1. **Support Vector Machine (SVM)**
- Kernels: Linear, Polynomial
- Regularization: `C=0.1`, `C=1`, `C=10`

### 2. **Gaussian Naive Bayes (GNB)**
- Assumes features follow a Gaussian distribution
- Fast and effective for high-dimensional data

---

##  Requirements

To run this project, you need the following Python dependencies:

- **Python 3.8+**
- **pandas**
- **numpy**
- **matplotlib**
- **seaborn**
- **scikit-learn**
- **imbalanced-learn**

### Install Dependencies

To install all the required dependencies, run the following command in your terminal:

```bash
pip install -r requirements.txt

