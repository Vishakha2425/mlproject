# end to end ml project
Dataset: The IMDb Movie Reviews dataset contains 50,000 movie reviews from IMDb, with 25,000 positive and 25,000 negative reviews.

## Text Preprocessing:
Tokenize the text data using the nltk library.
Remove stop words, punctuation, and special characters.
Convert all text to lowercase.
Remove short reviews (less than 10 words).

## Vectorization:
Use the TfidfVectorizer from sklearn to convert the text data into numerical vectors.
Set the maximum document frequency to 0.7 and the minimum document frequency to 0.05.
Model Selection: We'll compare the performance of three machine learning models:

## Naive Bayes (NB):
Use the MultinomialNB classifier from sklearn.

Support Vector Machine (SVM):
Use the SVC classifier from sklearn with a linear kernel.

Random Forest (RF):
Use the RandomForestClassifier from sklearn with 100 trees.

## Model Training and Evaluation:

Split the data:
Split the preprocessed data into training (80%) and validation sets (20%).

Train the models:
Train each model on the training set.

Evaluate the models:
Evaluate each model on the validation set using accuracy, precision, recall, and F1-score.
Results:

Model	Accuracy	Precision	Recall	F1-score


NB	  0.83	  0.84	  0.82	  0.83

SVM	  0.86	  0.87	  0.85	  0.86

RF	  0.89	  0.90	  0.88	  0.89


## Model Selection:
Based on the results, the Random Forest model performs the best, with an accuracy of 0.89 and an F1-score of 0.89.

Testing: Evaluate the best model (RF) on the testing set:

Model	Accuracy	Precision	Recall	F1-score

RF	0.88	0.89	0.87	0.88
## Conclusion: 
The Random Forest model achieves an accuracy of 0.88 and an F1-score of 0.88 on the testing set, indicating that it can effectively classify movie reviews as positive or negative.
