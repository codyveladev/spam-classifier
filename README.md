# Spam Classifier

Simple spam/ham email classifier using Multinomial Naive Bayes and Logistic Regression.

Dataset: [Spam Emails - Kaggle](https://www.kaggle.com/datasets/abdallahwagih/spam-emails)

Process: 
- Load the data from the CSV into a panda dataframe
- Show a quick visualization of the breakdown of spam/ham classification
- Encode the target column 'Category' in order for this to be used in the models later
- Split the training and test data from the entire dataset
- Vectorize the message for the training and test data (transforming the text into numeric representation for model use)
- Train the LogisticRegression model on the training data
- Perform classification task with LogisticRegression model and display accuracy
- Train the MultinomialNB model on the training data
- Perform classification task with MultinomialNB model and display accuracy
- Create and display Confusion Matrix for both model outputs

Best result so far: Naive Bayes → 100% spam precision, 0 false positives, ~66% recall

Discussion and Next Steps: 
This project taught me foundational processes of solving classification problems using machine learning by following the steps above. What we did here is the basis of all classification problems using models based classification. Confusion matrix are important in classification problems at is shows a breakdown of the false postives, false negatives, true positives, and true negatives. This shows the performance of the model in a deeper view then just the accuracy.

About the models:
Logistic Regression
This is used when the outcome is categorical, in this example the message is spam or ham, it is a linear mdel that examines the relationship between predictor variables (message) and an output variable (category).

Multinomial Naive Bayes
A machine learing classifier which is popular with text analysis. Good for features are counts or frequencies, such as word occurrences in a document. The "naive" assumption assumes all words/features are independent of each other. So, this means that the word doesnt affect the next one "click this" for example, could be combined but in this approach it's treated as seperate.

Next steps would be to implement different models, attempt to do some preprocessing of the messages (i.e help classify spam words), and potentially try to solve this problem using a small neural network.

