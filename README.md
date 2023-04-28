# Sentiment Analysis of Musical Instrument Reviews

This project is about sentiment analysis of musical instrument reviews. The goal is to develop a machine learning model that can classify a review as positive or negative based on its text.

## Dataset 
The dataset used in this project consists of customer reviews of musical instruments, from Kaggle. The dataset contains 10K reviews and their corresponding sentiment labels (positive or negative).

## Approach
The following steps were taken in this project:
- Data cleaning and exploration
- Text preprocessing (tokenization, stopwords removal, stemming, etc.)
- Balancing the dataset using SMOTE (Synthetic Minority Over-sampling Technique)
- Vectorizing the text data using TF-IDF (Term Frequency-Inverse Document Frequency) method
- Training several machine learning models on the balanced data using cross-validation
- Evaluating the models' performance using precision, recall, F1-score, and accuracy metrics
- Selecting the best model and saving it using pickle

## Results
The best model was a logistic regression model with a TF-IDF vectorizer, which achieved an accuracy of 95.7% on the test set. 
* The overall accuracy of the model is 0.95, indicating that is performing well in classifying the reviews as positive and negative
* The precision for both cases are very good 
* The recall for the positive reviews is 0.99, indicating that the model is very good identoifying positive reviews as positive
* The recall for the negative reviews is less precise then the positive
* The F1-score for positive reviews is very high, indicating that the model is very good at identifying positive reviews
* The F1-score for negative reviews is also very high, indicating that the model is very good at identifying negative reviews
* The weighted average F1-score of the model is 0.957, which is quite high and indicates that the model is performing well overall

## Final conclusions:
* The dataset was highly imbalanced with a majority of positive reviews compared to negative reviews
* Balancing the dataset using SMOTE improved the model's performance significantly by increasing its ability to identify negative reviews
* The accuracy score of the best model was high at 95.6%
* The precision and recall scores were high for both positive and negative reviews. The model was better at identifying positive reviews, but it still performed well for negative reviews
* The macro-average F1-score was 0.96, indicating good performance on both classes, while the weighted average F1-score was slightly lower at 0.95
* Limited variety of the datset, with most of the reviews being for guitars
* Future work could include expanding the datset with more varaity of reviews or products and use other NLP techiques to improve performce.
