# SMS Spam Detection

This project focuses on detecting whether a given text message is "ham" (non-spam) or "spam." It utilizes Natural Language Processing (NLP) techniques and machine learning to classify SMS messages into these two categories.

## Problem Statement

The objective of this project is to build a model capable of distinguishing between legitimate ("ham") and unwanted ("spam") text messages. The solution involves text preprocessing, feature extraction, and training a machine learning model.

## Technologies Used

- Python
- Jupyter Notebook
- Libraries:
  - nltk (Natural Language Toolkit)
  - re (Regular Expressions)
  - scikit-learn (CountVectorizer, Multinomial Naive Bayes)
  
## Dataset

The dataset used for this project is sourced from [https://raw.githubusercontent.com/sunnysavita10/Naive-Bayes/main/SpamClassifier-with-ML/sms_spam_data/SMSSpamCollection.csv]. It includes labeled examples of SMS messages, indicating whether each message is "ham" or "spam."

## Approach

1. **Data Loading:** The dataset is loaded using the pandas library.
2. **Text Preprocessing:** The text messages undergo preprocessing steps, including converting to lowercase, removing non-alphabetic characters, and stemming.
3. **Feature Extraction:** The CountVectorizer from scikit-learn is used to convert the preprocessed text into numerical features.
4. **Model Training:** The Multinomial Naive Bayes classifier is trained on the feature matrix and corresponding labels.
5. **Model Evaluation:** The model is evaluated using metrics such as accuracy and classification report on a test set.
6. **Prediction:** The trained model can be used to predict whether a new message is "ham" or "spam."

## Result

The model achieved an accuracy of 97.93% on the test set. Further details can be found in the classification report within the notebook.

## Sample Predictions

1. For the message: "Free entry in 2 a wkly comp to win FA Cup fina...", the model predicts: spam
2. For the message: "Thanks gaurav for the update. This provides clear visibility for the next release.", the model predicts: ham
