# Knn-Randomforest-Gradientboosting-Classifiers

Exploratory Data Analysis

The first step in the machine learning pipeline is taking a look at the data to make sure that you
understand what you are working with.
Step1: The file was converted into data frame for convenience.

Step2:Segregated the data into continuous numeric data and categorical data.

Step3: Checked if there are any missing values in the given data sets and found there are no missing
values. If there were missing values, then we can handle that by replacing missing values by 'mean' in
features with continuous numeric data and by 'mode' in features with categorical data. There are no
categorical data.

Step4: Couldn't find Unique Identifier Coulmn.

Step5: Checked whether the given datasets are balanced or not, and found the datasets are balanced.

Step6: Found Correlation between Input variables and Target variable. The correlations were not sig-
nificant.


Baseline Models

Formulated 3 baseline models : 1.Random Forest Classier Below are the accuracies before performing
feature engineering and optimizing the model's hyperparameters.
Value of Accuracy train: 0.993000
value of Accuracy test: 0.698333
2.Gradient Boosting Classifier Below are the accuracies before performing feature engineering and opti-
mizing the model's hyperparameters.
value of Accuracy train: 1.000000
value of Accuracy test: 0.840000
3.K-Nearest Neighbors Classifier Below are the accuracies before performing feature engineering and
optimizing the model's hyperparameters.
value of Accuracy train: 0.826500
value of Accuracy test: 0.723333

Feature Engineering

1. Normalization of Data set. It didn't prove much effective in order to improve accuracy of my baseline
models.

2. Used SelectKBest function to select important features, on which I trained and tested the three models.
For Random Forest Classifier and K-Nearest Neighbors Classifier selected 15 best features for maximum
accuracy and for Gradient Boosting Classifier selected 12 features for maximum accuracy.

The accuracies of the models were improved by tuning the hyper parameters and by Feature Engineering,
for Random Forest, n-estimators was tuned to improve accuracy. In case of Gradient Boosting Classifier
learning rate , n-estimators, max depth were tuned to improve the model accuracy. In case of K Nearest
Neighbors n-neighbors, p, leaf size were tuned to improve the model accuracy.
Selecting important features improved accuracy as well as the running time.
The Models (After tuning the hyperparameters and Feature Engineering)were compared based on their
accuracies on test data and found that Gradient Boosting Classifier gave highest accuracy among all
three models.
The baseline models (Before tuning the hyperparameters and Feature Engineering)were compared based
on their accuracies on test data and found that K-Nearest Neighbors Classifier gave highest accuracy
among all three models.
Yes, there were challenges to tune the hyperparameters and to select best features, optimal hyperparam-
eters combination, a 'for loop code' was written.
There might be some more powerful classification techniques which could have provided better results
