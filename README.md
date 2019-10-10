# Amazon Fine Food Review Analysis Using Various Machine Learning Models<br>
![](Amazon_Fine_food_reviews.jpg)
__Performed Data Cleaning, Text Preprocessing, Converted Text Data to Numeric Vectors, Applied Various ML Models on the Numeric Data.__<br>
___
__Objective : Given a review, determine whether the review is positive (Rating of 4 or 5) or negative (rating of 1 or 2).__<br>
___
__About Dataset__<br>
Data Source: https://www.kaggle.com/snap/amazon-fine-food-reviews <br>


The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.<br>

Number of reviews: 568,454<br>
Number of users: 256,059<br>
Number of products: 74,258<br>
Timespan: Oct 1999 - Oct 2012<br>
Number of Attributes/Columns in data: 10 

Attribute Information:

1. Id
2. ProductId - unique identifier for the product
3. UserId - unique identifier for the user
4. ProfileName
5. HelpfulnessNumerator - number of users who found the review helpful
6. HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
7. Score - rating between 1 and 5
8. Time - timestamp for the review
9. Summary - brief summary of the review
10. Text - text of the review<br>

The dataset is available in two forms
1. .csv file
2. SQLite Database

In order to load the data, We have used the SQLITE dataset as it easier to query the data and visualize the data efficiently.
<br> 

Here as we only want to get the global sentiment of the recommendations (positive or negative), we will purposefully ignore all Scores equal to 3. If the score id above 3, then the recommendation wil be set to "positive". Otherwise, it will be set to "negative".
___
## Data Cleaning
- Removing Duplicate Data.
- Removing Ambiguous Data.
- Removing Null Text Data.
___
## Text Preprocessing
1. Removing __HTML__ Links and Tags.
2. Removing Special Character and Punctuations.
3. Removing Alpha NUmeric Letter.
4. Perform Decontraction.
5. Converting Text to Lower Case.
6. Removing Stop Words.
7. Stemming the Words.
___
## Featurization: Converting Text Data to Numeric Vectors
- Convert Text Data to Bag of Words.
- Convert Text Data to Bi-Grams/n-grams.
- Convert Text Data to term frequency-Inverse Document Frequency(tf-idf).
- Convert Text Data to Average Word2Vector.
- Convert Text Data to weighted tf-idf Word2Vector.
___
### 1. Amazon Food Reviews Explanatory Data Analysis and Visualizing Data using t-Stochastic Neighborhood Embedding(TSNE)
- Visualize BOW vectors using TSNE.
- Visualize tf-IDF vectors using TSNE.
- Visualize Avg W2V vectors using TSNE.
- Visualize Weighted tf-IDF W2V vectors using TSNE.
___
### 2. Amazon Food REview Analysis using K-Nearest Neighbors

> - Find the right Hyperparameter using Area Under the Receiver Operating Curve(ROC).
> - Plot F1 Scores Vs Hyperparameter.
> - PLot Confusion Matrices.
> - Plot Pretty Table to compare all the different Implementations.
> - Also find the Accuracy of Algorithms.
- Brute force KNN on BOW Vector.
- Brute force KNN on tf-IDF.
- Brute force KNN on Avg W2V.
- Brute force KNN on Weighted tf-IDF W2V.
- kd-Tree Implementation of KNN on BOW Vector.
- kd-Tree Implementation of KNN on tf-IDF.
- kd-Tree Implementation of KNN on Avg W2V.
- kd-Tree Implementation of KNN on Weighted tf-IDF W2V.<br>
Analysis using KNN on different patterned Data.
___
### 3. Amazon Food Reviews Analysis using Logistic Regression
> - Find the right Hyperparameter using Area Under the Receiver Operating Curve(ROC).
> - Plot F1 Scores Vs Hyperparameter.
> - PLot Confusion Matrices.
> - Predict Top 10 Features of the Positive and Negative Class(Feature Importance).
> - Performing perturbation test (multicollinearity check).
> - Plot Pretty Table to compare all the different Implementations.
> - Also find the Accuracy of Algorithms.
> - Write Summary for Implementation.
- Logistic Regression with "l1" regularization on BOW.
- Logistic Regression with "l2" regularization on BOW.
- Logistic Regression with "l1" regularization on tf-IDF.
- Logistic Regression with "l2" regularization on tf-IDF.
- Logistic Regression with "l1" regularization on Avg W2V
- Logistic Regression with "l2" regularization on Avg W2V.
- Logistic Regression with "l1" regularization on Weighted tf-IDF W2V.
- Logistic Regression with "l2" regularization on tf-IDF W2V.
___
### 4. Amazon Food Reviews Analysis using Naive Bayes
> - Find the right Hyperparameter using Area Under the Receiver Operating Curve(ROC).
> - Plot F1 Scores Vs Hyperparameter.
> - PLot Confusion Matrices.
> - Predict Top 10 Features of the Positive and Negative Class(Feature Importance).
> - Perform Feature Engineering to Improve Model Performance.
> - Plot Pretty Table to compare all the different Implementations.
> - Also find the Accuracy of Algorithms.
- Naive Bayes on BOW.
- Naive Bayes on tf-IDF.
- Naive Bayes on BOW after Feature Engineering.
- Naive Bayes on tf-IDF after Feature Engineering.
___
### 5. Amazon Food Reviews Analysis using Support Vector Machine
> - Find the right Hyperparameter using Area Under the Receiver Operating Curve(ROC).
> - Plot F1 Scores Vs Hyperparameter.
> - PLot Confusion Matrices.
> - Predict Top 10 Features of the Positive and Negative Class(Feature Importance).
> - Use Linear Kernel and Radial Basis Function Kernel.
> - Plot Pretty Table to compare all the different Implementations.
> - Also find the Accuracy of Algorithms.
- SVM with "l1" regularization and Linear Kernel on BOW.
- SVM with "l2" regularization and Linear Kernel on BOW. 
- SVM with "l1" regularization and Linear Kernel on tf-IDF.
- SVM with "l2" regularization and Linear Kernel on tf-IDF.
- SVM with "l1" regularization and Linear Kernel on Avg W2V.
- SVM with "l2" regularization and Linear Kernel on Avg W2V.
- SVM with "l1" regularization and Linear Kernel on Weighted tf-IDF W2V.
- SVM with "l2" regularization and Linear Kernel on tf-IDF W2V.
- SVM with RBF Kernel on BOW.
- SVM with RBF Kernel on tf-IDF.
- SVM with RBF Kernel on Avg W2V.
- SVM with RBF Kernel on Weighted tf-IDF W2V.
___
### 6. Amazon Food Review using Decision Tree
> - Find the right Hyperparameter using Area Under the Receiver Operating Curve(ROC).
> - Plot F1 Scores Vs Hyperparameter.
> - PLot Confusion Matrices.
> - Plot Decision Trees.
> - Plot Pretty Table to compare all the different Implementations.
> - Also find the Accuracy of Algorithms.
- Decision Tree on BOW.
- Decision Tree on tf-IDF.
- Decision Tree on Avg W2V.
- Decision Tree on Weighted tf-IDF W2V.
