# Spam Classifier

Simple spam/ham email classifier using Multinomial Naive Bayes and Logistic Regression.

Dataset: [Spam Emails - Kaggle](https://www.kaggle.com/datasets/veleon/ham-and-spam-dataset)

Main steps:
- TF-IDF vectorization
- Train/test split (stratified)
- Model comparison with confusion matrices

Best result so far: Naive Bayes → 100% spam precision, 0 false positives, ~66% recall
